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
                PR <a href="https://github.com/hyperledger/fabric/pull/4603" class=".btn">#4603</a>
            </td>
            <td>
                <b>
                    Enhance queryapproved cmd to query all approved chaincode definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enhances queryapproved command to query all approved chaincode definitions.
See https://github.com/hyperledger/fabric/issues/4564 for the detail.

Also, this fixes an unstable test code on _lifecycle functions on queryapproved to query all approved chaincode definitions.

#### Type of change

- New feature
- Bug fix

#### Description

As a sub-task stemming from issue #4564, this enhances queryapproved command to query all approved chaincode definitions.
Also, this fixes an unstable test code on _lifecycle functions on queryapproved to query all approved chaincode definitions.

Once this patch is merged, I will submit patches to update the documantations:


#### Addtional Details

The example of output when executing the enhanced queryapproved in the implementation:

```
$ peer lifecycle chaincode queryapproved -C mychannel
Approved chaincode definition on channel 'mychannel':
name: basic2, sequence: 2, version: 1.0.1, init-required: false, package-id: basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a, endorsement plugin: escc, validation plugin: vscc
name: basic, sequence: 1, version: 1.0.1, init-required: false, package-id: basic_1.0.1:f4babb5fd92c0ab4bce8c6ac30ca7bbb4a55e6c37774582d11639b6036ae0273, endorsement plugin: escc, validation plugin: vscc
name: basic2, sequence: 1, version: 1.0.1, init-required: false, package-id: basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a, endorsement plugin: escc, validation plugin: vscc
```

```
 $ peer lifecycle chaincode queryapproved -C mychannel -O json
{
        "approved_chaincode_definitions": [
                {
                        "name": "basic2",
                        "sequence": 2,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a"
                                        }
                                }
                        }
                },
                {
                        "name": "basic",
                        "sequence": 1,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic_1.0.1:f4babb5fd92c0ab4bce8c6ac30ca7bbb4a55e6c37774582d11639b6036ae0273"
                                        }
                                }
                        }
                },
                {
                        "name": "basic2",
                        "sequence": 1,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a"
                                        }
                                }
                        }
                }
        ]
}
```

#### Releated PRs

- https://github.com/hyperledger/fabric-protos/pull/196
- https://github.com/hyperledger/fabric/pull/4592


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 10:14:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4602" class=".btn">#4602</a>
            </td>
            <td>
                <b>
                    added time to the test to make it long enough
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
        Created At 2024-01-10 05:32:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4601" class=".btn">#4601</a>
            </td>
            <td>
                <b>
                    Upgrade the CouchDB used to v3.3.3 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to CouchDB v3.3.3.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 14:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4600" class=".btn">#4600</a>
            </td>
            <td>
                <b>
                    Upgrade the CouchDB used to v3.3.3 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to CouchDB v3.3.3.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 14:18:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4599" class=".btn">#4599</a>
            </td>
            <td>
                <b>
                    Fix doc typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix remaining doc typo from prior commit.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 14:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4598" class=".btn">#4598</a>
            </td>
            <td>
                <b>
                    docs: fix typos (backport release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs: fix typos
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 13:29:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4597" class=".btn">#4597</a>
            </td>
            <td>
                <b>
                    docs: fix typos
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
        Created At 2024-01-09 08:57:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4596" class=".btn">#4596</a>
            </td>
            <td>
                <b>
                    find and fix error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Often fails this [test](https://github.com/hyperledger/fabric/blob/main/integration/raft/config_test.go#L1258) 
- https://github.com/hyperledger/fabric/actions/runs/7493668256/job/20399967195
- https://github.com/hyperledger/fabric/actions/runs/7483402876/job/20368656381
- https://github.com/hyperledger/fabric/actions/runs/7462441029/job/20304890927

Failure occurs when [waiting for the orderer to delete a channel](https://github.com/hyperledger/fabric/blob/main/integration/raft/config_test.go#L1336) 

[Here is an explanation](https://github.com/hyperledger/fabric/blob/main/integration/raft/config_test.go#L1314): why they added the removal of the channel with orderer

I'll describe what's going on:
- the orderer is in a constant cycle periodically performing the [function](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L339)
- send a command to remove channel. It passes the following functions [serveRemove](https://github.com/hyperledger/fabric/blob/main/orderer/common/channelparticipation/restapi.go#L360), [RemoveChannel](https://github.com/hyperledger/fabric/blob/main/orderer/common/multichannel/registrar.go#L769) (`r.lock` monopole is taken in this function), [Halt](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L226) (the actual removal of the channel is expected [here](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L228))
- let's return to the main loop, this is where the actual deletion should take place, it wants to execute the function [SwitchFollowerToChain](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L357), but she can't, she needs a `r.lock` monopole.

==================================

The error in the raft tests is due to the struggle for monopoly control of r.lock in the SwitchChainToFollower and RemoveChannel functions.

RemoveChannel grabs monopoly control and waits for the channel to terminate. During termination, SwitchChainToFollower tries to grab monopoly control and fails.

Here is my variant of solving the error. If someone suggests a more correct and reddish way, it would be great.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 17:23:07 +0000 UTC
    </div>
</div>

