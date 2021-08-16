---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/156" class=".btn">#156</a>
            </td>
            <td>
                <b>
                    Remove retry for correlating transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Counterpart to https://github.com/hyperledger-labs/firefly-ethconnect/pull/139.

This will reduce the noisy logs when using tokens, because tokens generates ethconnect events that are "unexpected" from the perspective of the blockchain plugin. There will still be a single warning printed for each token transaction, but that's...a little better?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-14 01:08:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/154" class=".btn">#154</a>
            </td>
            <td>
                <b>
                    Add support for creating token pools
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial support for tokens by plugging in an instance of https://github.com/hyperledger-labs/firefly-tokens-erc1155.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 19:15:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/153" class=".btn">#153</a>
            </td>
            <td>
                <b>
                    Update CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I was missing the `@` characters on the GitHub IDs previously :(
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 18:25:46 +0000 UTC
    </div>
</div>

