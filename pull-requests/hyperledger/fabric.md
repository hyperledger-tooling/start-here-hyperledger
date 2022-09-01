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
                PR <a href="https://github.com/hyperledger/fabric/pull/3621" class=".btn">#3621</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove kafka from shared config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I1aefd584e0217642c1315544da8eb1e1849ec759

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Remove kafka brokers from shared config

#### Related issues

Issue: #3513 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-01 10:52:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3619" class=".btn">#3619</a>
            </td>
            <td>
                <b>
                    Update release information in readme and docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Clarify that v1.4 is out of maintenance
- Releases are now periodic rather than every four months.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 16:20:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3618" class=".btn">#3618</a>
            </td>
            <td>
                <b>
                    Update proto dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To include SeekContentType in orderer protobuf

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 14:06:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3617" class=".btn">#3617</a>
            </td>
            <td>
                <b>
                    use matrix to avoid copy my self in github action(pipeline as) code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

- use matrix to avoid copy my self in github action(pipeline as) code
- use matrix add binary file compile checking or mac and windows os

#### Additional details

n/A

#### Related issues

n/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-27 15:04:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3615" class=".btn">#3615</a>
            </td>
            <td>
                <b>
                    Fix getting_started doc link (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix doc link issue identified in #3468.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 13:56:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3614" class=".btn">#3614</a>
            </td>
            <td>
                <b>
                    Fix orderer snapshot doc typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix orderer snapshot doc typo identified in #3282.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 13:45:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3612" class=".btn">#3612</a>
            </td>
            <td>
                <b>
                    Fix doc typo.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix doc typo identified in #3177.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 12:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3611" class=".btn">#3611</a>
            </td>
            <td>
                <b>
                    Enable more parallel jobs in github actions (backport #3607)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3607 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 12:47:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3609" class=".btn">#3609</a>
            </td>
            <td>
                <b>
                    Enable more parallel jobs in github actions (backport #3607)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3607 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 12:47:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3608" class=".btn">#3608</a>
            </td>
            <td>
                <b>
                    Enable more parallel jobs in github actions (backport #3607)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3607 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 12:46:52 +0000 UTC
    </div>
</div>

