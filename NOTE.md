> Passing props is how information flows in React apps, from parents to children.

Propsで親から子へと情報が流れる．


> As a next step, we want the Square component to “remember” that it got clicked, and fill it with an “X” mark. To “remember” things, components use state.

状態を記憶するためには，stateを利用する．

> React components can have state by setting this.state in their constructors. this.state should be considered as private to a React component that it’s defined in.

constructorでthis.stateを初期化する．componentに個別である．

> When you call setState in a component, React automatically updates the child components inside of it too

子にも変更は伝わる．


