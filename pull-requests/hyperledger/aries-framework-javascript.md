---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    ci: get last alpha package version from npm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We currently use the commit number, but this is incorrect as the number will be reset to 0 again when the next minor version is released.

E.g. instead of the tag `alpha.347` it will now be `0.2.0-alpha.12`.

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-31 10:44:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    fix: incorrect encoding of services for did:peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes for incorrect encoding of services in peer dids. Checked against the [peer-did-python](https://github.com/sicpa-dlab/peer-did-python) implementation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 13:07:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/609" class=".btn">#609</a>
            </td>
            <td>
                <b>
                    feat: support new did document in didcomm message exchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds support for sending and receiving messages that are stored using peer dids and the new did record. The sending of messages is completely the same, mainly because I unified the `Service` classes from the old and new did document class as they were 100% identical. This made integrating it quite straight forward

Current exchange is still working, but haven't been able to properly test the message exchange using the new did documents yet as we don't have DID exchange etc yet. Will add proper tests over the next few days, but you should be fine to use for now.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 17:09:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    feat: add support for did:peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds support for did:peer dids as described in the peer did method specification. It supports all methods (0,1,2).

The implementation should be seen as experimental as the peer did spec is quite complex and there's a good chance I messed some things up.

One thing that needs fixing for sure is the encoding of didcomm services, but I need to wait for a reply on that: https://github.com/decentralized-identity/peer-did-method-spec/issues/39
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 22:35:19 +0000 UTC
    </div>
</div>

