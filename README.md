# `@inovando/cra-template`
> ⚡️ Inovando's template for create-react-app

[![NPM version](https://img.shields.io/npm/v/@inovando/cra-template.svg)](https://www.npmjs.com/package/@inovando/cra-template)
[![code style: prettier](https://img.shields.io/badge/code_style-prettier-ff69b4.svg)](https://github.com/prettier/prettier)
[![Commitizen friendly](https://img.shields.io/badge/commitizen-friendly-brightgreen.svg)](http://commitizen.github.io/cz-cli/)


![Package Main Techs](docs/techs.png)

## Preview

|   Desktop   |  Mobile  |
|---------|-----------|
| ![Template Chrome Desktop Preview](docs/preview-desktop.gif) | ![Template Mobile Preview](docs/preview-mobile.gif) |


## Usage

1. Initialize your project with this command:

```
npx create-react-app my-app --template @inovando
```

2. Duplicate `.env.example` to `.env.development.local` and `.env.production` fulfilling variables as needed

3. Run the following commands:

```bash
yarn start # React server
yarn mock # Mock server (to see table example)
```

4. Done 🎉

5. (Optional) If you need PWA, don't forget to change icons at `public/site.webmanifest`

6. (Optional) If your project will use Cypress and your OS is Linux Ubuntu/Debian, you need to run the following commands:

```bash
sudo apt-get install libgtk2.0-0 libgtk-3-0 libgbm-dev libnotify-dev libgconf-2-4 libnss3 libxss1 libasound2 libxtst6 xauth xvfb
```

7. (Optional) Duplicate `cypress.env.example.json` to `cypress.env.json` fulfilling variables as needed

## Scripts

### `yarn serve`

Serve app based on `build/` folder (generated by `yarn build`)

### `yarn build-and-serve`

Build and serve `build/` folder

### `yarn generate:crud`

Will prompt some questions to create a new CRUD with 3 routes (/entity, /entity/new, /entity/:id)

### `yarn generate:crud-modal`

Will prompt some questions to create a new CRUD based on a modal with 1 route (/entity)

## Features
- [x] [ESLint](https://github.com/santospatrick/eslint-config-react)/[Prettier](https://github.com/santospatrick/prettier-config)
- [x] [Axios](https://www.npmjs.com/package/axios)
- [x] [Styled Components](https://styled-components.com/)
- [x] [React Final Form](https://final-form.org/react)
- [x] [Yup](https://runkit.com/jquense/yup)
- [x] [Husky](https://github.com/typicode/husky)/[Lint Staged](https://github.com/okonet/lint-staged)
- [x] [Material UI](https://material-ui.com/)
- [x] [React Router](https://reacttraining.com/react-router/web/guides/quick-start)
- [x] [React Toastify](https://github.com/fkhadra/react-toastify)
- [x] CRUD Example
- [x] Commitizen Friendly
- [x] [Generate Code from CLI](http://hygen.io/)
- [x] [Code Splitting](https://reactjs.org/docs/code-splitting.html#route-based-code-splitting)
- [x] [Sentry](https://sentry.io/)
- [x] [PWA Ready](https://web.dev/progressive-web-apps/) (All required variations can be [generated with Real Favicon Generator](https://realfavicongenerator.net/))
- [x] [date-fns](https://date-fns.org/)
- [x] [Numeral.js](http://numeraljs.com/)
- [x] [JS Brasil](https://geradorbrasileiro.com)
- [x] [Cypress](https://www.cypress.io/)
- [ ] [SWR](https://swr.vercel.app/)

## FAQ

### Why ESLint and plugins are dependencies?

Until the release date of this package, create react app [does not support devDependencies](https://github.com/facebook/create-react-app/issues/8082) field at `template.json`

### Git hooks not working

```
rm -rf node_modules && yarn
```
