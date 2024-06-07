# bun-scoped-pkg-patch-bug

Reproduction:

- Clone this repo
- Run `bun install` (ensure you're using a version of bun with `bun patch`, you can do `bun upgrade --canary` to get the latest version)
- Run `bun patch @contentlayer/cli`
- See error below:

```sh
bun patch @contentlayer/cli@0.3.4
[0.49ms] ".env"
bun patch v1.1.13-canary.1 (386bc212)

[477.00ms] done

error: could not find package: @contentlayer/cli@0.3.4
```