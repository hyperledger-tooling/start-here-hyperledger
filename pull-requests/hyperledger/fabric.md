---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2601" class=".btn">#2601</a>
            </td>
            <td>
                <b>
                    Maintain order of transactions in the commit notification
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Maintain order of transactions in the commit notification so the gateway can deliver the clients the chaincode events in the same and consistent order.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 18:21:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2599" class=".btn">#2599</a>
            </td>
            <td>
                <b>
                    FABGW-18: Fix concurrency issue in commit notifier close
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This code path should only be executed if the ledger notifications stop, which is never expected to happen at runtime. However, it does happen within the unit tests could cause an intermittent test failure.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 15:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2598" class=".btn">#2598</a>
            </td>
            <td>
                <b>
                    Bump vmImage to Ubuntu-20.04
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Just keeping up with latest deps

Signed-off-by: Brett Logan <lindluni@github.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 13:40:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2597" class=".btn">#2597</a>
            </td>
            <td>
                <b>
                    FAB-18472 Fix unit test hang when using softhsm 2.6.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Stop the unit tests from hanging when running the pkcs11 unit tests
with softhsm 2.6.1 on linux

Signed-off-by: D <d_kelsey@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-18 11:06:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2596" class=".btn">#2596</a>
            </td>
            <td>
                <b>
                    Govendor added to documentation (backport #2588)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2588 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 21:44:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2595" class=".btn">#2595</a>
            </td>
            <td>
                <b>
                    Govendor added to documentation (backport #2588)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2588 done by [Mergify](https://mergify.io).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.io/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.io/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.io/
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-17 21:43:46 +0000 UTC
    </div>
</div>

