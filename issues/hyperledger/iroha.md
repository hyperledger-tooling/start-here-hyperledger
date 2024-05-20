---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4567" class=".btn">4567</a>
            </td>
            <td>
                <b>
                    Fix `non_local_definitions` warning caused by `derive(displaydoc::Display)`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">good first issue</span>
            </td>
            <td>
                ## Description

There are dozens of warnings like this ([example CI run](https://github.com/hyperledger/iroha/actions/runs/8994520149/job/24708092714?pr=4456)):

```
warning: non-local `impl` definition, they should be avoided as they go against expectation
  --> primitives/numeric/src/lib.rs:65:30
   |
65 | #[derive(Debug, Clone, Copy, displaydoc::Display)]
   |                              ^^^^^^^^^^^^^^^^^^^
   |
   = help: move this `impl` block outside the of the current constant `_DERIVE_Display_FOR_NumericError`
   = note: an `impl` definition is non-local if it is nested inside an item and may impact type checking outside of that item. This can be the case if neither the trait or the self type are at the same nesting level as the `impl`
   = note: one exception to the rule are anon-const (`const _: () = { ... }`) at top-level module and anon-const at the same nesting as the trait or type
   = note: this lint may become deny-by-default in the edition 2024 and higher, see the tracking issue <https://github.com/rust-lang/rust/issues/120363>
   = note: the derive macro `displaydoc::Display` may come from an old version of the `displaydoc` crate, try updating your dependency with `cargo update -p displaydoc`
   = note: `#[warn(non_local_definitions)]` on by default
   = note: this warning originates in the derive macro `displaydoc::Display` (in Nightly builds, run with -Z macro-backtrace for more info)
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-08 01:11:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4511" class=".btn">4511</a>
            </td>
            <td>
                <b>
                    Rename `Upgrade::new` into `Upgrade::executor`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span><span class="chip">api-changes</span>
            </td>
            <td>
                `Upgrade::new` is very vague. Either rename it into `Upgrade::executor` or `UpgradeExecutor::new`.
The assumption here is that there will be other things to upgrade, not only executor. Is this correct?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-25 06:18:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4499" class=".btn">4499</a>
            </td>
            <td>
                <b>
                    Investigate why `actions/setup-python@v5` fails sometimes in `I2::CI::check_for_incorrect_images`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span><span class="chip">CI</span>
            </td>
            <td>
                The `I2::CI::check_for_incorrect_images` job fails sometimes with the following:

```
Error: The version '3.11' with architecture 'x64' was not found for this operating system.
```

[Example log](https://github.com/hyperledger/iroha/actions/runs/8796269117/job/24138820362#step:2:270)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 10:06:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4487" class=".btn">4487</a>
            </td>
            <td>
                <b>
                    Detect color support in `parity_scale_decoder`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span>
            </td>
            <td>
                > Instead of feature-gating it, I would suggest following the same pattern that `iroha` (crate in /cli/) itself follows:
> 
> * It detects colors support automatically via `supports_color` crate
> * User can override it by `--terminal-colors=false`/`--terminal-colors=true` flag

_Originally posted by @0x009922 in https://github.com/hyperledger/iroha/pull/4486#discussion_r1572274579_
            
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-19 13:26:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4301" class=".btn">4301</a>
            </td>
            <td>
                <b>
                    `panic_on_invalid_genesis.sh` is outdated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2-dev</span><span class="chip">config-changes</span><span class="chip">Tests</span>
            </td>
            <td>
                Update this script to use the new config system (#4239):

https://github.com/hyperledger/iroha/blob/964476722e2a219becaacdb3676ca058ec5748cd/scripts/tests/panic_on_invalid_genesis.sh#L4


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 23:34:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4295" class=".btn">4295</a>
            </td>
            <td>
                <b>
                    Implement human-readable bytes in the config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">question</span><span class="chip">iroha2-dev</span><span class="chip">config-changes</span><span class="chip">UI</span>
            </td>
            <td>
                ## Description

Actually implement parsing from a human-readable string for `HumanBytes`:

https://github.com/hyperledger/iroha/blob/964476722e2a219becaacdb3676ca058ec5748cd/config/base/src/lib.rs#L36-L38

### Specification

Here is an excerpt from the config reference draft:

> Bytes amount is specified as a human-readable string:
> 
> ```toml
> # 42 bytes
> value1 = "42B"
> 
> # 1 kilobyte = 1000 bytes
> value2 = "1KB"
> 
> # 1 kilobyte (binary format) = 1024 bytes
> value3 = "1KiB"
> 
> # Sum of multiple
> value4 = "1GB 5MB"
> ```
> 
> Iroha can parse sizes in bytes, kilobytes (`K`), megabytes (`M`), gigabytes (`G`), terabytes (`T`),
> and petabytes (`P`).
> 
> The format of suffixes:
> 
> - **`{size}iB`:** Binary size
> - **`{size}B`:** Decimal size

I used [`humanfriendly`](https://humanfriendly.readthedocs.io/en/latest/api.html?highlight=parse_size#humanfriendly.parse_size) Python package as a reference.

## Also

- [kb, kB, KiB… What’s Up With That? | Pacoup.com](https://web.archive.org/web/20150324153922/https://pacoup.com/2009/05/26/kb-kb-kib-whats-up-with-that/)
- #4294 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 22:54:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4294" class=".btn">4294</a>
            </td>
            <td>
                <b>
                    Implement human-readable durations in the config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">question</span><span class="chip">iroha2-dev</span><span class="chip">config-changes</span><span class="chip">UI</span>
            </td>
            <td>
                ## Description

Enhance `HumanDuration` type to actually parse a human-readable string:

https://github.com/hyperledger/iroha/blob/964476722e2a219becaacdb3676ca058ec5748cd/config/base/src/lib.rs#L23-L27

### Specification

Here is an excerpt from the configuration reference draft:


> Duration is specified as a human-readable string:
> 
> ```toml
> value1 = "1sec"
> value2 = "1hour 12min 5s"
> value3 = "2years 2min 12us"
> value4 = "550ms"
> ```
> 
> The duration string is a concatenation of time spans. Each time span is an
> integer number and a suffix. Supported suffixes:
> 
> - `nsec`, `ns` &mdash; nanoseconds
> - `usec`, `us` &mdash; microseconds
> - `msec`, `ms` &mdash; milliseconds
> - `seconds`, `second`, `sec`, `s`
> - `minutes`, `minute`, `min`, `m`
> - `hours`, `hour`, `hr`, `h`
> - `days`, `day`, `d`
> - `weeks`, `week`, `w`
> - `months`, `month`, `M` &mdash; defined as $30.44$ days
> - `years`, `year`, `y` &mdash; defined as $365.25$ days

I used [`humantime`](https://docs.rs/humantime/latest/humantime/fn.parse_duration.html) crate for reference. Maybe it can be used as is. Otherwise, it is straighforward (and quite interesting!) to write our own parser with something like [`winnow`](https://docs.rs/winnow).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 22:48:51 +0000 UTC
    </div>
</div>

