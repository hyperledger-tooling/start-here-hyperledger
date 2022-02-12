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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1628" class=".btn">#1628</a>
            </td>
            <td>
                <b>
                    Fix for non-revoc proof with no timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 20:39:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1627" class=".btn">#1627</a>
            </td>
            <td>
                <b>
                    Upgrade ConfigArgParse to version 1.5.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - This allows multi-instance multi-argument parameters such as `--inbound-transport` to be specified using the associated environment variable.  Version 1.2.3 of ConfigArgParse was unable to parse the associated environment variables properly.
- Example using the environment variable for `--inbound-transport`: `ACAPY_INBOUND_TRANSPORT=[[\"http\",\"0.0.0.0\",\"8021\"],[\"ws\",\"0.0.0.0\",\"8023\"]]`

Results In:
```
::::::::::::::::::::::::::::::::::::::::::::::
:: Aries Cloud Agent                        ::
::                                          ::
::                                          ::
:: Inbound Transports:                      ::
::                                          ::
::   - http://0.0.0.0:8021                  ::
::   - ws://0.0.0.0:8023                    ::
...
```

Signed-off-by: Wade Barnes <wade@neoterictech.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-10 21:03:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1620" class=".btn">#1620</a>
            </td>
            <td>
                <b>
                    Breaking change: ConnRecord their_role and state inconsistency between 0160 and 0023
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-07 16:55:12 +0000 UTC
    </div>
</div>

