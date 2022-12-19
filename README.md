# Typescript Starter

A bare minimal project that uses Typescript, code linting and styling from Standard, and testing framework from Jest.

### Install

- Node.js is required to install project dependencies. Use the latest version whenever possible.
- Run `npm ci` in the root of the project directory to install all dependencies.

### Usage

#### `src` folder

Source files including unit tests are in the `src` folder. Feel free to organize the directory layout based on your
requirements.

#### `package.json`

Inspect file `package.json` and make any necessary adjustments. Run `npm outdated` occasionally to check which
dependencies have newer versions.

#### `npm run lint`

Uses `ts-standard` to run code lint and style checks.

#### `npm run compile`

Uses `tsc` to compile all Typescript files in the `src` folder and output to the `dist` folder. Javascript files are
not part of the compilation but can be added by modifying `tsconfig.json` with `allowJs` option.

#### `npm test`

Uses Jest to run unit tests. By default, files ending in .test.ts or .test.js are tested. Modify `jest.config.js` to
configure Jest.

#### `npm run build`

Runs these scripts in sequential order: `lint`, `compile`, `test`. This will ensure that your code passes lint and
style checks, compiles successfully, and passes all unit tests.

#### `tsconfig.json`

This file is generated from `tsc --init` with defaults. Worth tweaking it as per project requirements.

#### `ts-node`

During development, `ts-node` can be used to execute Typescript files or as a REPL.
See [usage](https://github.com/TypeStrong/ts-node).
