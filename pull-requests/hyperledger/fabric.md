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
                PR <a href="https://github.com/hyperledger/fabric/pull/3230" class=".btn">#3230</a>
            </td>
            <td>
                <b>
                    doc - add new gateway to key concepts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Horton <joshh@us.ibm.com>

#### Type of change

- Documentation update

#### Description

New Fabric Gateway service page needed a link in Key Concepts page / list
(gateway.md)

#### Additional details

Add to go here near the bottom (logical sequential) - https://hyperledger-fabric.readthedocs.io/en/latest/key_concepts.html


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-15 19:42:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3229" class=".btn">#3229</a>
            </td>
            <td>
                <b>
                    Fix inconsistent behavior of GetBookmarkAndClose method in different statedb
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

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description

<!--- Describe your changes in detail, including motivation. -->
When there are no more results in paginated range query, statecouchdb return endKey
as bookmark in GetBookmarkAndClose method, but stateleveldb return empty string as bookmark.
This inconsistent behavior may cause different code logic when use bookmark in smart contract
with different statedb.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 10:22:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3226" class=".btn">#3226</a>
            </td>
            <td>
                <b>
                    Add Intermediate CA certs to dial options (backport #3225)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3225 done by [Mergify](https://mergify.com).


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
        Created At 2022-02-11 16:21:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3225" class=".btn">#3225</a>
            </td>
            <td>
                <b>
                    Add Intermediate CA certs to dial options
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The gateway was omitting to include TLS intermediate certificates in the dial options when connecting to other nodes.
This commit appends them to the splice of root certs in the endpoint config.

Resolves #3224 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 11:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3222" class=".btn">#3222</a>
            </td>
            <td>
                <b>
                    Filter out purged data from private data store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Description
This PR  introduces support for the purge marker(s) and filters the data marked for purging. In addition, this PR removes the 
unused code for V11 format as now we upgraded data format along with retroactively creating hashed index at peer start.

#### Related issues
Resolves #3028 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 14:07:19 +0000 UTC
    </div>
</div>

