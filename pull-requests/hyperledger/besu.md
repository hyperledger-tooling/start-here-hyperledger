---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4286" class=".btn">#4286</a>
            </td>
            <td>
                <b>
                    create AbstractJsonRpcTest for better code reuse in other similar tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Pedro Novais <jpvnovais@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Abstracts some logic to be reused in similar tests, as suggested in PR #4146. (Helpful in downstream [fork](https://github.com/hyperledger/besu/pull/4146/files#diff-d27d85eaed527f7ef2ead8611cf0a17b4e33ed7c11dd341385eb9e9acfd30b70R11))

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 13:14:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4283" class=".btn">#4283</a>
            </td>
            <td>
                <b>
                    interpret an empty string (0x80) as an unsigned byte of 0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">mainnet</span>
            </td>
            <td>
                Signed-off-by: Stefan <stefan.pingel@consensys.net>

## PR description
This PR addresses Besu failure to decode a devp2p Hello message that contains the witness protocol capability version 0. In that Hello message the version of the witness protocol is encoded as 0x80 (zero length string), which is a valid way of encoding the version number 0.  

## Fixed Issue(s)
fixes #4279

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 05:55:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4282" class=".btn">#4282</a>
            </td>
            <td>
                <b>
                    Flexible Privacy Groups feature - Support to Tessera's EC encryptor
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Flexible privacy contracts are modified so they allow the use of enclave public keys longer than 32 bytes. This way the feature will now support the EC encryptor mode of Tessera. Java classes adapted as well so they could encode/decode Solidity `bytes` properly.

Since there were `bytes32` parameters in the method signatures of the proxy contract, I could not just upgrade the implementation. This means that the changelog should warn about this change. I guess it is ok since [in the actual documentation, this feature is referred to as an experimental one](https://besu.hyperledger.org/en/stable/HowTo/Use-Privacy/Use-FlexiblePrivacy/) and changes like this might be expected.

## Fixed Issue(s)

fixes https://github.com/hyperledger/besu/issues/4262


## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 15:21:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4280" class=".btn">#4280</a>
            </td>
            <td>
                <b>
                    working on snapshot impl for bonsai
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Karim TAAM <karim.t2am@gmail.com>

<!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Documentation

- [ ] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-19 12:37:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/4278" class=".btn">#4278</a>
            </td>
            <td>
                <b>
                    Trace block timeout
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Thanks for sending a pull request! Please check out our contribution guidelines: -->
<!-- https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md -->

## PR description
Added some thread management around `trace_block` to prevent large traces from blocking the node.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->
Addresses #4050 

## Documentation

- [x] I thought about documentation and added the `doc-change-required` label to this PR if
    [updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 23:30:10 +0000 UTC
    </div>
</div>

