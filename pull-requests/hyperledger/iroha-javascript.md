---
layout: default
title: iroha-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-javascript
---

# iroha-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    fix: bundle cjs script for crypto lib
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now it should work in node without on-demand transformations like `esbuild-register` or `sucrase/register`. But the way it is done now is not the best... FIXME

Version bumps:

- `@iroha2/client` - 0.2.0 -> 0.2.1
- `@iroha2/crypto` - 0.1.0 -> 0.2.0

#### Breaking changes

Only one - initialization way:

```ts
// was
import init from '@iroha2/crypto'

// now
import { init } from '@iroha2/crypto'
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-24 11:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/75" class=".btn">#75</a>
            </td>
            <td>
                <b>
                    Bump `@iroha2/client` version to 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Forgot to do it in previous PR (
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 13:27:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-javascript/pull/74" class=".btn">#74</a>
            </td>
            <td>
                <b>
                    Update data model with new SCALE codec compiler, actualize client code, implement `Fixed`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-22 12:44:27 +0000 UTC
    </div>
</div>

