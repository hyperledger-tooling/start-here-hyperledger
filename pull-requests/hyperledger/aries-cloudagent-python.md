---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1921" class=".btn">#1921</a>
            </td>
            <td>
                <b>
                    Leave credentialStatus element in the LD credential
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                During the implementation we stumbled upon inability of a recipient to validate a credential offer. That happens because the `credentialStatus` fields is popped from the credential offer (see [here](https://github.com/sake/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/issue_credential/v2_0/formats/ld_proof/handler.py#L506)). Later, the two entities (one from credential request, and another from the offer) are being compared, and naturally the comparison fails, which leads to inability to receive the credential offer.
This change makes sure that the comparison of the provided reference data is comparable with the credential content, by replacing the `pop` method with `get` to leave the `credentialStatus` intact in the offer object.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 12:06:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1920" class=".btn">#1920</a>
            </td>
            <td>
                <b>
                    Simple did registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This Pr simplifies the did registry to a list for future development of a did registry interface.

Signed-off-by: Adam Burdett <burdettadam@gmail.com>
Co-authored-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-29 17:57:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1916" class=".btn">#1916</a>
            </td>
            <td>
                <b>
                    Revert "[#1895] Stopping the aca-py shell process keeps python process running"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This reverts commit 67db5de43770933efd8cbc816ffb5d3850fa5785.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 14:29:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1915" class=".btn">#1915</a>
            </td>
            <td>
                <b>
                    chore: update pydid
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recent changes to the resolution of sov/indy DIDs caused PyDID to parse
service endpoints that should have been recognized as DIDComm services
as plain services. This broke some logic in accepting invitations from
public DIDs. Pulling in these updates from PyDID resolves the issue.

Signed-off-by: Daniel Bluhm <dbluhm@pm.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 13:31:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1914" class=".btn">#1914</a>
            </td>
            <td>
                <b>
                    feat: include connection ids in keylist update webhook
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the connection IDs of the mediated connections. This should make it easier to trigger the next step in a flow (i.e. accept a connection request for one of the connections, if it's in the right state).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 14:55:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1913" class=".btn">#1913</a>
            </td>
            <td>
                <b>
                    Remove aca-py check for unrevealed revealed attrs on proof validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issue #1893

Removes the "hard" verification on un-revealed attributes and adds "verify_msgs" to the presentation exchange record to describe any warnings or errors encountered when processing the received proof.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 13:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1912" class=".btn">#1912</a>
            </td>
            <td>
                <b>
                    fix: incorrect response schema for discover features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small change that won't really affect anything but OpenAPI json and client generators.

The query features endpoint returns the discovery record directly rather than nesting it in a `results` attribute.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 19:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1911" class=".btn">#1911</a>
            </td>
            <td>
                <b>
                    [#1895] Stopping the aca-py shell process keeps python process running
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 17:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1910" class=".btn">#1910</a>
            </td>
            <td>
                <b>
                    Create sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 16:17:10 +0000 UTC
    </div>
</div>

