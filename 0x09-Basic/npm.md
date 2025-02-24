# npm
`npm` (Node Package Manager) is the default package manager for Node.js.
## Key Features of npm
- Package Installation – Installs libraries and dependencies easily.

- Version Management – Allows installing specific versions of packages.

- Dependency Management – Maintains a package.json file that records installed dependencies.

- Scripts Execution – Runs custom scripts for automation.

- Global and Local Packages – Supports both project-specific and system-wide installations.

## Installing npm
To install it:

Download and install Node.js from the official Node.js website

Verify installation by running the command below:

```js
npm -v
```
If a version number is returned, it means you have npm installed.

## package.json and package-lock.json

The `package.json` file contains important information about your project including the dependencies/packages your project is using.

When you are using multiple packages in your project, the way you keep track of these packages is by using the `package.json` file.

The `package.json` file is important especially when other developers want to clone your project and know the specific packages that your project is using, they can then use the `package.json` file to install all of them.

## Key elements of package.json file

name: the name of the project.

- version: the version of the project, typically following a semantic versioning.

- description: a brief description of the project.

- main: the entry point of the project.

- dependencies: specifies the libraries and packages required for the project to run.

- devDependencies: specifies libraries and packages needed only for development.

- scripts: defines script commands that can be run on the project.

- author: information about the project author.

e.t.c.
## Creating a `package.json` file

To create a package.json file, on your terminal or command prompt, run the command:
```js
npm init
```
To quickly generate a `package.json` file without providing any information, you can pass the `y` flag:

Once you create the `package.json` file, you can now start installing packages.

When you install a package, npm stores the files and folders for this package in a folder called `node_modules`.

## `package-lock.json`

The `package-lock.json` file ensures consistency in dependency installation by storing detailed information about the exact versions of installed packages, along with their source URLs.

## Installing Packages
There are two ways we can install packages:

- Locally (specific to a project)

- Globally (system-wide)

### Local Installation
To install a package locally, run the npm install command without passing any flags.

```js
npm install package-name
```
### Global Installation
To install a package globally, pass the `--global` or `-g` flag to `npm` install command.

```js
npm install -g package-name
```
### Listing installed packages
To list locally installed packages, run:
```js
npm list
```
To list globally installed packages, pass the -g flag to npm list:
```js
npm list -g
```

### Uninstalling a package
You can uninstall a package using the `npm uninstall` command:
```js
npm uninstall packageName
```
To uninstall a globally installed package, pass the -g flag to the npm uninstall command:
```js
npm uninstall -g packageName
```
### Installing a specific version
You can install a specific version as shown:
```js
npm install packageName@version
```
### Check security vulnerabilities
To check the security vulnerabilities of a package, run:
```js
npm audit packageName
```
## Development vs Regular/Production Dependencies

Regular/Production dependencies are dependencies that the project needs to run.

To install a package as a regular dependency, run `npm install` without passing any options.
```js
npm install packageName
```
## Running Scripts
You can define scripts in `package.json` under `"scripts"` and run them using:
```js
npm run scriptName
```
# Package Versioning and Updates

Packages written by other people are updated by those authors regularly to fix bugs and even introduce new features.

`npm` versions follow a semantic versioning.

Semantic versioning is a system of numbering software versions which each number containing three digits separated by a dot such as 12.17.19

- The first digit represents the major version (12).

- The second digit represents the minor version (17).

- The last digit represents the patch version (19).

Major version is used for changes that are not backward compatible; when changing to this version, we might break things.

Major versions must be incremented if any backward incompatible changes are introduced.

Minor version is used when introducing new features that are backward compatible and won't break anything when we change to that version.

Minor versions must be incremented if new, backward compatible functionality is introduced.

Patch updates are used for updates that contain small bug fixes, and updating won't also break anything.

Patch versions must be incremented if only backward compatible bug fixes are introduced.

When a new version is released, the digits to the right usually reset back to zero. For example, if the current version is 2.34.0 and a major release happens, the new version will be 3.0.0, also when a new minor version is released, the version number changes to 2.35.0























