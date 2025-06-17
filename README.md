# ⚛️ React + TypeScript + Vite Template

This template offers a minimal and efficient setup to start building applications using **React**, **TypeScript**, and **Vite**, featuring **Hot Module Replacement (HMR)** and pre-configured **ESLint** rules.

## 🔌 Available Official Plugins

You can choose between the following official plugins for fast refresh support:

- [@vitejs/plugin-react](https://github.com/vitejs/vite-plugin-react/blob/main/packages/plugin-react/README.md) – Uses [Babel](https://babeljs.io/) for Fast Refresh  
- [@vitejs/plugin-react-swc](https://github.com/vitejs/vite-plugin-react-swc) – Uses [SWC](https://swc.rs/) for Fast Refresh

## 🧹 Expanding ESLint Configuration for Production

When building for production, it’s recommended to enable type-aware rules for stricter and more reliable linting.

### ✍️ Update `parserOptions` in your ESLint config:

```js
export default {
  // other rules...
  parserOptions: {
    ecmaVersion: 'latest',
    sourceType: 'module',
    project: ['./tsconfig.json', './tsconfig.node.json'],
    tsconfigRootDir: __dirname,
  },
}
