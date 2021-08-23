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
                PR <a href="https://github.com/hyperledger/fabric/pull/2850" class=".btn">#2850</a>
            </td>
            <td>
                <b>
                    Update Go to v1.16.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update Go to v1.16.7.
Go module support is assumed starting in Go v1.16.
Therefore, for chaincodes without go modules (such as in the integration tests),
need to explicitly set GO111MODULE to off otherwise chaincode will not compile.
See Go v1.16 release notes for more details: https://golang.org/doc/go1.16#go-command

As part of troubleshooting the Go upgrade, also added debug for the chaincode
compile command.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-23 12:16:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2849" class=".btn">#2849</a>
            </td>
            <td>
                <b>
                    Options for GRPC message size configurable (backport #2805) 2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #2805

Signed-off-by: Parameswaran Selvam parselva@in.ibm.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-22 14:40:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2848" class=".btn">#2848</a>
            </td>
            <td>
                <b>
                    Options for GRPC message size configurable (backport #2805) 2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of pull request #2805

Signed-off-by: Parameswaran Selvam parselva@in.ibm.com
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-21 15:23:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2847" class=".btn">#2847</a>
            </td>
            <td>
                <b>
                    [FAB-11334] - Adds a functional / integration test for peer unjoin 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This integration test launches the peer unjoin command, simulating normal operation and some error / negative test cases.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change
- Test update

#### Description

This integration test targets the `peer node unjoin` CLI, both with positive and negative examples: 

- checks for error when unjoining a channel while the peer is running.
- checks for double-unjoin (unjoin unjoined)
- checks for partial unjoin:  If the unjoin fails, the next peer restart will attempt to resume the ledger purge.
- checks for normal unjoin

#### Related issues


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 15:53:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2845" class=".btn">#2845</a>
            </td>
            <td>
                <b>
                    Gateway Evaluate() with transient data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add protection logic to ensure sensitive transient data is not unintentionally leaked to other org’s peers when evaluating transaction proposal.
If transient data is present and target_organizations is not specified, send request only to a local peer, or fail if one is not available for that channel/chaincode

resolves #2841 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-19 15:31:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2844" class=".btn">#2844</a>
            </td>
            <td>
                <b>
                    FAB-18529 added null check in channel header parsing (backport #2838)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2838 done by [Mergify](https://mergify.io).


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
        Created At 2021-08-19 13:10:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2843" class=".btn">#2843</a>
            </td>
            <td>
                <b>
                    FAB-18529 added null check in channel header parsing (backport #2838)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2838 done by [Mergify](https://mergify.io).


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
        Created At 2021-08-19 13:10:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2839" class=".btn">#2839</a>
            </td>
            <td>
                <b>
                    Add documentation for AbsoluteMaxBytes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Document AbsoluteMaxBytes channel config relation to gRPC limits.
Also replace orderer Addresses with org OrdererEndpoints in the channel config documentation (recommended since v1.4.2).

Closes #2820.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 20:34:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2838" class=".btn">#2838</a>
            </td>
            <td>
                <b>
                    FAB-18529 added null check in channel header parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Bug fix

#### Description
Fuzz testing has reported SEGV while sending incomplete/null
message request to orderer.  When the submit request payload
is null, the orderer fails with SEGV while trying to parse/read 
the channel header.

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 15:19:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2837" class=".btn">#2837</a>
            </td>
            <td>
                <b>
                    Update bootstrap.sh download script for Fabric CA v1.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update bootstrap.sh download script for Fabric CA v1.5.1

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-18 12:21:39 +0000 UTC
    </div>
</div>

