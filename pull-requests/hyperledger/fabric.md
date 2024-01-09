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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4595" class=".btn">#4595</a>
            </td>
            <td>
                <b>
                    Upgrade the CouchDB used to v3.3.3 as per CVE-2023-45725.
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

Move to CouchDB v3.3.3.  There's a [security vulnerability](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-45725) with CouchDB v3.3.2.  I **think** this only impacts the testing that happens to Fabric, but this PR is a good way to be sure.

#### Additional details

I have tested that CouchDB v3.3.3 is not majorly functionally different than CouchDB v3.3.2. (See its [Release Notes](https://docs.couchdb.org/en/stable/whatsnew/3.3.html#release-3-3-3)).  There have been no breaking API changes in v3.3.3, only bug fixes and security patches.

I would suggest backporting this to Fabric v2.5.x because it's only a CouchDB Patch.

#### Related issues

Tracked by https://github.com/hyperledger/fabric/issues/4594
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 15:34:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4592" class=".btn">#4592</a>
            </td>
            <td>
                <b>
                    Extend _lifecycle functions to query all approved chaincode definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch updates some _lifecycle functions on queryapproved to query all approved chaincode definitions.
See https://github.com/hyperledger/fabric/issues/4564 for the detail.

#### Type of change

- New feature

#### Description

As a sub-task stemming from issue #4564, this updates some _lifecycle functions on queryapproved to query all approved chaincode definitions.

Once this patch is merged, I will submit a patch to enhance the command:

#### Addtional Details

The example of output when executing the enhanced queryapproved in the provisional implementation:

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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 04:15:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4591" class=".btn">#4591</a>
            </td>
            <td>
                <b>
                    Update smartcontract.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixing link to API in the context of "Smart contracts have many APIs available to them" because it is broken in current version of hyperledger fabric documentation

#### Type of change

- Documentation update

#### Description

Reading documentation, especially the current and release-2.5 version, I noticed that there is a link that leads to nowhere in such versions. It looks like release-2.2 had the linked documentation but it no longer exists. I tried to find the best replacement from the existing documentation for the previously linked and made such changes.

#### Additional details

N/A

#### Related issues

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 02:24:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4590" class=".btn">#4590</a>
            </td>
            <td>
                <b>
                    fix error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #4589

Analysed recent errors in gatway integration tests. There is one error everywhere (I hope it is the last one). 
The problem is that after restarting orderer2 peer did not manage to reconnect to it because of backoff timeout.
I studied the logs and made it so that we don't send Submit until the peer connects to orderer2.

The mechanics of waiting are as follows:
- looking for a string similar to "pickfirstBalancer: UpdateSubConnState: 0xc0006b4210, {TRANSIENT_FAILURE connection error: desc = "transport: Error while dialing: dial tcp 127.0.0.1:22005""
- I get the address "0xc0006b4210" from the line.
- I move the peer log cursor to the end.
- After restarting the peer, I expect the line "0xc0006b4210, {READY". This is a part of the line pickfirstBalancer: UpdateSubConnState: 0xc0006b4210, {READY <nil>} - a sign that the connection is restored

For a test this is ok, but maybe in real work it will not work. Then I suggest someone to modify the file `github.com/hyperledger/fabric/internal/pkg/gateway/registry.go` . When selecting connections orderers should check the connection status and reconnect violently if necessary.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 21:42:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4588" class=".btn">#4588</a>
            </td>
            <td>
                <b>
                    Validate the request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset adds validation to the request before using it.

Change-Id: Ic6a7a65d6da289d84fe82c3f6e048e396b1f1a0e

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset adds validation to the request before using it.

This can help protect from malformed request.


#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-03 22:04:07 +0000 UTC
    </div>
</div>

