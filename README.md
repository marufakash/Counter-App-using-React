## Counter App using React

- [Click here to see the demo](https://using-react-counter-app.netlify.app/)

    ```JavaScript
    import React, { useState } from 'react';
    import style from './counter.module.css';

    const Counter = () => {
        const [count, setCount] = useState(0);

        return (
            <div className={style.counter}>
                <h1>Counter App using React</h1>
                <h1 className={style.count}>{count}</h1>
                <div>
                    <button onClick={() => setCount(count-1)}>DECREASE</button>
                    <button onClick={() => setCount(0)}>RESET</button>
                    <button onClick={() => setCount(count+1)}>INCREASE</button>
                </div>
            </div>
        )
    }

    export default Counter;
    ```