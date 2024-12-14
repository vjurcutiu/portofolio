# Trading Bot Frontend

This project is the frontend application for a trading bot, built using Vue.js and Webpack. It provides a user interface for interacting with the trading bot, displaying data, and managing trading operations.

## Table of Contents
- [Installation](#installation)
- [Development](#development)
- [Build](#build)
- [Project Structure](#project-structure)
- [Key Components](#key-components)
- [Configuration](#configuration)
- [License](#license)

## Installation
To install the project dependencies, run the following command:

```bash
npm install
```

## Development
To start the development server, run the following command:

```bash
npm run dev
```

This will start the Webpack development server on port `5550` with hot module replacement enabled.

## Build
To build the project for production, run the following command:

```bash
npm run build
```

This will create a production-ready build in the `dist` directory.

## Project Structure
The project structure is as follows:
```
src/
├── components/         # Reusable Vue components
├── router/             # Router configuration
├── store/              # Vuex store setup
├── assets/             # Static assets (images, styles, etc.)
├── locale/             # Localization files
├── libs/               # Utility functions
├── App.vue             # Root Vue component
└── main.js             # Application entry point
webpack/
├── webpack.base.config.js     # Base Webpack configuration
├── webpack.dev.config.js      # Development Webpack configuration
└── webpack.prod.config.js     # Production Webpack configuration
```

## Key Components

### Webpack Configuration
- **Base Configuration**: `webpack.base.config.js`
- **Development Configuration**: `webpack.dev.config.js`
- **Production Configuration**: `webpack.prod.config.js`

### Vue.js Application
- **Entry Point**: `main.js`
- **Root Component**: `App.vue`
- **Router Configuration**: `router/index.js`
- **Vuex Store**: `store/index.js`
- **Localization**: `locale/index.js`
- **Utility Functions**: `libs/util.js`

### Loaders and Plugins
- **CSS and Less**:
  - The project uses `css-loader`, `autoprefixer-loader`, and `less-loader` for handling CSS and Less files.
- **File Handling**:
  - The project uses `url-loader` for handling image and font files.
  - It uses `html-loader` for handling HTML and template files.
- **Plugins**:
  - `ExtractTextPlugin` for extracting CSS into separate files.
  - `HtmlWebpackPlugin` for generating HTML files.
  - `CommonsChunkPlugin` for optimizing common chunks.

## Configuration
The project uses environment-specific configurations for development and production. The environment is set in the `env.js` file, which is generated during the build process.

## License
This project is licensed under the MIT License. For more details, see the `LICENSE` file.
