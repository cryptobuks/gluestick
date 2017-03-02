# `gluestick-cli`
Gluestick CLI is an command line interface for `gluestick` package. It exposes few commands from your global packages, and proxies rest of them to your [local distribution of gluestick](../packages/gluestick).

## Exposed commands

### `gluestick new`

Takes care of generating new project

```bash
gluestick new <YOUR_APPLICATION_NAME>
```

Available options:

* `-d, --dev <path>` - Relative path to development version of gluestick
* `-y, --yarn` - Use yarn to perform installations (not working yet, see [#528](https://github.com/TrueCar/gluestick/issues/528))

### `gluestick reinstall-dev`

Reinstall gluestick dependency project

```bash
gluestick reinstall-dev
```

### `gluestick watch`

Watches and applies changes from gluestick package to current project

```bash
gluestick watch
```

### `gluestick reset-hard`

Removes gluestick dependency project clean build, cache and reinstalls dependencies

```bash
gluestick reset-hard
```