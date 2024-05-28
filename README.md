[![REUSE status](https://api.reuse.software/badge/github.com/cap-js/cds-plugin-for-ord)](https://api.reuse.software/info/github.com/cap-js/cds-plugin-for-ord)

# CDS Plugin for ORD

## About this project

Enables generation of ORD document for CAP based applications.

## Requirements and Setup

### Installation

```sh
$ npm install @cap-js/ord
```

### Usage

There are multiple ways to view the ORD Document by using this plugin.

#### Programmatic API

```js
const cds = require('@sap/cds')
```

```js
const csn = await cds.load(cds.env.folders.srv)
const ord = cds.compile.to.ord(csn)
```

#### Command Line

```sh
$ cds compile <filePath to srv folder of CAP App> -2 ord [-o] [destinationFilePath]
```

#### ORD Endpoints 

1) Run a `cds watch` in the application's root path.
2) Check the following relative paths for ORD information - `/.well-known/open-resource-discovery` , `/open-resource-discovery/v1/documents/1`.


## Support, Feedback, Contributing

This project is open to feature requests/suggestions, bug reports etc. via [GitHub issues](https://github.com/cap-js/ord/issues). Contribution and feedback are encouraged and always welcome. For more information about how to contribute, the project structure, as well as additional contribution information, see our [Contribution Guidelines](CONTRIBUTING.md).

## Security / Disclosure
If you find any bug that may be a security problem, please follow our instructions at [in our security policy](https://github.com/cap-js/ord/issues/security/policy) on how to report it. Please do not create GitHub issues for security-related doubts or problems.

## Code of Conduct

We as members, contributors, and leaders pledge to make participation in our community a harassment-free experience for everyone. By participating in this project, you agree to abide by its [Code of Conduct](https://github.com/cap-js/.github/blob/main/CODE_OF_CONDUCT.md) at all times.

## Licensing

Copyright 2024 SAP SE or an SAP affiliate company and cds-plugin-for-ord contributors. Please see our [LICENSE](LICENSE) for copyright and license information. Detailed information including third-party components and their licensing/copyright information is available [via the REUSE tool](https://api.reuse.software/info/github.com/cap-js/<your-project>).