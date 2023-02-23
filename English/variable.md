# Variable

1. Name
    1. Constant
        - Use all capital letters for constants.
        ```js
        const FOO = 0;
        ```
        - Use underscores when you need to separate words.
        ```js
        const FOO_ID = 1;
        ```
    2. Variable
        - Use all lowercase letters for variables.
        ```js
        const name = 'momu54';
        ```
        - Don't separate.
        ```js
        const livingcountry = 'Taiwan';
        ```
    3. `for (;;)` loop
        - `foo (;;)` loop uses **i** as the count.
        ```js
        for (let i = 0; i < 100; i++) {
        	// Do something...
        }
        ```
        - Use the following letter when there is more than one loop.
        ```js
        for (let i = 0; i < 200; i++) {
        	for (let j = 0; i < 400; i++) {
        		// Do something...
        	}
        }
        ```
2. Assignment

    1. Destructuring assignment

        - When you need to assign the value of an object to a variable, use destructuring assignment first.

            **Do this**

            ```js
            const theobject = {
            	foo: 'bar',
            	bar: 'foo',
            };
            const { foo: foo1, bar: bar1 } = theobject;

            const thearray = ['foo', 'bar'];
            const [foo2, bar2] = thearray;
            ```

            **Don't do this**

            ```js
            const theobject = {
            	foo: 'bar',
            	bar: 'foo',
            };

            const foo1 = theobject.foo;
            const bar1 = theobject.bar;

            const thearray = ['foo', 'bar'];
            const foo2 = thearray[0];
            const bar2 = thearray[1];
            ```
