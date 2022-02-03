# getting start

```bash
yarn add -D esbuild
yarn add -D react react-dom
```

*app.jsx*

```jsx
import * as React from 'react'
import * as ReactDOM from 'react-dom'

let Greet = () => <h1>Hello, world!</h1>

ReactDOM.render(
    <Greet />,
    document.getElementById('app')
)
```

変換

```bash
npx esbuild app.jsx --bundle --outfile=out.js
```

index.html

確認用

```html
<!DOCTYPE html>
<html>
<head>
    <title>esbuild sample</title>
</head>
<body>
    <div id="app"></div>
    <script src="./out.js"></script>
</body>
</html>
```
