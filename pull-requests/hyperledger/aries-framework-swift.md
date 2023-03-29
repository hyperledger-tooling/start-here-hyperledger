---
layout: default
title: aries-framework-swift
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-swift
---

# aries-framework-swift <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-swift){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    ci: Use strict option for swiftlint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 11:42:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    enhance wallet error message more descriptable with failure reason.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Checklist

- [x] have run AriesFrameworkTests
- [x]  I have run AllTests

# Description

it would be help to solve problems if framework provide detailed messages about indy when an error occurs in wallet .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 06:48:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/35" class=".btn">#35</a>
            </td>
            <td>
                <b>
                    ci: Fix workflow error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Github [macOS runners](https://github.com/actions/runner-images/blob/main/images/macos/macos-12-Readme.md) use cocoapods 1.12.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-27 07:16:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    refactor: Prepare to support multiple wallets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Checklist

- [x]  have run AriesFrameworkTests
- [x] I have run AllTests

# Description

Checking the actual existance of the file may be a better approach than relying on UserDefault to determine the existence of the wallet.

In this task, I changed the way to manage master secret id.  I referenced this from aries-cloudagent-python. 
Master secret id is just a label given to the master secret stored in the wallet, so there is no need to create it arbitrarily.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 13:25:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-swift/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Exclude walletKey from AgentConfig encode/decode.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Checklist

- [x] I have run AriesFrameworkTests
- [x] I have run AllTests

# Description

Exclude walletKey from AgentConfig encode/decode. It should be stored separately in a safer place.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-24 00:14:12 +0000 UTC
    </div>
</div>

