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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1591" class=".btn">#1591</a>
            </td>
            <td>
                <b>
                    Fixes for revocable credential issuance
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fix RevocationError instantiations
- Ensure transaction is not left open when IndyIssuerRevocationRegistryFullError exception is raised

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-08 01:26:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1589" class=".btn">#1589</a>
            </td>
            <td>
                <b>
                    Fix for Test Harness --version issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
```
aries_cloudagent/commands/upgrade.py
from packaging import version as package_version
ModuleNotFoundError: No module named 'packaging'
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 15:07:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1583" class=".btn">#1583</a>
            </td>
            <td>
                <b>
                    Multiple Indy Ledger - Askar Fixes and Cleanup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>

- Fixes issues with multiple ledger support when using `askar` wallet-type. Issue (#1567) reported [here](https://github.com/hyperledger/aries-cloudagent-python/issues/1567#issuecomment-1004153961).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-04 00:12:04 +0000 UTC
    </div>
</div>

