---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1081" class=".btn">#1081</a>
            </td>
            <td>
                <b>
                    Encode custom width integers using the next power of two width
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Anchor IDL does not support custom width integers. Instead of creating a user-defined type for them, we will encode them using the smaller integer width greater than the given one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 18:51:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1080" class=".btn">#1080</a>
            </td>
            <td>
                <b>
                    Substrate: Support contracts node v0.22
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Change the linker to use stabilized APIs for any remaining `__unstable__`
- Update integration tests:
  - Introduce a helper for the (currently) broken contracts `query` API
  - Use `WeightV2` for gas limits
  - Use estimated gas from dry run instead of hardcoded value
  - Compile test contracts in parallel
- Updates to the `latest` contracts CI image for pallet contracts v0.22.1. I'm aware that this is not ideal but it's what's available right now. There shouldn't be a breaking release soon, we can switch to `production` as soon as its here.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-24 11:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1079" class=".btn">#1079</a>
            </td>
            <td>
                <b>
                    Switch `ink!` dependency to beta release
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
        Created At 2022-11-22 13:19:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1078" class=".btn">#1078</a>
            </td>
            <td>
                <b>
                    Use named fields for casts in ast::Expression
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-21 08:46:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1077" class=".btn">#1077</a>
            </td>
            <td>
                <b>
                    Validate documentation examples on CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR moves most of our solidity code blocks into dedicated examples. Snippets that should work for all our targets go into the `/examples` directory, and target specific ones into `/examples/target`. I implemented a test to check that all examples successfully compile, in parallel.

Also a lot of examples contained syntactical errors, I fixed everything. Additionally they are now correctly formatted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 17:20:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1075" class=".btn">#1075</a>
            </td>
            <td>
                <b>
                    Fix bytes() cast from fixed length and vice versa
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sean Young <sean@mess.org>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-18 13:33:10 +0000 UTC
    </div>
</div>

