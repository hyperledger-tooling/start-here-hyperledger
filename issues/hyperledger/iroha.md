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
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">config-changes</span><span class="chip">Tests</span>
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
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">question</span><span class="chip">iroha2</span><span class="chip">config-changes</span><span class="chip">UI</span>
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
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">question</span><span class="chip">iroha2</span><span class="chip">config-changes</span><span class="chip">UI</span>
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

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4291" class=".btn">4291</a>
            </td>
            <td>
                <b>
                    [suggestion] Update executor config in the genesis block
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">config-changes</span>
            </td>
            <td>
                ## Description

> TL;DR: drop inline executor support; rename field to `executor_file`.

Genesis block contains `executor` field, which might either represent an inline base64-encoded WASM blob, or a file path to the WASM blob:

https://github.com/hyperledger/iroha/blob/964476722e2a219becaacdb3676ca058ec5748cd/configs/swarm/genesis.json#L185

This is backed by the `ExecutorMode` struct:

https://github.com/hyperledger/iroha/blob/964476722e2a219becaacdb3676ca058ec5748cd/genesis/src/lib.rs#L122-L131

As we discussed in #4239, `executor` field with file path should be renamed to `executor_file` for uniformity.

In addition to that, I propose to remove inline executor mode. It was effectively deprecated a long time ago: there was a warning printed when the inline mode is used (cannot find references for that). The reason is that inlining WASM blob makes the whole genesis file (1) clunky and (2) hardly reproducible due to WASM compilation intricacies.




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 22:34:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4290" class=".btn">4290</a>
            </td>
            <td>
                <b>
                    [suggestion] Remove `parse_display` dependency entirely
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                In #4239 @mversic suggested to remove `parse_display` dependency entirely from the workspace. At the moment it is used by `iroha_ffi_derive`:

https://github.com/hyperledger/iroha/blob/df8c49aab4842aeac64291b108fa6cfcd04fffbe/ffi/derive/Cargo.toml#L27

There are other crates, like `strum` and `serde_with`, that we usually rely on instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 22:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4289" class=".btn">4289</a>
            </td>
            <td>
                <b>
                    [suggestion] Use `nonzero_ext` across workspace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                #4239 introduced `nonzero_ext` dependency in `iroha_config`. @mversic suggested that it might be a good idea to use it all across the workspace.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-18 22:20:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4227" class=".btn">4227</a>
            </td>
            <td>
                <b>
                    Support encoding/decoding to/from JSON in `parity_scale_decoder`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                1. rename `parity_scale_decoder` to `parity_scale_codec` or something similar
2. add support to encode/decode SCALE to/from JSON

atm, we're supporting only decoding to Rust debug format. I think we should just replace that with JSON, but we can also support different formats with some flag
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 11:25:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4226" class=".btn">4226</a>
            </td>
            <td>
                <b>
                    Prevent registering genesis Domain or Account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                We have to make sure that instructions that try to register "genesis" domain or "genesis@genesis" account are always rejected. Tests should be added as well. Additionally, if there are none, tests should be added that confirm that any transaction signed by the "genesis@genesis" is rejected
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 07:26:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4224" class=".btn">4224</a>
            </td>
            <td>
                <b>
                    `SignedBlock` is immutable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                After #4918 was merged the same should be done for `SignedBlock`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-23 06:52:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4223" class=".btn">4223</a>
            </td>
            <td>
                <b>
                    Reject `BlockMessage`s eagerly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Optimization</span><span class="chip">Chore</span>
            </td>
            <td>
                              depending on the previously received control flow messages, is it possible that some of the `BlockMessage`s should just be rejected?

_Originally posted by @mversic in https://github.com/hyperledger/iroha/pull/4115#discussion_r1449877651_
            
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 09:01:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4218" class=".btn">4218</a>
            </td>
            <td>
                <b>
                    [suggestion] Remove JSON encoding for API Version and Health requests, use plain text
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                ## Description

When you `GET /api_version`, you get a JSON:

```json
"1"
```

I think it is redundant to use JSON here and plain text would be just fine:

```
1
```

Same applies for `GET /health`:

```json
"Healthy"
```

There is no any reason to use JSON here over plain text.

### Benefits

Simplify API a little bit, remove redundancy.

### Research

A simple patch of this sections would suffice:

https://github.com/hyperledger/iroha/blob/565271dd043b6371c1fc2e4edce0754a3058c1bb/torii/src/routing.rs#L308-L317

https://github.com/hyperledger/iroha/blob/565271dd043b6371c1fc2e4edce0754a3058c1bb/torii/src/routing.rs#L139-L141


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 01:58:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4197" class=".btn">4197</a>
            </td>
            <td>
                <b>
                    [refactor]: Improve decoding of `ChainId`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                              This could be improved by using constructor `fn new(inner: impl Into<Box<str>>)`.
I will extract it into separate good first issue.

_Originally posted by @Erigara in https://github.com/hyperledger/iroha/pull/4185#discussion_r1450199917_

Idea is to remove redundant clone by directly convert from `String` to `Box<str>`.
            
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-12 10:25:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/4176" class=".btn">4176</a>
            </td>
            <td>
                <b>
                    [suggestion] Support `release` profile in `test_env.py`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">question</span><span class="chip">iroha2</span><span class="chip">Tests</span>
            </td>
            <td>
                ## Description

`test_env.py` builds and uses several binaries in `debug` mode (`kagami`, `iroha`, `iroha_client_cli`). In some cases I find it more practical to setup a testing environment using `release` binaries. When I do not change binaries themselves, but want to run tests again and again, tests running with `release` Iroha build might complete much faster, **although I haven't checked**.

So, my request is to extend `test_env.py` CLI with an argument to specify using binaries with `release` profile:

```shell
./test_env.py setup --release
# or
./test_env.py setup --profile=release
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-26 11:16:47 +0000 UTC
    </div>
</div>

