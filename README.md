[![npm version](https://badge.fury.io/js/%40unitsix%2Feslint-config-essix.svg)](https://badge.fury.io/js/%40unitsix%2Feslint-config-essix)[![Build Status] (https://travis-ci.org/unitsix/npm-eslint-config-essix.svg?branch=master)](https://travis-ci.org/unitsix/npm-eslint-config-essix)

# eslint-config
=========

Based on instructions here: [Shared ESLint config](http://eslint.org/docs/developer-guide/shareable-configs)

Define all of your rules here and just extend this in your project.

## Installation

  `npm install @unitsix/eslint-config-essix`

## Usage

npm install --save-dev eslint-config

Then, extend `@unitsix/eslint-config-essix` in your `.eslintrc`:

```json
{
  "@unitsix/eslint-config-essix"
}
```

## Tests

  N/A

## Deploy

### With Make

  `make publish-patch`
  or
  `make publish-minor`
  or
  `make publish-major`

### Without Make

```
npm version patch -m "Version %s - add sweet badges"
```

**%s** = the new version number.

This command will bump the version number in **package.json**, add a new commit, and tag it with this release number.

**Note**: Your Git working directory has to be **clean** before you can run **npm version**.

After bumping the version number

```
git push && git push --tags (or git push origin master --tags)
npm publish
```
