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
                PR <a href="https://github.com/hyperledger/besu/pull/3339" class=".btn">#3339</a>
            </td>
            <td>
                <b>
                    Merge main into merge branch
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

Merge `main` into `merge`
* merge main
* convert merge-specific classes using log4j to slf4j
* add slf4j labmda shim to util project, for parameters that are expensive to evaluate

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->

## Changelog

- [ ] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 20:02:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3333" class=".btn">#3333</a>
            </td>
            <td>
                <b>
                    Add ec-curve parameter public key export/export-address subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
- Add ec-curve parameter public key export/export-address subcommands
- Defaults to secp256k1
- Support secp256k1 and secp256r1
- Added a log message when creating a key with the selected ec curve name 

Note: due to the static initialization of the SignatureAlgorithmFactory, we need to ensure that its setup happens before any other key-related operation. This is why I have added it as the first instruction in the `run()` method in the subcommands.

## Fixed Issue(s)
fixes #3206 

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 09:46:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3331" class=".btn">#3331</a>
            </td>
            <td>
                <b>
                    Update besu-native to 0.4.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                https://github.com/hyperledger/besu-native/releases/tag/0.4.3
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 05:21:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/3330" class=".btn">#3330</a>
            </td>
            <td>
                <b>
                    21.10.9 update hashes to match regenerated artefacts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Besu CI pipeline was re-run on the same commit, generating the same artefact with a different hash

Signed-off-by: Sally MacFarlane <sally.macfarlane@consensys.net>

See https://app.circleci.com/pipelines/github/hyperledger/besu?branch=release-21.10.x&filter=all 
^ looking at this - pipeline for commit 8f465c0 was run twice. 7 days ago and 2 days ago.
Since the commit is the same https://github.com/hyperledger/besu/commit/8f465c0faf568b395c8e271c6caff6f79d77a7a7
I'm updating the hashes.
Also ref https://github.com/hyperledger/homebrew-besu/pull/70

## Changelog

- [x] I thought about the changelog and included a [changelog update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 04:29:58 +0000 UTC
    </div>
</div>

