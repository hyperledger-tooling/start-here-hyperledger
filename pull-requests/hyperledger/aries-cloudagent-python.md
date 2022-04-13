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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1726" class=".btn">#1726</a>
            </td>
            <td>
                <b>
                    Use provided connection_id if provided
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue https://github.com/hyperledger/aries-cloudagent-python/issues/1703

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-11 21:39:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1725" class=".btn">#1725</a>
            </td>
            <td>
                <b>
                    feat: create new JWT tokens and invalidate older for multitenancy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Tokens will now include an `iat` value which is also stored in the wallet record. If the `iat` of the JWT doesn't match the user won't be authorized. This means when a new token is created (using the multitenant apis) the old token becomes invalid.

Looking for some input if this is a desired approach. It is a breaking change as previously you would always get the same token, while now you always get a new token revoking the older tokens.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-10 14:55:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1722" class=".btn">#1722</a>
            </td>
            <td>
                <b>
                    Prep for adding the 0.7.4-rc0 tag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 20:07:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1721" class=".btn">#1721</a>
            </td>
            <td>
                <b>
                    Duplicate checking for schema and cred def
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue:  https://github.com/hyperledger/aries-cloudagent-python/issues/1707

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 18:28:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1720" class=".btn">#1720</a>
            </td>
            <td>
                <b>
                    Adds support to faber demo for returning json response in connectionless proof-requests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also updates demo to use `WEBHOOK_TARGET`, when supplied, to construct presentation request exchange urls 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 14:34:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1719" class=".btn">#1719</a>
            </td>
            <td>
                <b>
                    Allow specifying key derivation method on sub-wallet create
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When working in managed multi-tenancy mode, we store the keys for the sub-wallets within a WalletRecord in ACA-Py. These keys are then recalled when needed and used to unlock the wallet for processing messages or admin API requests intended for that sub-wallet. In the process of opening the wallet, the key is pushed through a key derivation algorithm to transform it into a wallet encryption key. This key derivation algorithm is a costly operation.

This PR implements allowing the key derivation method to be specified when creating a sub-wallet. This means that a multi-tenant ACA-Py agent can elect to use the `RAW` derivation method, for instance, and significantly reduce the wallet open cost.

Since these keys are securely stored in ACA-Py, using a `RAW` key does not seem to impact security of the key. Additionally, I don't think the profile of potential attack changes from using the key derivation method when considering wallet tokens.

Credit to @burdettadam.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-07 14:02:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1718" class=".btn">#1718</a>
            </td>
            <td>
                <b>
                    Allow deletion of invalid V20PresExRecord - failing schema validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Related to issue #1687, there was a bug in DIF presentation proposal code where the presentation request created from the proposal with auto flags was not according to the marshmallow schema. This rendered multiple present-proof-v2 endpoints unusable due to schema validation error. This bug was fixed in PR #1690.
- This PR is a recreation of @matgnt PR#1701 as some tests were failing after rebase but local tests were passing. Changes here allow for the deletion of such records. For now, it only handles `V20PresExRecord` but if required it can be extended to other BaseExchangeRecord.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 20:55:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1716" class=".btn">#1716</a>
            </td>
            <td>
                <b>
                    Fix order of operations connecting faber to endorser
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Fixes issue: https://github.com/hyperledger/aries-cloudagent-python/issues/1703

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 15:41:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1715" class=".btn">#1715</a>
            </td>
            <td>
                <b>
                    run_docker start - pass environment variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
- resolve #1330 
- Closed PR #1709, there were issues applying `fixup` during rebase to cleanup commit history. I thought it is safer to recreate the PR as it has minor changes.

@MonolithicMonk ACAPY_INBOUND_TRANSPORT should be specified as `ACAPY_INBOUND_TRANSPORT=[[\"http\",\"0.0.0.0\",\"8021\"]]` and not as `ACAPY_INBOUND_TRANSPORT=[["http","0.0.0.0","8021"]]`

You can pass environment variables using `ENV_VARS` variable [similar to `PORTS`]. For your reference:
```
PORTS="5002 8002" ENV_VARS="ACAPY_INBOUND_TRANSPORT=[[\"http\",\"0.0.0.0\",\"8021\"]]" \ 
./scripts/run_docker start ......
``` 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-06 14:42:20 +0000 UTC
    </div>
</div>

