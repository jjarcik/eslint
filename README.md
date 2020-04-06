# Perfect ESLint config
```
yarn add eslint-plugin-jsx-a11y -D
yarn add eslint-plugin-flowtype -D 
yarn add eslint-plugin-import -D
yarn add eslint-plugin-jsx-control-statements -D
yarn add eslint-config-react-app -D
```

```JavaScript
module.exports = {
  extends: ['react-app', 'plugin:jsx-control-statements/recommended'],
  "parser": "babel-eslint",
  rules: {
    'react/jsx-uses-vars': 1,
    'react/react-in-jsx-scope': 1,
    'react/jsx-uses-react': 'error',
    'comma-dangle': ['error', 'only-multiline'],
    'space-before-function-paren': 0,
    eqeqeq: 'warn',
    semi: ['error', 'never'],
    indent: ['error', 2],
    'default-case': [0],
    'react-hooks/exhaustive-deps': [0],
    'jsx-quotes': ['error', 'prefer-double'],
    'comma-dangle': ['error', {
      'arrays': 'always-multiline',
      'objects': 'always-multiline',
      'imports': 'always-multiline',
      'exports': 'always-multiline',
      'functions': 'always-multiline'
    }],
    'react/jsx-no-undef': [2, { 'allowGlobals': true }]
  },
  'plugins': [
    'jsx-control-statements',
  ]
}
```

## ESLint config with flow-types
```JavaScript
module.exports = {
  extends: ['react-app', 'plugin:jsx-control-statements/recommended', 'plugin:flowtype/recommended'],
  "parser": "babel-eslint",
  rules: {
    'react/jsx-uses-vars': 1,
    'react/react-in-jsx-scope': 1,
    'react/jsx-uses-react': 'error',
    'comma-dangle': ['error', 'only-multiline'],
    'space-before-function-paren': 0,
    eqeqeq: 'warn',
    semi: ['error', 'never'],
    indent: ['error', 2],
    'default-case': [0],
    'react-hooks/exhaustive-deps': [0],
    'jsx-quotes': ['error', 'prefer-double'],
    'comma-dangle': ['error', {
      'arrays': 'always-multiline',
      'objects': 'always-multiline',
      'imports': 'always-multiline',
      'exports': 'always-multiline',
      'functions': 'always-multiline'
    }],
    'react/jsx-no-undef': [2, { 'allowGlobals': true }]
  },
  'plugins': [
    'jsx-control-statements',
    'flowtype'
  ],
  "settings": {
    "flowtype": {
      "onlyFilesWithFlowAnnotation": true
    }
  },
  "rules": {
    "flowtype/boolean-style": [
      2,
      "boolean"
    ],
    "flowtype/define-flow-type": 1,
    "flowtype/delimiter-dangle": [
      2,
      "never"
    ],
    "flowtype/generic-spacing": [
      2,
      "never"
    ],
    "flowtype/no-mixed": 2,
    "flowtype/no-primitive-constructor-types": 2,
    "flowtype/no-types-missing-file-annotation": 2,
    "flowtype/no-weak-types": 2,
    "flowtype/object-type-delimiter": [
      2,
      "comma"
    ],
    "flowtype/require-parameter-type": 2,
    "flowtype/require-readonly-react-props": 0,
    "flowtype/require-return-type": [
      2,
      "always",
      {
        "annotateUndefined": "never"
      }
    ],
    "flowtype/require-valid-file-annotation": 2,
    "flowtype/semi": [
      2,
      "always"
    ],
    "flowtype/space-after-type-colon": [
      2,
      "always"
    ],
    "flowtype/space-before-generic-bracket": [
      2,
      "never"
    ],
    "flowtype/space-before-type-colon": [
      2,
      "never"
    ],
    "flowtype/type-id-match": [
      2,
      "^([A-Z][a-z0-9]+)+Type$"
    ],
    "flowtype/union-intersection-spacing": [
      2,
      "always"
    ],
    "flowtype/use-flow-type": 1,
    "flowtype/valid-syntax": 1
  },
  
}
```
