---
layout: default
title: solang-llvm
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang-llvm
---

# solang-llvm <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang-llvm){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang-llvm/pull/13" class=".btn">#13</a>
            </td>
            <td>
                <b>
                    Update workflow name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The workflow to build LLVM binaries must not be called `Build Release Binaries`, because we are not doing so.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 18:09:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang-llvm/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Remove bloat from docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Reduce the image size by 30% from 4.9G to 3.45G

- Strip LLVM and solana binaries
- Remove cargo registry cache after `cargo install`
- Install only the `minimal` rustup profile. This gets rid of the docs, which are several 100mb
- Change the apt command so that the autoclean works
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 12:32:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang-llvm/pull/10" class=".btn">#10</a>
            </td>
            <td>
                <b>
                    Use Rust 1.65
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Companion to https://github.com/hyperledger/solang/pull/1236
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 10:31:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang-llvm/pull/9" class=".btn">#9</a>
            </td>
            <td>
                <b>
                    Upgrade Anchor version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The container image needs to be updated so that the PR tests for https://github.com/hyperledger/solang/pull/1233 can run correctly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 19:13:45 +0000 UTC
    </div>
</div>

