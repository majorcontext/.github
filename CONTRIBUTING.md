# Contributing

This is the default contributing guide for a Major Context repository that
has none of its own. If the repository you are changing has its own
`CONTRIBUTING.md`, follow that file instead; it takes precedence over this
one.

## Before you start

Open an issue before you start a large change. Describe the problem and
your proposed approach. This avoids wasted work on a change a maintainer
would not accept.

A small fix, such as a typo or a clear bug, does not need an issue first.

## Making a change

- Keep one change per pull request.
- Link the issue your pull request addresses.
- Run before you open a pull request:

```bash
go build ./...
go vet ./...
go test -race ./...
gofmt -l .
```

`gofmt -l .` must print nothing. Run `gofmt -w .` to fix formatting.

## Commits

Use [Conventional Commit](https://www.conventionalcommits.org/) subjects:
`type(scope): description`. Use a lowercase description and no final
period.

## License

By submitting a contribution, you agree to license it under this project's
MIT license.
