# Typescript Starter

A bare minimal project that uses Typescript, code linting and styling from Standard, and testing framework from Jest.

### Install

- Node.js is required to install project dependencies. Use the latest version whenever possible.
- Run `npm install` in the root of the project directory to install the dev dependencies.

### Usage

#### `src` folder

Source files including unit tests are in the `src` folder. Feel free to organize the directory layout based on your
requirements.

#### `package.json`

Take a look at `package.json` and make adjustments if necessary. Run `npm update --dry-run` occasionally to check
which dependencies have newer versions.

#### `npm test`

Run `npm test` to pass code lint and style checks, and unit tests.

#### `dist` folder

Run `npx tsc` to compile the Typescript files in the `src` folder and output to the `dist` folder. Javascript files
are not part of the compilation but can be added by modifying `tsconfig.json` with `allowJs` option.

Compilation step can (or should) be added to the `scripts` section of the `package.json` file, deemed appropriate
for the project.

#### `tsconfig.json`

This file is generated from `tsc --init` with defaults. Worth tweaking it as per project requirements.

#### `ts-node`

During development, `ts-node` can be used to execute Typescript files or as a REPL.
See [usage](https://github.com/TypeStrong/ts-node).
