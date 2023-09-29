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
                    0.10.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.10.3
                </span>
            </td>
            <td>
                Release 0.10.3 is a patch release to add an upgrade process for very old versions of Aries Cloud Agent Python (circa [0.5.2](#052)). If you have a long time deployment of an issuer that uses revocation, this release could correct internal data (tags in secure storage) related to revocation registries. Details of the about the triggering problem can be found in [Issue \#2485].

[Issue \#2485]: https://github.com/hyperledger/aries-cloudagent-python/issue/2485

The upgrade is applied by running the following command for the ACA-Py instance to be upgraded:

`./scripts/run_docker upgrade --force-upgrade --named-tag fix_issue_rev_reg`

## What's Changed
* 0.10.3 by @swcurran in https://github.com/hyperledger/aries-cloudagent-python/pull/2522
* Feat: Upgrade from tags and fix issue with legacy IssuerRevRegRecords [<=v0.5.2] @shaangill025 https://github.com/hyperledger/aries-cloudagent-python/pull/2486


**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.10.2...0.10.3
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.10.3" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-09-29 16:10:11 +0000 UTC
    </span>
</div>

