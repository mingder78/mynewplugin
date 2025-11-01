mynewplugin
=================

A new CLI generated with oclif


[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/mynewplugin.svg)](https://npmjs.org/package/mynewplugin)
[![Downloads/week](https://img.shields.io/npm/dw/mynewplugin.svg)](https://npmjs.org/package/mynewplugin)


<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g @yourorg/mynewplugin
$ mynewplugin COMMAND
running command...
$ mynewplugin (--version)
@yourorg/mynewplugin/0.0.1 darwin-x64 node-v22.16.0
$ mynewplugin --help [COMMAND]
USAGE
  $ mynewplugin COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`mynewplugin hello PERSON`](#mynewplugin-hello-person)
* [`mynewplugin hello world`](#mynewplugin-hello-world)
* [`mynewplugin help [COMMAND]`](#mynewplugin-help-command)
* [`mynewplugin plugins`](#mynewplugin-plugins)
* [`mynewplugin plugins add PLUGIN`](#mynewplugin-plugins-add-plugin)
* [`mynewplugin plugins:inspect PLUGIN...`](#mynewplugin-pluginsinspect-plugin)
* [`mynewplugin plugins install PLUGIN`](#mynewplugin-plugins-install-plugin)
* [`mynewplugin plugins link PATH`](#mynewplugin-plugins-link-path)
* [`mynewplugin plugins remove [PLUGIN]`](#mynewplugin-plugins-remove-plugin)
* [`mynewplugin plugins reset`](#mynewplugin-plugins-reset)
* [`mynewplugin plugins uninstall [PLUGIN]`](#mynewplugin-plugins-uninstall-plugin)
* [`mynewplugin plugins unlink [PLUGIN]`](#mynewplugin-plugins-unlink-plugin)
* [`mynewplugin plugins update`](#mynewplugin-plugins-update)

## `mynewplugin hello PERSON`

Say hello

```
USAGE
  $ mynewplugin hello PERSON -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ mynewplugin hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [src/commands/hello/index.ts](https://github.com/tmp/mynewplugin/blob/v0.0.1/src/commands/hello/index.ts)_

## `mynewplugin hello world`

Say hello world

```
USAGE
  $ mynewplugin hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ mynewplugin hello world
  hello world! (./src/commands/hello/world.ts)
```

_See code: [src/commands/hello/world.ts](https://github.com/tmp/mynewplugin/blob/v0.0.1/src/commands/hello/world.ts)_

## `mynewplugin help [COMMAND]`

Display help for mynewplugin.

```
USAGE
  $ mynewplugin help [COMMAND...] [-n]

ARGUMENTS
  [COMMAND...]  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for mynewplugin.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v6.2.34/src/commands/help.ts)_

## `mynewplugin plugins`

List installed plugins.

```
USAGE
  $ mynewplugin plugins [--json] [--core]

FLAGS
  --core  Show core plugins.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ mynewplugin plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/index.ts)_

## `mynewplugin plugins add PLUGIN`

Installs a plugin into mynewplugin.

```
USAGE
  $ mynewplugin plugins add PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into mynewplugin.

  Uses npm to install plugins.

  Installation of a user-installed plugin will override a core plugin.

  Use the MYNEWPLUGIN_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the MYNEWPLUGIN_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ mynewplugin plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ mynewplugin plugins add myplugin

  Install a plugin from a github url.

    $ mynewplugin plugins add https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ mynewplugin plugins add someuser/someplugin
```

## `mynewplugin plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ mynewplugin plugins inspect PLUGIN...

ARGUMENTS
  PLUGIN...  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ mynewplugin plugins inspect myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/inspect.ts)_

## `mynewplugin plugins install PLUGIN`

Installs a plugin into mynewplugin.

```
USAGE
  $ mynewplugin plugins install PLUGIN... [--json] [-f] [-h] [-s | -v]

ARGUMENTS
  PLUGIN...  Plugin to install.

FLAGS
  -f, --force    Force npm to fetch remote resources even if a local copy exists on disk.
  -h, --help     Show CLI help.
  -s, --silent   Silences npm output.
  -v, --verbose  Show verbose npm output.

GLOBAL FLAGS
  --json  Format output as json.

DESCRIPTION
  Installs a plugin into mynewplugin.

  Uses npm to install plugins.

  Installation of a user-installed plugin will override a core plugin.

  Use the MYNEWPLUGIN_NPM_LOG_LEVEL environment variable to set the npm loglevel.
  Use the MYNEWPLUGIN_NPM_REGISTRY environment variable to set the npm registry.

ALIASES
  $ mynewplugin plugins add

EXAMPLES
  Install a plugin from npm registry.

    $ mynewplugin plugins install myplugin

  Install a plugin from a github url.

    $ mynewplugin plugins install https://github.com/someuser/someplugin

  Install a plugin from a github slug.

    $ mynewplugin plugins install someuser/someplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/install.ts)_

## `mynewplugin plugins link PATH`

Links a plugin into the CLI for development.

```
USAGE
  $ mynewplugin plugins link PATH [-h] [--install] [-v]

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help          Show CLI help.
  -v, --verbose
      --[no-]install  Install dependencies after linking the plugin.

DESCRIPTION
  Links a plugin into the CLI for development.

  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ mynewplugin plugins link myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/link.ts)_

## `mynewplugin plugins remove [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ mynewplugin plugins remove [PLUGIN...] [-h] [-v]

ARGUMENTS
  [PLUGIN...]  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ mynewplugin plugins unlink
  $ mynewplugin plugins remove

EXAMPLES
  $ mynewplugin plugins remove myplugin
```

## `mynewplugin plugins reset`

Remove all user-installed and linked plugins.

```
USAGE
  $ mynewplugin plugins reset [--hard] [--reinstall]

FLAGS
  --hard       Delete node_modules and package manager related files in addition to uninstalling plugins.
  --reinstall  Reinstall all plugins after uninstalling.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/reset.ts)_

## `mynewplugin plugins uninstall [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ mynewplugin plugins uninstall [PLUGIN...] [-h] [-v]

ARGUMENTS
  [PLUGIN...]  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ mynewplugin plugins unlink
  $ mynewplugin plugins remove

EXAMPLES
  $ mynewplugin plugins uninstall myplugin
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/uninstall.ts)_

## `mynewplugin plugins unlink [PLUGIN]`

Removes a plugin from the CLI.

```
USAGE
  $ mynewplugin plugins unlink [PLUGIN...] [-h] [-v]

ARGUMENTS
  [PLUGIN...]  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ mynewplugin plugins unlink
  $ mynewplugin plugins remove

EXAMPLES
  $ mynewplugin plugins unlink myplugin
```

## `mynewplugin plugins update`

Update installed plugins.

```
USAGE
  $ mynewplugin plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v5.4.52/src/commands/plugins/update.ts)_
<!-- commandsstop -->
