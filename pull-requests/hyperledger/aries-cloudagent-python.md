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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3106" class=".btn">#3106</a>
            </td>
            <td>
                <b>
                    Fix the check for vc_di proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix the error that is getting raised in AATH.  (Double checked and the AATH tests will now pass.)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 18:15:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3105" class=".btn">#3105</a>
            </td>
            <td>
                <b>
                    Make single wallet config more explicit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This changes some naming and configuration to make the multitenant single wallet vs multi wallet settings and usage more clear. Askar wallets can use either the basic manager `MultitenantManager` which is used by default and creates a DB/wallet for each tenant. Or, it can use the `AskarProfileMultitenantManager` to create subwallets in a single DB/wallet. This has been renamed to `SingleWalletAskarMultitenantManager` for clarity, and the config changed to `multitenancy-config: '{"wallet_type": "single-wallet-askar"}'` from `multitenancy-config: '{"wallet_type": "askar-profile"}'`

Also fixed an issue with the upgrade check during startup that was using the base manager before initialization and creating subwallet db's on restart when in single wallet mode. I'm looking into this more because the `BaseMultitenantManager` is injected in many other places. Need to make sure they are also using the correct manager via the `MultitenantManagerProvider`.

Added some documentation in `Multitenancy.md`

***Note:*** the multitenant_provider plugin needs to be update because it inherits this class. Already done in my forked repo. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-17 17:32:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3103" class=".btn">#3103</a>
            </td>
            <td>
                <b>
                    Library update 15/07/24 / Fix unit test typing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes some type checking syntax in unit tests. I'm not really sure why these didn't get flagged before or why the command line doesn't seem to pick up these specific errors. They are easy to fix though so I just changed them.

Upgrades ruff, pytest-ruff, portalocer and mkdocs-material
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 16:24:54 +0000 UTC
    </div>
</div>

