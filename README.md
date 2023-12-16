# React + TypeScript + Vite

This template provides a minimal setup to get React working in Vite with HMR and some ESLint rules.

Currently, two official plugins are available:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) uses [Babel](https://babeljs.io/) for Fast Refresh
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) uses [SWC](https://swc.rs/) for Fast Refresh

## Expanding the ESLint configuration

If you are developing a production application, we recommend updating the configuration to enable type aware lint rules:

- Configure the top-level `parserOptions` property like this:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: "latest",
    sourceType: "module",
    project: ["./tsconfig.json", "./tsconfig.node.json"],
    tsconfigRootDir: __dirname,
  },
};
```

- Replace `plugin:@typescript-eslint/recommended` to `plugin:@typescript-eslint/recommended-type-checked` or `plugin:@typescript-eslint/strict-type-checked`
- Optionally add `plugin:@typescript-eslint/stylistic-type-checked`
- Install [eslint-plugin-react](https://github.com/jsx-eslint/eslint-plugin-react) and add `plugin:react/recommended` & `plugin:react/jsx-runtime` to the `extends` list

---

### folder structure:

#### assets

for public and static files use in project like:
fonts, svg files, images file for include in project

#### components

usual for global component for usage on all pages, usually create with multiple micro component or ui kit

#### config

here some files for configuration app like:
constant, http-service(axios instance), web-engage, ...

#### hooks

for react js hooks

#### i18n

for locale file, also files can in public path

#### pages

per page need folder, you can implant files like this example:

login //folder name is kebab-case
Login.tsx
login.api.ts
login.styles.ts or .scss
login.types.ts // for store all typescript types for Login
login.constant.ts // for constant file only use in Login
components // for components only use in Login

#### redux/storage

for state management files like reducer

#### router

for store files and router providers

#### theme

for config theme file and ui components about

#### types

store for global types, you can store in separated files

#### ui-kit

this folder can handle ui-kit components

#### utils

for helper or utils files

#### public

#### services

you can add http request's file here or handle on per component or page

#### story book
