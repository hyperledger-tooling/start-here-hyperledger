---
layout: default
title: ursa
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/ursa
---

# ursa <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/ursa){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/ursa/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Run libursa tests on Ubuntu 20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds `libursa`-specific jobs to GH Actions (namely building `libursa` and running its tests).

One thing I'm not sure about is the workaround for getting `libursa` to build on its own -- currently, running `cargo build` in the `libursa` directory on the `main` branch will yield this error:
```
error: current package believes it's in a workspace when it's not:
current:   ursa/libursa/Cargo.toml
workspace: ursa/Cargo.toml

this may be fixable by adding `libursa` to the `workspace.members` array of the manifest located at: ursa/Cargo.toml
Alternatively, to keep it out of the workspace, add the package to the `workspace.exclude` array, or add an empty `[workspace]` table to the package's manifest.
```
I heeded the second suggestion and excluded `libzmix` and `libursa` from the workspace, but I'm not sure if this is the correct course of action. Feel free to request/make changes!

As for the changes to `libursa/src/kex/secp256k1.rs`, the compatibility test was never updated after `libsecp256k1` was replaced with `k256` in #171, so this PR also fixes that.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-14 04:00:58 +0000 UTC
    </div>
</div>

