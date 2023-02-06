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
                PR <a href="https://github.com/hyperledger/fabric/pull/3994" class=".btn">#3994</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: e2e again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: e2e again


#### Related issues

Epic: https://github.com/hyperledger/fabric/issues/3511
Issue: https://github.com/hyperledger/fabric/issues/3515

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-06 08:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3993" class=".btn">#3993</a>
            </td>
            <td>
                <b>
                    Orderer v3: Remove system channel usage from integration tests: raft no.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: Ie801bbf66b5ae320fbb1f8a099f1cc4b2070ec94

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: Remove system channel usage from integration tests: raft no.2

#### Related issues
Epic: https://github.com/hyperledger/fabric/issues/3511
Issue: https://github.com/hyperledger/fabric/issues/3515

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-05 16:42:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3991" class=".btn">#3991</a>
            </td>
            <td>
                <b>
                    Expedite purge private data integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Combine purge private data tests into a single 'It' to improve speed (18 minutes to 5 minutes).
This will remove the excessive network teardowns, network builds, and chaincode deployments.
Also remove unneccessary delays and redundant ledger entries.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-04 21:15:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3990" class=".btn">#3990</a>
            </td>
            <td>
                <b>
                    Fix Makefile did't delete docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Because multi-architecture docker image patches removed tags from the docker image, the docker-clean target could not remove the docker image. This patch changes the docker-clean target to remove untagged docker images.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-03 00:52:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3989" class=".btn">#3989</a>
            </td>
            <td>
                <b>
                    fix(sec): upgrade github.com/opencontainers/runc to 1.1.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### What happened？
There are 1 security vulnerabilities found in github.com/opencontainers/runc v1.0.0-rc8
- [CVE-2022-29162](https://www.oscs1024.com/hd/CVE-2022-29162)


### What did I do？
Upgrade github.com/opencontainers/runc from v1.0.0-rc8 to 1.1.2 for vulnerability fix

### What did you expect to happen？
Ideally, no insecure libs should be used.

### The specification of the pull request
[PR Specification](https://www.oscs1024.com/docs/pr-specification/) from OSCS
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 14:03:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3988" class=".btn">#3988</a>
            </td>
            <td>
                <b>
                    Fix chaincode interest for private data purge (backport #3986)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3986 done by [Mergify](https://mergify.com).


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
        Created At 2023-02-02 13:12:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3986" class=".btn">#3986</a>
            </td>
            <td>
                <b>
                    Fix chaincode interest for private data purge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Gateway was not calculating chaincode interest correctly for purge private data calls, since writeset metadata was not being added for purge calls.
The collection level endorsement policies will now be honored instead of defaulting to the chaincode level endorsement policy.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 22:44:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3977" class=".btn">#3977</a>
            </td>
            <td>
                <b>
                    Move purge private data tests to separate runner
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 10:22:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3975" class=".btn">#3975</a>
            </td>
            <td>
                <b>
                    Add BFT support to gateway
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Extend the gateway Submit() logic to concurrently send transaction to all available orderers if the channel is configured to use BFT ordering service.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 16:01:12 +0000 UTC
    </div>
</div>

