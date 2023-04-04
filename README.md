# goyek - using Go for automation

[Presentation](https://docs.google.com/presentation/d/1AQt-a_b4MR3gty-_aZw08bXX708KTQBu9inSncoydyk/edit?usp=sharing).

This repository demonstrates a very basic build automation for a Go project created in:

- **[Make](./make)**
- **[Mage](./mage)**
- **[goyek](./goyek)**

## Build Workflow

The build workflow, called `all`, consists of the following steps:

### `fmt`

Simply runs `go fmt ./...`.

This target is imported as it can be reused by multiple projects.

### `test`

Runs tests and generates code coverage even if any test fails.
