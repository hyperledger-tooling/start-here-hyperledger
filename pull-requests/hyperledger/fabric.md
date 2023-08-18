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
                PR <a href="https://github.com/hyperledger/fabric/pull/4378" class=".btn">#4378</a>
            </td>
            <td>
                <b>
                    fix warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Leading whitespaces before Go directives in comments.
- Incorrect usages of fmt.Printf, fmt.Println, and similar formatting and printing functions.
- Redundant parentheses in expressions and types.
- Types in variable and constant declarations that can be omitted since they can be inferred by the compiler. Such types are redundant, omitting them may improve readability of the code.
- Type conversions that may be omitted.
- Aliases of imported packages that may be omitted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 16:18:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4374" class=".btn">#4374</a>
            </td>
            <td>
                <b>
                    Add readthedocs config file (backport #4366)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4366 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 14:43:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4373" class=".btn">#4373</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: delivery client integration
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
Integrate the BFT block deliverer with the deliver client.
If the consensus-type is BFT, the BFTDeliverer is created.

#### Related issues

#4348 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 09:20:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4372" class=".btn">#4372</a>
            </td>
            <td>
                <b>
                    Remove usage of deprecated functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Remove usage of deprecated functions:
- math/rand
- protobuf/proto
- protobuf/ptypes
- grpc
- crypto/x509
- fsouza/go-dockerclient
- net
- grpc/grpclog
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-17 08:49:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4369" class=".btn">#4369</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.21.0
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
        Created At 2023-08-16 22:38:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4368" class=".btn">#4368</a>
            </td>
            <td>
                <b>
                    Remove usage of deprecated ioutil package functions [internal]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go std lib deprecated package ioutils since go ver 1.16, while Fabric still uses it in several places. This commit continues (https://github.com/hyperledger/fabric/pull/4367) to remove usage of ioutils from the internal package.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 22:23:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4367" class=".btn">#4367</a>
            </td>
            <td>
                <b>
                    Remove usage of deprecated ioutil package functions [ledger]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Go std lib deprecated package ioutils since go ver 1.16, while Fabric still uses it in several places. This commit removes usage of ioutils from ledger-related packages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-16 11:51:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4366" class=".btn">#4366</a>
            </td>
            <td>
                <b>
                    Add readthedocs config file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add readthedocs config file.

For more background see https://blog.readthedocs.com/migrate-configuration-v2/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 16:04:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4365" class=".btn">#4365</a>
            </td>
            <td>
                <b>
                    BFT Block Puller: BFTDeliverer
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

- A BFTDeliverer that fetches blocks using a block receiver and maintains a BFTCensorshipMonitor.
- Abstract the creation of a BFTCensorshipMonitor via an abstract factory, so that we can use a mock for it in testing.
- Add a "ShuffledEndpoints" method to the connection source and test it. 
- Unit testing of BFTDeliverer.

#### Related issues

#4348 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 10:18:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4364" class=".btn">#4364</a>
            </td>
            <td>
                <b>
                    invalid identity error="MSP \"Org3MSP\" is not defined on channel"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                see https://github.com/hyperledger/fabric/issues/4358

Type of change
Documentation update
Description
specifying a CORE_PEER_LOCALMSPID with quotation marks leads to misleading error message =>

Error: proposal failed (err: rpc error: code = Unknown desc = error validating proposal: access denied: channel [] creator org unknown, creator is malformed)

Related issues
https://github.com/hyperledger/fabric/issues/4358

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 19:46:42 +0000 UTC
    </div>
</div>

