### Absurldy simple MicroFrontEnd using Rspack

Just something I threw together quickly, I'll add more to this as I dig in more.

## To Install:

1. Git clone the repo
2. npm install host
3. npm install remote
4. You should see something on `http://localhost:8080/`

## To Use:

1. Go to remote and create a component
2. Add component to `rspack.config.js`. Look for `ModuleFederationPlugin`
3. See below

```javascript
      exposes: {
        "./MyComponentName": "./src/MyComponentName",
      },
```

4. Go to host folder
5. Open `App.jsx`, or whichever component you want to import to.
6. Import `MyComponentName`, like you would any react component.
