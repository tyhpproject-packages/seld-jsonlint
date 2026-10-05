<!-- tyhp-readme:start -->
# tyhpdef/seld-jsonlint

Tyhp type definitions for `seld/jsonlint` `1.12.1`.

```bash
composer require --dev tyhpdef/seld-jsonlint:1.12.1
```

This is a metapackage. Composer also installs `tyhpdef/seld-jsonlint-impl` (type files).
Require **this** name, not `tyhpdef/seld-jsonlint-impl`.

See https://tyhplang.com.

## Maintain `seld/jsonlint`? Ship the types yourself

If you are a Packagist maintainer of `seld/jsonlint`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/seld-jsonlint-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `seld/jsonlint` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/seld-jsonlint": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `seld/jsonlint` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `seld/jsonlint` with a real constraint,
   `"replace": { "tyhpdef/seld-jsonlint": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `seld/jsonlint` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/seld-jsonlint` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
