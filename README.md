# Table of contents

* [Overview](#overview)
* [Usage](#usage)
    * [Broker](#broker)
    * [Debugger](#debugger)

<a name="overview"/>

# Overview

debug-ui

* was created to provide simple UI without dependencies for [debug-broker][debug-broker]
* is an HTML page powered by JavaScript
* can be run by Firefox at localhost
* is hosted by GitHub pages [here][hosted-debug-ui]

<a name="usage"/>

# Usage

Simply open this UI hosted by GitHub pages [here][hosted-debug-ui].

<a name="broker"/>

## Broker

The first time you open UI, you will see an error message like this:

```
ERROR: broker parameter is missing
NOTE: Add 'broker=http://localhost:7999' parameter, where http://localhost:7999 should have DebugBroker instance running
```

You need provide broker URL:

* append `?broker=<url to debug-broker instance>` to your web browser's address bar
* press `Enter` to apply the changes

**Note**:

* consult [debug-broker documentation][debug-broker] to find out how (and where) to install the broker
* `<url to debug-broker instance>` should be a fully qualified URL, even with `http(s)://` part

<a name="debugger"/>

## Debugger

The first time you open UI, you will see an error message like this:

```
ERROR: debugger parameter is missing
NOTE: Add 'debugger=app-title' parameter, where app-title should be Debugger instance name used by app
```

You need to provide debugger name:

* append `&debugger=<app title>` to your web browser's address bar
* press `Enter` to apply the changes

**Note**:

* consult [debug-broker documentation][debug-broker] to find out what debugger name is

[debug-broker]: https://github.com/OGStudio/debug-broker
[hosted-debug-ui]: https://ogstudio.github.io/debug-ui

