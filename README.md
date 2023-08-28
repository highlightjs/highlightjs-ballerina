![](./ballerina-swan-lake-logo.svg)

# The Ballerina programming language

[![GitHub (pre-)release](https://img.shields.io/github/release/ballerina-platform/ballerina-lang/all.svg)](https://github.com/ballerina-platform/ballerina-lang/releases)
[![GitHub (Pre-)Release Date](https://img.shields.io/github/release-date-pre/ballerina-platform/ballerina-lang.svg)](https://github.com/ballerina-platform/ballerina-lang/releases)
[![GitHub last commit](https://img.shields.io/github/last-commit/ballerina-platform/ballerina-lang.svg)](https://github.com/ballerina-platform/ballerina-lang/commits/master)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)
![Twitter Follow](https://img.shields.io/twitter/follow/ballerinalang?style=social)

[Ballerina](https://ballerina.io/) is a statically typed, open-source cloud-native programming language developed
and supported by [WSO2](https://wso2.com/).

With Ballerina, you could easily develop microservices, API endpoints and integrations,
and any other application for the cloud. Additionally, Ballerina has all the general-purpose
functionalities you could expect from a modern programming language.

With Ballerina's compiler-level built-in support for widely used data types such
as JSON and XML, your focus on handling structured data, network service interactions,
and dealing with concurrency is made much more effective.

#### Providing and consuming services
It has inherently concurrent first-class language constructs for providing and consuming services.

#### Sequence diagrams
Sequence diagram based graphical view shows the most fundamental aspect of the semantics of a network distributed application.

#### Structural typing
It allows for looser coupling between distributed components and eliminates the friction of data binding.

#### Metadata
Extensible metadata enables easy integration of Ballerina programs with cloud platforms.
You could directly generate Docker and Kubernetes artifacts straight away from
the source code.

# highlightjs-ballerina

This repository offers `highlight.js` support for [Ballerina](https://ballerina.io).

## Usage

The first step in setting up syntax highlighting for Ballerina is to setup `highlight.js` library in your webpage or the node app.

### Static website or simple usage

After loading `highlight.js`, load the CDN build of Ballerina located in the `dist` folder.

```html
<!-- stylesheet -->
<link rel="stylesheet" href="https://unpkg.com/highlightjs/styles/vs.css" />

<!-- scripts -->
<script type="text/javascript" src="/path/to/highlight.min.js"></script>
<script type="text/javascript" src="/path/to/ballerina.min.js"></script>
<script type="text/javascript">
	hljs.highlightAll();
</script>
```

### With node or another build system

If you're using Node / Webpack / Rollup / Browserify, etc, simply require the language module, then register it with Highlight.js.

```js
var hljs = require('highlightjs');
var hljsBallerina = require('@ballerina/highlightjs-ballerina');

hljs.registerLanguage('ballerina', hljsBallerina);
hljs.highlightAll();
```

## License

Ballerina code is distributed under [Apache license 2.0](https://github.com/ballerina-platform/ballerina-lang/blob/master/LICENSE).

## Author



## Links

- The official site for the Highlight.js library is <https://highlightjs.org/>.
- The Highlight.js GitHub project: <https://github.com/highlightjs/highlight.js>