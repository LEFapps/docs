# Docs for LEFapps development team

_Please run `npm run build` before pushing to GitHub._

## Table of contents

-   [Packages](#packages)

    -   [Overview](#overview)
    -   [Development](#development)

## Packages

### Overview

| npm                                                              | meteor                                                            | meteor wraps npm? | should switch to npm |
| ---------------------------------------------------------------- | ----------------------------------------------------------------- | ----------------- | -------------------- |
| [@lefapps/translations](https://github.com/LEFapps/translations) | [lef:translations](https://github.com/LEFapps/lef-translations)   | ✓                 |                      |
| [@lefapps/forms](https://github.com/LEFapps/forms)               | [lef:forms2](https://github.com/LEFapps/lef-forms2)               | ✓                 |                      |
|                                                                  | [lef:adminlist](https://github.com/LEFapps/lef-adminlist)         |                   | ?                    |
|                                                                  | [lef:imgupload](https://github.com/LEFapps/lef-imgupload)         |                   | ?                    |
|                                                                  | [lef:userui](https://github.com/LEFapps/lef-userui)               |                   |                      |
| [react-alert](https://www.npmjs.com/package/react-alert)         | [lef:alerts](https://github.com/LEFapps/lef-alerts)               |                   |                      |
|                                                                  | [lef:systemmailing](https://github.com/LEFapps/lef-systemmailing) |                   | ✓                    |
|                                                                  | [lef:cms](https://github.com/LEFapps/lef-cms)                     |                   | ✓                    |
|                                                                  | [lef:guard](https://github.com/LEFapps/lef-guard)                 |                   | ✓                    |
|                                                                  | [lef:utils](https://github.com/LEFapps/lef-utils)                 |                   | ✓                    |

### Development

Follow these steps to write new packages:

1.  Create a new npm package
    ```sh
    git clone git@github.com:LEFapps/npm-package-boilerplate.git
    mv npm-package-boilerplate yournewpackage
    cd yournewpackage
    rm -rf .git
    git init
    ```

2.  Push to new GitHub repository at [LEFapps](https://github.com/LEFapps/)

3.  Publish to npm `npm publish --access public` :rocket: 

4.  OPTIONALLY. Write a Meteor wrapper package.

Only in rare cases would you only write a Meteor package.
