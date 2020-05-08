# Problem Matcher for markdownlint-cli

[![CI Workflow Status](https://github.com/xt0rted/markdownlint-problem-matcher/workflows/CI/badge.svg)](https://github.com/xt0rted/markdownlint-problem-matcher/actions?query=workflow%3ACI)
[![Dependabot Status](https://api.dependabot.com/badges/status?host=github&repo=xt0rted/markdownlint-problem-matcher)](https://dependabot.com)

Adds a problem matcher that will detect errors from [markdownlint-cli](https://github.com/igorshubovych/markdownlint-cli) and create annotations for them.

**Demo annotations**

Here are some changes to **demo ** the annotations.

***

---

- - -

### Usage

```yml
on: push
jobs:
  build:
    runs-on: ubuntu-latest
    steps:
      - uses: actions/checkout@v2
      - uses: xt0rted/markdownlint-problem-matcher@v1
      - run: markdownlint **/*.md --ignore node_modules
```

## Options

Name | Allowed values | Description
-- | -- | --
`action` | `add` (default), `remove` | If the problem matcher should be registered or removed

## License

The scripts and documentation in this project are released under the [MIT License](LICENSE)
