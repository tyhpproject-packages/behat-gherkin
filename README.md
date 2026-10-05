<!-- tyhp-readme:start -->
# tyhpdef/behat-gherkin

Tyhp type definitions for `behat/gherkin` `4.17.0`.

```bash
composer require --dev tyhpdef/behat-gherkin:4.17.0
```

This is a metapackage. Composer also installs `tyhpdef/behat-gherkin-impl` (type files).
Require **this** name, not `tyhpdef/behat-gherkin-impl`.

See https://tyhplang.com.

## Maintain `behat/gherkin`? Ship the types yourself

If you are a Packagist maintainer of `behat/gherkin`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/behat-gherkin-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `behat/gherkin` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/behat-gherkin": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `behat/gherkin` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `behat/gherkin` with a real constraint,
   `"replace": { "tyhpdef/behat-gherkin": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `behat/gherkin` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/behat-gherkin` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
