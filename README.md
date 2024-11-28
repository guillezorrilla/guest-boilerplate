## Requirements

- [React Native dev environment ](https://reactnative.dev/docs/environment-setup)
- [Node.js LTS release](https://nodejs.org/en/)
- [Git](https://git-scm.com/)
- [Watchman](https://facebook.github.io/watchman/docs/install#buildinstall), required only for macOS or Linux users
- [Pnpm](https://pnpm.io/installation)
- [VS Code Editor](https://code.visualstudio.com/download) ⚠️ Make sure to install all recommended extension from `.vscode/extensions.json`

## 👋 Quick start

Clone the repo to your machine and install deps :

```sh
git clone https://github.com/user/repo-name

cd ./repo-name

pnpm install
```

To run the app on ios

```sh
pnpm ios
```

To run the app on Android

```sh
pnpm android
```

## Monorepo or npm package (due to react native dependencies)

- Api Layer
  - DTO
  - Endpoints
- Service Layer (map from API to Domain)
  - Mappers (API to Domain)
  - Models
- Presenters
  - Get Order
  - Get locations

## App Layer

- No interactors
- Own Redux Store
- Selectors
- Presenters
  - Responsable to save datain redux or context or zustand or whatever

# Changes to this project

- Change tailwind config to use css variables and inject them in the app rather than having static values for colors and theming, that includes add css variables into global.css
- Change project to use vitest rather than jest
- Add react testing library
- Use screaming architecture inside of the app folder
- Get rid of expo and change to react native cli and react navigation
- See how to make different configurations for each app in terms of the app.config (expo especific) and the tailwind css variables, maybe a configuration.json file that we fetch and inject into the app
- Simple action
  - Get locations from user
  - App token, we can inject that here for now
