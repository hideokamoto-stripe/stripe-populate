oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g stripe-populate
$ sp COMMAND
running command...
$ sp (--version)
stripe-populate/0.0.0 darwin-x64 node-v14.18.1
$ sp --help [COMMAND]
USAGE
  $ sp COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`sp hello PERSON`](#sp-hello-person)
* [`sp hello world`](#sp-hello-world)
* [`sp help [COMMAND]`](#sp-help-command)
* [`sp plugins`](#sp-plugins)
* [`sp plugins:install PLUGIN...`](#sp-pluginsinstall-plugin)
* [`sp plugins:inspect PLUGIN...`](#sp-pluginsinspect-plugin)
* [`sp plugins:install PLUGIN...`](#sp-pluginsinstall-plugin-1)
* [`sp plugins:link PLUGIN`](#sp-pluginslink-plugin)
* [`sp plugins:uninstall PLUGIN...`](#sp-pluginsuninstall-plugin)
* [`sp plugins:uninstall PLUGIN...`](#sp-pluginsuninstall-plugin-1)
* [`sp plugins:uninstall PLUGIN...`](#sp-pluginsuninstall-plugin-2)
* [`sp plugins update`](#sp-plugins-update)

## `sp hello PERSON`

Say hello

```
USAGE
  $ sp hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Whom is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/hideokamoto-stripe/stripe-populate/blob/v0.0.0/dist/commands/hello/index.ts)_

## `sp hello world`

Say hello world

```
USAGE
  $ sp hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ sp hello world
  hello world! (./src/commands/hello/world.ts)
```

## `sp help [COMMAND]`

Display help for sp.

```
USAGE
  $ sp help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for sp.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.10/src/commands/help.ts)_

## `sp plugins`

List installed plugins.

```
USAGE
  $ sp plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ sp plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.0.11/src/commands/plugins/index.ts)_

## `sp plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ sp plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ sp plugins add

EXAMPLES
  $ sp plugins:install myplugin 

  $ sp plugins:install https://github.com/someuser/someplugin

  $ sp plugins:install someuser/someplugin
```

## `sp plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ sp plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ sp plugins:inspect myplugin
```

## `sp plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ sp plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.

  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.

ALIASES
  $ sp plugins add

EXAMPLES
  $ sp plugins:install myplugin 

  $ sp plugins:install https://github.com/someuser/someplugin

  $ sp plugins:install someuser/someplugin
```

## `sp plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ sp plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.

EXAMPLES
  $ sp plugins:link myplugin
```

## `sp plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ sp plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ sp plugins unlink
  $ sp plugins remove
```

## `sp plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ sp plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ sp plugins unlink
  $ sp plugins remove
```

## `sp plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ sp plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ sp plugins unlink
  $ sp plugins remove
```

## `sp plugins update`

Update installed plugins.

```
USAGE
  $ sp plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
