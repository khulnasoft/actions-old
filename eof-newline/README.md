# EOF newline

This action flags files that are missing newlines at the end of the file.

This code is also derived from a similar check originally contributed to
Knative.

## Usage

```yaml
- uses: khulnasoft/actions/eof-newline@main
  with:
    # Set when checkout to a non-default path.
    path: ""
```

## Scenarios

```yaml
steps:
  - uses: actions/checkout@v3
  - uses: khulnasoft/actions/eof-newline@main
    with:
      path: "src/github.com/${{ github.repository }}"
```