---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/314" class=".btn">#314</a>
            </td>
            <td>
                <b>
                    Remove dependence of aries module on VcxStateType
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-01 18:18:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/313" class=".btn">#313</a>
            </td>
            <td>
                <b>
                    Update version of libc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 17:01:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/312" class=".btn">#312</a>
            </td>
            <td>
                <b>
                    Remove unncesessary deps from agency client
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslavkovar@protonmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 10:37:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/310" class=".btn">#310</a>
            </td>
            <td>
                <b>
                    Try to fix occasionally failing integration test.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span><span class="chip">hotfix</span><span class="chip">tests</span>
            </td>
            <td>
                The test `test_create_credential_works_twice` occasionally fails in CI - never run into this issue locally. The CI failure of this test is such that the second of creating the same credential definition passes, while it's expected to fail. I think the reason is  that probably on the second attempt, the created credential definition is not yet fully propagated through the pool, and so it appears like the credential definition doesn't exist yet. 
This PR add timeout into the test between first and second attempt to create the same cred. definition.

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-29 08:10:05 +0000 UTC
    </div>
</div>

