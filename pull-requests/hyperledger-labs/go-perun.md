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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Revert: Remove settle secondary (#351)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is linked to https://github.com/hyperledger-labs/perun-eth-backend/pull/47 and reverts commit https://github.com/hyperledger-labs/go-perun/commit/be6e07257c123309c98fbbea4b86440275be2797.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-20 13:35:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    #395_Fix_Falling_Unit_Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
This PR serves to fix the #395 issue of failing unit tests. 

### App Randomizer Internal Test 
Location: `channel/test/app_randomizer_internal_test.go`

Cause: The issue stems from the lack of Comparator (`Equal`) for MockAppRandomizer. This leads to the test not recognizing that the default appRandomizer has already been set in the internal test.

Solution: Add an identifier to the MockAppRandomizer to compare the old and new appRandomizer.

### Dialer Internal Test
Location: (`wire/net/simple/dialer_internal_test.go`)

Cause: Like @RmbRT has pointed out, there is a race between the init of `wire/simple` and `backend/sim/wire`, which set the RandomAddress and RandomAccount functions to be used in the internal tests.

Solution: Add the initialization of `NewRandomAddress` and `NewRandomAccount` to use the implementation from the `wire/simple`.

Alternative: Remove `init()` of `wire/simple` and only use the init of `backend/sim/wire`. This also results in passing internal tests but might cause issues for packages using `wire/simple` (need further investigation).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-19 14:51:08 +0000 UTC
    </div>
</div>

