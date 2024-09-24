# Gostarter

Gostarter is a starter project for my go projects.
It setup a project using [Huma]() framework and [React]() using [vite] for the frontend.
For simplicity sake the React app is embed in the Go binary so it can be all deploy with a single binary.

## Getting Started

1. Install bun: [see bun documentation](https://bun.sh/docs/installation).
2. Install Task: [see Task documentation](https://taskfile.dev/installation/).
3. Run `task dev` at the root to start the project in auto reload mode.
4. (optional) Run `task test` to run tests,linters,formatters accross the project.

## Usage

### Project structure

```
|
|_ cmd/
|____ api/
|______ main.go # Main go file with api code.
|
|_ web/ # React frontend root directory
|____ src/ # Typescript React source code.
|____ web.go # Go file with embed directive to embed the react app.
|
|_ Taskfile.yml # Build tool configuration file where tasks are defined
|
|_ .golangci.yml # Golang linter configuration
```

### Build tools

All available commands can be shown by running `task -l`:

```
task: Available tasks for this project:
* dev:        Run the app with auto reload for development.
* test:       Run linter, formatter and tests.
```
