> Passing props is how information flows in React apps, from parents to children.

Propsで親から子へと情報が流れる．


> As a next step, we want the Square component to “remember” that it got clicked, and fill it with an “X” mark. To “remember” things, components use state.

状態を記憶するためには，stateを利用する．

> React components can have state by setting this.state in their constructors. this.state should be considered as private to a React component that it’s defined in.

constructorでthis.stateを初期化する．componentに個別である．

> When you call setState in a component, React automatically updates the child components inside of it too

子にも変更は伝わる．


> We may think that Board should just ask each Square for the Square’s state. Although this approach is possible in React, we discourage it because the code becomes difficult to understand, susceptible to bugs, and hard to refactor. Instead, the best approach is to store the game’s state in the parent Board component instead of in each Square.

子要素のstateを参照するより，親要素にstateを持たせる方がいい，という例をしている．


> Since the Square components no longer maintain state, the Square components receive values from the Board component and inform the Board component when they’re clicked. In React terms, the Square components are now controlled components. The Board has full control over them.

Square自体はBoardにonClickを報告しているだけなので，controlled componentsと呼ばれる．
