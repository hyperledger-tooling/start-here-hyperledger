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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1849" class=".btn">#1849</a>
            </td>
            <td>
                <b>
                    0.7.4 Release Changelog and version update
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
        Created At 2022-06-30 17:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1847" class=".btn">#1847</a>
            </td>
            <td>
                <b>
                    Fix handling of non-revocable credential when timestamp is specified (askar/credx)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Test output with the error (mixing revocable and non-revocable credentials in one proof): https://github.com/hyperledger/aries-cloudagent-python/pull/1761#issuecomment-1165468687

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-29 22:44:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1846" class=".btn">#1846</a>
            </td>
            <td>
                <b>
                    Update the Supported RFCs document for 0.7.4 release
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
        Created At 2022-06-29 17:09:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1845" class=".btn">#1845</a>
            </td>
            <td>
                <b>
                    Only run on main repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #1839

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-27 17:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1844" class=".btn">#1844</a>
            </td>
            <td>
                <b>
                    Fix a typo in DevReadMe.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is a typo in the example command to run the project using the docker container.

```
PORTS="5000:5000 8000:8000 1000:1000" ./scripts/run_docker start --inbound-transport http 0.0.0.0 10000 --outbound-transport http --debug --log-level DEBUG
```

It opens the port 1,000 for access instead of 10,000 which is specified as "inbound-transport". As a result, the agent wouldn't be accessible. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-25 18:12:05 +0000 UTC
    </div>
</div>

