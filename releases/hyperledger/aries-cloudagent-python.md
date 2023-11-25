---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.10.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.5
                </span>
            </td>
            <td>
                Release 0.10.5 is a high priority patch release to correct an issue with the handling of the JSON-LD presentation verifications, where the status of the verification of the `presentation.proof` in the Verifiable Presentation was not included when determining the verification value (`true` or `false`) of the overall presentation. A forthcoming security advisory will cover the details.

Anyone using JSON-LD presentations is recommended to upgrade to this version of ACA-Py as soon as possible.

## What's Changed
* fix(backport): report presentation result by @dbluhm in https://github.com/hyperledger/aries-cloudagent-python/pull/2622
* 0.10.5 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2623


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.10.4...0.10.5
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.5" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-11-22 03:19:56 +0000 UTC
    </span>
</div>

