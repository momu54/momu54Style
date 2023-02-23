# 變數

1. 命名
    1. 常數
        - 常數全部使用大寫字母
        ```js
        const FOO = 0;
        ```
        - 當需要將單字分開時，使用底線
        ```js
        const FOO_ID = 1;
        ```
    2. 變數
        - 變數全部使用小寫字母
        ```js
        const name = 'momu54';
        ```
        - 不分隔
        ```js
        const livingcountry = 'Taiwan';
        ```
    3. `for (;;)` 迴圈
        - `for (;;)` 迴圈使用 **i** 作為次數
        ```js
        for (let i = 0; i < 100; i++) {
        	// Do something...
        }
        ```
        - 當有一個以上的迴圈時使用後面的字母
        ```js
        for (let i = 0; i < 200; i++) {
        	for (let j = 0; i < 400; i++) {
        		// Do something...
        	}
        }
        ```
2. 賦值

    1. 解構賦值

        - 當需要將物件的值賦值給變數時，優先使用解構賦值

            **這樣做**

            ```js
            const theobject = {
            	foo: 'bar',
            	bar: 'foo',
            };
            const { foo: foo1, bar: bar1 } = theobject;

            const thearray = ['foo', 'bar'];
            const [foo2, bar2] = thearray;
            ```

            **不要這樣做**

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
