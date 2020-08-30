# eslint-config-typed-fp

An opinionated ESLint config to encourage pure(ish), typeful functional programming in TypeScript.

## Installation

```sh
yarn add --dev eslint-config-typed-fp @typescript-eslint/eslint-plugin @typescript-eslint/parser eslint eslint-plugin-functional eslint-plugin-total-functions typescript
```

## Usage

Update your `.eslintrc.js`:

```diff
module.exports = {
+  parser: "@typescript-eslint/parser",
  parserOptions: {
+    project: "./tsconfig.json",
+    ecmaVersion: 2018,
+    sourceType: "module"
  },
  extends: [
+  "typed-fp",
  ...
  ],
  plugins: [
+  "@typescript-eslint",
+  "functional",
+  "total-functions",
  ...
],
  rules: {
    ...
  }
};

```

## What's in the box?

See the `extends` and `rules` sections in [index.ts](https://github.com/danielnixon/eslint-config-typed-fp/blob/master/src/index.ts).