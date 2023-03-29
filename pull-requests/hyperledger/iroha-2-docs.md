---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/303" class=".btn">#303</a>
            </td>
            <td>
                <b>
                    [feature] #301: render data model schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #301 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 01:46:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/302" class=".btn">#302</a>
            </td>
            <td>
                <b>
                    Weakly organised notes and JS tutorial rewriting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is not intended to be merged. I made it to share my WIP with others to collect feedback.

Related issues:

- #275
- #276
- #298 
- #301 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-26 07:00:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/300" class=".btn">#300</a>
            </td>
            <td>
                <b>
                    [chore]: stylistic changes (#299)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've fixed some links and updated an info block for convenience.
I hope it helps.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 07:25:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    [chore] #295: add XDG specification link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As stated in https://github.com/hyperledger/iroha-2-docs/issues/295, we should add a link to the XDG specification if someone needs to get acquainted with it.

---


Moreover, a footnote telling which variable in the spec would be helpful. For example, we can write that `iroha_client_cli` will look for `$XDG_CONFIG_HOME`.
Iroha doesn't start on my machine right now, while digging in the source shows [this code](https://github.com/hyperledger/iroha/blob/726f5eabf65a79ea618b4fce62a09cee7a5b13d1/client_cli/src/main.rs#L141-L142).

So far, I've tried this code to see that it shows a subdirectory relative to the current working dir.

```rust
#![allow(unused)]
#![feature(absolute_path)]
#[cfg(unix)]
fn main() -> std::io::Result<()> {
  use std::path::{self, Path};

  let absolute = path::absolute("config")?;
  println!("{}", absolute.display());
  Ok(())
}
```

Could someone explain how the config lookup works to me? I understand one of the possible paths is the config subdirectory relative to a current one, but where do we look for XDG paths?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-23 03:56:31 +0000 UTC
    </div>
</div>

