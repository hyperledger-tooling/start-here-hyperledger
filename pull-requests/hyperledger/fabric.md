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
                PR <a href="https://github.com/hyperledger/fabric/pull/3429" class=".btn">#3429</a>
            </td>
            <td>
                <b>
                    Fix some errors in the tutorial
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

- Documentation update

#### Description

This is a backport of the commit 318510f80a to release-2.2.

Signed-off-by: Satoshi Ito <satoshi.ito.tf@hitachi.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-19 04:15:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3428" class=".btn">#3428</a>
            </td>
            <td>
                <b>
                    Update doc CouchDB links to 3.2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Address comments from release-2.4 PR.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 16:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3427" class=".btn">#3427</a>
            </td>
            <td>
                <b>
                    new caas page (backport #3329)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3329 done by [Mergify](https://mergify.com).


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
        Created At 2022-05-17 18:39:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3426" class=".btn">#3426</a>
            </td>
            <td>
                <b>
                    New Block Attestation Orderer GRPC service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- New feature

#### Description
New RPC service for block attestation is added. It will be used by BFT block replication

#### Related issues
#3413 

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-17 10:20:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3424" class=".btn">#3424</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix code issues from the updated staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 20:03:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3423" class=".btn">#3423</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.18.2 (release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update staticcheck to a version that works with Go 1.18.
Fix code issues with the new staticcheck.
Fix unit test for new TLS messages and assertion changes in Go 1.18.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 19:45:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3420" class=".btn">#3420</a>
            </td>
            <td>
                <b>
                    Log proposal response differences
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the gateway, if proposal responses from different endorsing peers don’t match, then it’s very difficult for the end user to diagnose why.  This commit adds extra logging to help identify the cause of the mismatch.

If the log level is set to ‘debug’ for the ‘gateway’, then the proposal response payloads are unmarshalled and analysed to log specific differences between individual key/values in the read/write sets, SBE policy write differences, event differences and chaincode response differences.  For private collections, only the hashes are logged if they are different.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 12:06:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3418" class=".btn">#3418</a>
            </td>
            <td>
                <b>
                    Fix mistake change 'curl' to 'git'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-14 14:23:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3408" class=".btn">#3408</a>
            </td>
            <td>
                <b>
                    Fix doc to handle $PWD containing whitepaces (backport #2298)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A backport of pull requset #2298

Note: the file `docs/source/peer-chaincode-devmode.md` does not exist in release-2.2, so I deleted it from the commit.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 14:39:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3406" class=".btn">#3406</a>
            </td>
            <td>
                <b>
                    Update README build badge link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 13:18:43 +0000 UTC
    </div>
</div>

