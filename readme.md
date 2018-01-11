# Jest Handlebars
This package contains a Jest processor for handlebars files, that compiles the handlebars template and returns the render function.

## Installation
```
npm i jest-handlebars --save-dev
```

To enable the processor please add the following rule to the `transform` object in your jest configuration:

```js
"jest": {
    // ...
    transform: {
        "\\.hbs$": "<rootDir>/tests/jest/hbs-preprocessor.js",
    }
    // ...
}
```

Now all imported handlebars files will get compiled by the processor and the render function is imported.