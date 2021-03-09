# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## ESLingt Configuration

1.) Remove pre-set ESlint configuration
2.) yarn add eslint -D
3.) npx eslint —init
4.) add plugins: yarn add [ ] -D
@typescript-eslint/eslint-plugin           
@typescript-eslint/parser
eslint-config-airbnb
eslint-plugin-import
eslint-plugin-jsx-a11y
eslint-plugin-react
eslint-plugin-react-hooks
5.) edit .eslintrc.json
Add this rule: "rules": {
"no-use-before-define": "off",
"@typescript-eslint/no-use-before-define": ["error"]
},
"react/jsx-filename-extension": [ "warn", {"extensions": [".tsx”]},]
6.) yarn add eslint-import-resolver-typescript -D
7.) add to .eslintrcjson
    "settings": {
        "import/resolver": {
            "typescript": {}
        }
8.) in rules  add to .eslintrcjson:
    "import/extensions": [
            "error",
            "ignorePackages",
            {
                "ts": "never",
                "tsx": "never"
            }
        ]
9.) extends: "plugin:@typescript-eslint/recommended"
10.)rules:    "no-shadow": "off",
        "@typescript-eslint/no-shadow": ["error"]
11.) rules: "@typescript-eslint/explicit-function-return-type": [
"error",
{
"allowExpressions": true
}
]
12.) "plugins": [
…
"react-hooks"
],
13.) "rules":{
…
"react-hooks/rules-of-hooks": "error",
"react-hooks/exhaustive-deps": "warn"
}
14.) "rules":{
…
"import/prefer-default-export": "off"
}
15.)
"rules":{
…
"react/prop-types": "off"
}


In the project directory, you can run:

### `yarn start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in the browser.

The page will reload if you make edits.\
You will also see any lint errors in the console.

### `yarn test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `yarn build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `yarn eject`

**Note: this is a one-way operation. Once you `eject`, you can’t go back!**

If you aren’t satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you’re on your own.

You don’t have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn’t feel obligated to use this feature. However we understand that this tool wouldn’t be useful if you couldn’t customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).
