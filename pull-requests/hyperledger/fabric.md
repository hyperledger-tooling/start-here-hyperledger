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
                PR <a href="https://github.com/hyperledger/fabric/pull/4553" class=".btn">#4553</a>
            </td>
            <td>
                <b>
                    Remove legacy chaincode deploy from SBE integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes legacy chaincode deploy from being used by SBE integration tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-26 14:11:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4552" class=".btn">#4552</a>
            </td>
            <td>
                <b>
                    Remove deploy legacy from interop integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes DeployChaincodeLegacy usage from the integration interoperability tests, most of the code was removed because with removal of legacy LSCC these are not valid cases any longer.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-23 22:01:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4551" class=".btn">#4551</a>
            </td>
            <td>
                <b>
                    Return the struct directly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I3e1622c0c7ee144c3164cecc49f5cf6d75b9ec32

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

No need to create an empty struct and then fill in the data.

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
        Created At 2023-11-20 22:22:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4550" class=".btn">#4550</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: verifier in the monitor
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

Integration of the stand alone verifier with the censorship monitor.


#### Related issues
#4353 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 16:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4549" class=".btn">#4549</a>
            </td>
            <td>
                <b>
                    migration raft2bft - WIP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test update

#### Description

This PR aims to update the migration test. The goal is to migrate from Raft to BFT.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-20 10:00:26 +0000 UTC
    </div>
</div>

