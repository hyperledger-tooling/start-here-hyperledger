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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1596" class=".btn">#1596</a>
            </td>
            <td>
                <b>
                    Fix tails_local_path format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: DaevMithran <daevmithran1999@gmail.com>

Issue is not fixed yet. Tried replacing the white spaces with %20 in tails_local_path. I'm not receiving error in swagger now. I'm receiving error in the logs. And it creates only one rev_reg instead of two now. Can anyone guide me on this?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-11 21:13:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1593" class=".btn">#1593</a>
            </td>
            <td>
                <b>
                    Added missed new module -- upgrade -- to the RTD generated docs
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
        Created At 2022-01-10 23:26:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1592" class=".btn">#1592</a>
            </td>
            <td>
                <b>
                    Doh....update the date in the Changelog for 0.7.3
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
        Created At 2022-01-10 22:00:07 +0000 UTC
    </div>
</div>

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

