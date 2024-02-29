---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/403" class=".btn">#403</a>
            </td>
            <td>
                <b>
                    Go 1.21 upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This Pull Request aims to upgrade the Go programming language version to 1.21 across the project. Additionally, it includes updates to the GitHub Continuous Integration (CI) pipeline to accommodate the new version and ensures the codebase passes the updated linter.

## Changes Proposed:
### Upgrade Golang Version:

The Golang version has been updated from 1.17 to 1.21.
### Update GitHub CI Pipeline:

Modifications have been made to the existing GitHub CI pipeline configuration to support the updated Golang version.
The pipeline now includes steps for testing and building the project with Go 1.21.
### Code Changes:

- Necessary changes have been implemented throughout the codebase to ensure compatibility with Go 1.21.

- Any deprecated or outdated constructs have been replaced with their equivalent supported versions.

- The codebase has been refactored to pass the updated linter without errors or warnings.
### Why This Change is Necessary:
- Stay Current: Upgrading to the latest Golang version ensures that the project benefits from the latest language features, performance improvements, and bug fixes.
- Maintain Compatibility: Keeping the project up-to-date with the latest Golang version ensures compatibility with other libraries, tools, and dependencies.
- Enhance Code Quality: Updating the linter and addressing any issues found ensures that the codebase adheres to best practices and maintains a high level of quality.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-29 08:46:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    381 wire authentication
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
This PR serves to fix the #381 issue of Wire Authentication. 

### TLS Connection
Location: `wire/net/simple`

Issue: currently using TCP without TLS for communication. 

Solution: Implement a simple mutual TLS Dialer and TLS Listener in the `simple` package, the default net wire for `go-perun`.

Bonus: A simple connection test has also been set up with self-signed Certificates in `dialer_internal_test.go`

### Wire identity authentication
Location: `wire/address.go`, `wire/account.go`, and `wire/net/exchange_addr.go`, `wire.proto`

Issue: While each message currently contains a sender and recipient wire address in its Envelope, those are not yet authenticated; there is no signature in the `wire.proto`. This means anyone can send a message coming from SENDER, without needing the private key, thus allowing to spoof any wire identity.

Solution: Add Signing and Verifying for Account and Address. Like Wallet, the Account is expected to hold the private key, and the Address serves as the Public Key. Wire Authentication can be achieved by including a signature signed by the account in the `AuthResponseMsg.` Recipient can check the validity of this signature using the Sender Address (Public Key) to decrypt the signature.

### Wire Authentication Implementation
Location: `backend/sim/wire` and `wire/net/simple`

Description: A simple implementation for the integration of key-pair to be used for wire authentication has been implemented in the testing and default wire. 

For `backend/sim/wire`: This simple signing and verification of signature, independent from the given message.

For `wire/net/simple`: RSA-2048 Random-generated Key-Pair for (Account, Address), Signing of a given message by hashing and encrypting. Signature length: 256 Bits.

An address exchange test has also been added to the package to test the authentication function.


[Visualization](https://miro.com/app/board/uXjVNszT4kY=/?share_link_id=475156674819)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-26 09:00:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Update CHANGELOG to include v0.11.0 release
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
        Created At 2024-02-22 13:43:26 +0000 UTC
    </div>
</div>

