<!-- tyhp-readme:start -->
# tyhpdef/league-event

Tyhp type definitions for `league/event` `3.0.3`.

```bash
composer require --dev tyhpdef/league-event:3.0.3
```

This is a metapackage. Composer also installs `tyhpdef/league-event-impl` (type files).
Require **this** name, not `tyhpdef/league-event-impl`.

See https://tyhplang.com.

## Maintain `league/event`? Ship the types yourself

If you are a Packagist maintainer of `league/event`, you can take over these
types.

Copy `_tyhpdef/` from **`tyhpdef/league-event-impl`** (Apache-2.0; keep the `NOTICE`).
Then either:

1. **Bundle** the files in `league/event` and set `extra.tyhp.package` on
   that `composer.json`, plus
   `"replace": { "tyhpdef/league-event": "self.version" }`, or
2. **Publish a sibling** types package under your vendor, versioned with
   `league/event` (same `X.Y.Z`). Set `extra.tyhp.package` there,
   `require` `league/event` with a real constraint,
   `"replace": { "tyhpdef/league-event": "self.version" }`, and set
   `extra.tyhp.tyhpdef` on `league/event` to your sibling’s Composer name.

Ship that to Packagist first, then open an issue:

https://github.com/tyhpproject/tyhp-runtime-src/issues/new?template=tyhpdef-ownership.yml

We verify Packagist ownership and that the types parse and cover the PHP
API, then stop publishing community tags for those versions. We do not
transfer the `tyhpdef/league-event` Packagist name.

Full process: `TYHPDEF_OWNERSHIP.md` in
https://github.com/tyhpproject/tyhp-runtime-src
<!-- tyhp-readme:end -->
