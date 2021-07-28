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
                PR <a href="https://github.com/hyperledger/fabric/pull/2796" class=".btn">#2796</a>
            </td>
            <td>
                <b>
                    Update doc for default chaincode instantiation policy (release-1.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update doc to indicate that default chaincode instantiation policy
is any channel admin.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 20:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2795" class=".btn">#2795</a>
            </td>
            <td>
                <b>
                    [FAB-18530] fix: add validation for chaincode name when packaging chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: ankitm123 <ankitmohapatra123@gmail.com>


#### Type of change
- Bug fix

#### Description
I am able to package and install chaincode with names which are not valid,
```
peer lifecycle chaincode package cc_1.0.0.tar.gz --path ../../fabric-chaincode-poc --lang golang --label cc_1.0.0_1.0
+ res=0
Chaincode is packaged
Installing chaincode on peer0.org1...
Using organization 1
peer lifecycle chaincode install cc_1.0.0.tar.gz
+ res=0
2021-07-27 12:16:13.991 EDT [cli.lifecycle.chaincode] submitInstallProposal -> INFO 001 Installed remotely: response:<status:200 payload:"\nMcc_1.0.0_1.0:5e0f5e9f4e8bc50706a74ac24ba855bcf267c469d1931812b9f5a80381d4f035\022\014cc_1.0.0_1.0" > 
2021-07-27 12:16:13.991 EDT [cli.lifecycle.chaincode] submitInstallProposal -> INFO 002 Chaincode code package identifier: cc_1.0.0_1.0:5e0f5e9f4e8bc50706a74ac24ba855bcf267c469d1931812b9f5a80381d4f035
Chaincode is installed on peer0.org2
```
but then it fails during approval (with the message mentioned in the issue):
```
+ peer lifecycle chaincode approveformyorg -o localhost:7050 --ordererTLSHostnameOverride orderer.example.com --tls --cafile /home/ankitm123/work/fabric-samples/test-network/organizations/ordererOrganizations/example.com/orderers/orderer.example.com/msp/tlscacerts/tlsca.example.com-cert.pem --channelID mychannel --name cc_1.2.3 --version 1.0 --package-id cc_1.2.3_1.0:81221a01ec04a1e2502d5b2746d0a047619878fca818b9894c6a15f366254e42 --sequence 1
+ res=1
Error: proposal failed with status: 500 - failed to invoke backing implementation of 'ApproveChaincodeDefinitionForMyOrg': error validating chaincode definition: invalid chaincode name 'cc_1.2.3'. Names can only consist of alphanumerics, '_', and '-' and can only begin with alphanumerics
```
I think chaincode name should be validated as early as `peer lifecycle chaincode package`.

This PR adds a `--name` flag to the package subcommand, and validates that the provided name is valid.


#### Additional details

After this change:
```
➜  test-network git:(main) peer lifecycle chaincode package cc_1.1.tar.gz --path ../../fabric-chaincode-poc --lang golang --label cc_1.1.0  
Error: chaincode name must be specified

➜  test-network git:(main) peer lifecycle chaincode package cc_1.tar.gz --path ../../fabric-chaincode-poc --lang golang --label cc_1.1.0 --name cc_1.0.0
Error: invalid chaincode name 'cc_1.0.0'. Names can only consist of alphanumerics, '_', and '-' and can only begin with alphanumerics

➜  test-network git:(main) peer lifecycle chaincode package cc_1.1.tar.gz --path ../../fabric-chaincode-poc --lang golang --label cc_1.1.0 --name cc
```

#### Related issues
https://jira.hyperledger.org/browse/FAB-18530
https://jira.hyperledger.org/browse/FAB-18409

#### Release Note




            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 20:14:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2793" class=".btn">#2793</a>
            </td>
            <td>
                <b>
                    [FAB-11334] Adds a viper Cmd to unjoin a peer from a channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change adds a Viper cobra.Command to unjoin the peer from a specified channel.

Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- New feature

#### Description

This PR introduces a `node unjoin` cobra.Cmd to the peer binary.  When enjoining a channel, the peer must be shut down, and the command will scrub all channel artifacts from the kvledger and transient storage.   If a crash occurs during the removal of the ledger, the residual artifacts will be scrubbed at the next launch of the peer. 

#### Additional details

PR #2769 
PR #2754 
PR #2732 

#### Related issues

[FAB-16035](https://jira.hyperledger.org/browse/FAB-16035)
[FAB-4481](https://jira.hyperledger.org/browse/FAB-4481)
[FAB-17787](https://jira.hyperledger.org/browse/FAB-17787)
[FAB-17801](https://jira.hyperledger.org/browse/FAB-17801)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 11:56:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2784" class=".btn">#2784</a>
            </td>
            <td>
                <b>
                    FAB-18067 Discovery support Implicit Collections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Implemented the fix as suggested by Yacov in his Jira comment.

Verified the fix works against the asset-transfer-secured-agreement sample which uses implicit collections.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-26 12:21:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2783" class=".btn">#2783</a>
            </td>
            <td>
                <b>
                    Update to latest major version of Go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Brett Logan <lindluni@github.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-24 23:40:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2780" class=".btn">#2780</a>
            </td>
            <td>
                <b>
                    FAB 18365 IT flake evictionsuspector failed to read eviction 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Description
In failing case, the OSN being removed has committed the config change but failed to receive apply_config msg to halt the chain. This state is defined to be handled as part of the eviction suspicion logic. But it failed when evictionsuspector failed to check from lastconfig block if chain is up-to-date. 

Fix: Updated the order of statements which looks at the latest config block and block height validation.

#### Type of change
- Bug fix

Signed-off-by: Parameswaran Selvam <parselva@in.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-23 11:02:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2779" class=".btn">#2779</a>
            </td>
            <td>
                <b>
                    Hardening raft catchup IT
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
        Created At 2021-07-22 23:42:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2778" class=".btn">#2778</a>
            </td>
            <td>
                <b>
                    Merge and enhance coding guidelines across github and wiki
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enhances and merges the additional coding guidelines present in the [wiki page](https://wiki.hyperledger.org/display/fabric/Coding+Guidelines) into the coding guidelines page maintained in the docs at github.

Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 22:43:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2776" class=".btn">#2776</a>
            </td>
            <td>
                <b>
                    Update private data docs - remove SDK reference (backport #2770)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2770 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-22 17:34:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2775" class=".btn">#2775</a>
            </td>
            <td>
                <b>
                    Additional documentation for implicit private data collections (backport #2772)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2772 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-22 16:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2774" class=".btn">#2774</a>
            </td>
            <td>
                <b>
                    Additional documentation for implicit private data collections (backport #2772)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #2772 done by [Mergify](https://mergify.io).


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
        Created At 2021-07-22 16:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2773" class=".btn">#2773</a>
            </td>
            <td>
                <b>
                    FABGW-25 Endorse using generated ChaincodeInterest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change the Endorse() method logic as described in the design document attached to the Jira.
- Process proposal on local org peer.
- Using the ChaincodeInterest in the propsal response, invoke discovery to obtain a layout that contains the local org
- Obtain the remaining endorsements
- Build the transaction to send back to the client.

Extra unit tests added to test the new logic.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 13:07:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2772" class=".btn">#2772</a>
            </td>
            <td>
                <b>
                    Additional documentation for implicit private data collections
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">doc-merge</span>
            </td>
            <td>
                Add additional documentation for implicit private data collections.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 11:32:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2771" class=".btn">#2771</a>
            </td>
            <td>
                <b>
                    FABGW-25 Test for system chaincode
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit addresses the closing comments in PR #2767:

- Skip systems chaincode in this block as well
- Add a test that asserts that the system chaincodes are indeed skipped

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-22 08:59:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2770" class=".btn">#2770</a>
            </td>
            <td>
                <b>
                    Update private data docs - remove SDK reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove reference to SDK since SDK is no longer used to deploy chaincode.
Also remove reference to legacy lifecycle (legacy lifecycle
remains fully documented in release-1.4 docs and in the main branch CLI reference doc).

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-21 23:09:14 +0000 UTC
    </div>
</div>

