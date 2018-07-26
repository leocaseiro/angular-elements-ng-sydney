## Refs and the DOM

```
class MyComponent extends React.Component {
  constructor(props) {
    super(props);
    this.myRef = React.createRef();
  }
  render() {
    return <my-web-component ref={this.myRef}></my-web-component>;
  }
}
```

```
const node = this.myRef.current;
node.messages = [];
```

https://reactjs.org/docs/refs-and-the-dom.html
