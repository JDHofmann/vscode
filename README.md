# vscode

.eslintr.js

module.exports = {
  root: true,
  parser: "@typescript-eslint/parser",
  parserOptions: {
    ecmaVersion: 2020,
    sourceType: "module",
    ecmaFeatures: {
      jsx: true,
    },
  },
  settings: {
    react: {
      version: "detect",
    },
  },
  env: {
    browser: true,
    es6: true,
    node: true,
  },
  plugins: ["react", "simple-import-sort"],
  extends: [
    "eslint:recommended",
    "plugin:react/recommended",
    "plugin:jsx-a11y/recommended",
    "plugin:@typescript-eslint/eslint-recommended",
    "plugin:@typescript-eslint/recommended",
    "plugin:prettier/recommended",
  ],
  rules: {
    "prettier/prettier": ["error", {}, { usePrettierrc: true }], // Use our .prettierrc file as source,
    "react/react-in-jsx-scope": "off",
    "react/prop-types": "off",
    "simple-import-sort/imports": "error",
    "@typescript-eslint/explicit-function-return-type": "off",
    "@typescript-eslint/no-explicit-any": "off",
    "react/self-closing-comp": [
      "error",
      {
        component: true,
        html: true,
      },
    ],
    "jsx-a11y/anchor-is-valid": [
      "error",
      {
        components: ["Link"],
        specialLink: ["hrefLeft", "hrefRight"],
        aspects: ["invalidHref", "preferButton"],
      },
    ],
    // Prevents string literals without expressions
    "react/jsx-curly-brace-presence": ["error", "never"],
  },
};

.prettierrc

{
  "endOfLine": "lf",
  "semi": false,
  "singleQuote": true,
  "tabWidth": 4,
  "trailingComma": "es5"
}

settings

{
    "editor.wordWrap": "on",
    "terminal.integrated.env.osx": {
        "PATH": ""
    },
    "files.autoSave": "onWindowChange",
    "indentRainbow.colors": [

        "rgba(255,255,64,0.40)",
        "rgba(127,255,127,0.40)",
        "rgba(255,127,255,0.40)",
        "rgba(79,236,236,0.40)"
    ],
    "workbench.statusBar.visible": true,
    "update.showReleaseNotes": false,
    "workbench.startupEditor": "newUntitledFile",
    "editor.autoClosingQuotes": "always",
    "html.format.indentInnerHtml": true,
    "emmet.excludeLanguages": [

        "markdown"
    ],
    "html.autoClosingTags": false,
    "html.format.contentUnformatted": "",
    "emmet.includeLanguages": {
        "erb": "html"
    },
    "editor.quickSuggestionsDelay": 500,
    "editor.tabCompletion": "on",
    "editor.fontFamily": "Input Sans",
    "editor.fontSize": 14,
    "editor.parameterHints.enabled": false,
    "editor.suggest.showColors": false,
    "terminal.integrated.minimumContrastRatio": 7,
    "editor.minimap.renderCharacters": false,
    "editor.renderWhitespace": "all",
    "breadcrumbs.enabled": true,
    "editor.minimap.enabled": false,
    "editor.renderControlCharacters": false,
    "peacock.favoriteColors": [
 
    
        {
            "name": "Tangerine",
            "value": "#ff9966"
        },
        {
            "name": "Gold",
            "value": "#ffa000"
        },
        {
            "name": "Mandalorian Blue",
            "value": "#1857a4"
        },
        {
            "name": "Green",
            "value": "#317d49"
        },
        {
            "name": "Sky Blue",
            "value": "#00c8ff"
        },
        {
            "name": "Raspberry Pink",
            "value": "#db53aa"
        },
        {
            "name": "Sea Foam",
            "value": "#42b883"
        },
        {
            "name": "Red",
            "value": "#dd0531"
        }
    ],
    "peacock.surpriseMeFromFavoritesOnly": true,
    "liveshare.authenticationProvider": "GitHub",
    "eslint.options": {
        "enable": true
    },
    "workbench.colorTheme": "Monokai",
    "yaml.schemas": {
        "file:///Users/jdbrewer-hofmann/.vscode/extensions/atlassian.atlascode-2.8.5/resources/schemas/pipelines-schema.json": "bitbucket-pipelines.yml"
    },
    "editor.semanticTokenColorCustomizations": null,
    "prettier.htmlWhitespaceSensitivity": "strict",
    "editor.formatOnSave": true,
    "editor.defaultFormatter": "esbenp.prettier-vscode",
    "prettier.semi": false,
    "prettier.requireConfig": true,
    "editor.tabSize": 2,
    "http.proxyAuthorization": null,
    "editor.colorDecorators": false,
    "editor.codeActionsOnSave": null,
}
