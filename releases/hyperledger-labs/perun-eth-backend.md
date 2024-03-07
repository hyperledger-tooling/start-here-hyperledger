---
layout: default
title: perun-eth-backend
parent: Hyperledger Labs
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger-labs/perun-eth-backend
---

# perun-eth-backend <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-eth-backend){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    Athos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v0.5.0
                </span>
            </td>
            <td>
                Improved Contract Compatibility, Swap Parallelization and other fixes.

## Added :boom:
* AppID Type to generalize App identifiers instead of using Ethereum addresses: [#44] :boom:
* Add a shared nonce map to ensure that the nonce is incremented for all transactions, including those sent in parallel: [#43]
* Add ability to set the gas limits instead of using fixed values: [#46]
* Add pointer receiver to Asset.UnmarshallBinary to return the unmarshalled value instead of the default: [#36]

## Fixed
* Fix the order from Asset.MarshalBinary: [#36]
* Restore compatibility between go-perun post-0.10.6 and eth-backend: [#44]

## Changed
* Use git diff instead of go test to check if the bindings are generated correctly: [#33]
* Remove IncreaseAllowance and use Approve instead to ensure compatibility with more contracts in the depositing process: [#43]

## Legend
- <span id="breaking">:boom:</span> This is a breaking change, e.g., it changes the external API.
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger-labs/perun-eth-backend/releases/tag/v0.5.0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2024-03-05 12:21:50 +0000 UTC
    </span>
</div>

