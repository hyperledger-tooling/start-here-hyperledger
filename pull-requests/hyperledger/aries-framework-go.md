---
layout: default
title: aries-framework-go
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-go
---

# aries-framework-go <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-go){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3272" class=".btn">#3272</a>
            </td>
            <td>
                <b>
                    refactor: change type of Forward.Msg from byte array to Envelope stru…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Change Msg field of `Forward` model. Make nested packed forwards while creating forward message

**Summary:**

- Change Msg field of `Forward` from byte array to `Envelope` structure as defined in [protocol](https://github.com/hyperledger/aries-rfcs/blob/main/concepts/0094-cross-domain-messaging/README.md#corerouting10forward)
- Make nested packed forwards(for each routing key) while creating forward message


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 12:08:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3271" class=".btn">#3271</a>
            </td>
            <td>
                <b>
                    CL Anoncreds tink primitives
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
CL Anoncreds tink primitives

**Description:**
This is the first PR to support CL Anoncreds in Aries-framework-go [#180](https://github.com/hyperledger/aries-framework-go/issues/180).

**Summary:**
- Adds [ursa-wrapper-go](https://github.com/hyperledger/ursa-wrapper-go) as an optional dependency (under the `ursa` build tag).
- Adds think crypto primitives and keys for the Issuance flow 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 06:25:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3270" class=".btn">#3270</a>
            </td>
            <td>
                <b>
                    feat: add ext db packages to REST Agent (#3269)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ana Maria Franco <afrancoc2000@gmail.com>

**Title:**
Adding extended database packages to the Rest Agent

**Description:**
The Rest Agent doesn't have an easy way to use the [extended package databases](https://github.com/hyperledger/aries-framework-go-ext/tree/ce8776c10037404f5c31a67aced0df6828bc4c28), so, I'm adding the posibility to use them in here.

[Issue 3269](https://github.com/hyperledger/aries-framework-go/issues/3269)

**Summary:**

I'm adding support for the Rest Agent to: couchdb, mongodb, mysql, postgresql, from the [aries-framework-go-ext](https://github.com/hyperledger/aries-framework-go-ext) package, and updating the docs.

Also I ran `go mod tidy -go=1.16 && go mod tidy -go=1.17` and updated the go.mod keeping compatibility with go 1.16. Not sure if compatibility with go 1.16 is still wanted.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-09 14:28:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-go/pull/3268" class=".btn">#3268</a>
            </td>
            <td>
                <b>
                    feat: Legacy Anoncrypt(RFC-0019) DIDComm v1 implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Title:**
Legacy Anoncrypt(RFC-0019) DIDComm v1 implementation

**Description:**
This is the PR to support legacy anoncrypt (pack/unpack) while DIDComm V1 is used.

**Summary:**
Add anoncrypt packing/unpacking using Chacha20 encryption algorithm

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 14:06:56 +0000 UTC
    </div>
</div>

