---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/982" class=".btn">#982</a>
            </td>
            <td>
                <b>
                    style: prettier formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I somehow directly pushed to main and now messed up the prettier formatting. I restricted the branch protection to make sure it doesn't happen again. This PR fixes the prettier formatting.

﻿Signed-off-by: Timo Glastra <timo@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-12 13:17:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/980" class=".btn">#980</a>
            </td>
            <td>
                <b>
                    feat: agent mediation role
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add mediationRole property to AgentConfig to ensure MediatorModule is initialized correctly. This prevents concurrency issues when multiple attempts to create a mediatorRoutingRecord fail.

Signed-off-by: Niall Shaw <niall.shaw@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-10 14:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/979" class=".btn">#979</a>
            </td>
            <td>
                <b>
                    feat: add present proof v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is essentially a three-way merge of

feat/ppv2
0.3.0-pre
TimoGlastra/refactor/generalize-proofs


BREAKING CHANGE: the present proof module has been extended to support both v1 and v2 of protocol. See [Migrating from AFJ 0.2.x to 0.3.0](https://github.com/hyperledger/aries-framework-javascript/blob/main/docs/migration/0.2-to-0.3.md) for a detailed migration instructions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-09 11:38:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/976" class=".btn">#976</a>
            </td>
            <td>
                <b>
                    chore: add maintainers.md file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #973

﻿Signed-off-by: Timo Glastra <timo@animo.id>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-08 11:40:01 +0000 UTC
    </div>
</div>

