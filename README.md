# CNN Birdman

## Getting Started

### 1. Add `cnn-birdman` to your existing project.

```bash
$ npm install -D -E https://github.com/cnnlabs/cnn-birdman.git
```

### 2. Add to your existing npm scripts:
This will automatically lint your src directory, but to choose different directory use -R option.

```diff
"scripts": {
+  "lint": "cnn-birdman [-R <directory>] run [style|javascript]" // optionally pass in specific
}
```
### 3. Add a `.eslintrc` into your project
Currently there are two ESLint configs you can use: `cnn-eslint-base` and `cnn-react`

Determine the directory you would like to lint (typically the root) and add one of
the following as a `.eslintrc` file.

```js
// .eslintrc
{ "extends": "cnn-eslint-base" }
```
```js
// .eslintrc
{ "extends": "cnn-react" }
```

### 4. Run the new script command
```bash
$ npm run lint
```

## TODO
- Document creating nested `.eslintrc` files
- Fix stdio cutoff when errors exceed threshold...?
- Add better error / success messaging