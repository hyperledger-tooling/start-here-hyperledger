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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4362" class=".btn">#4362</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.7 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.7.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 20:30:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4361" class=".btn">#4361</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.7 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.7.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 20:30:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4360" class=".btn">#4360</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.20.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.20.7.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 18:59:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4359" class=".btn">#4359</a>
            </td>
            <td>
                <b>
                    docs: fix link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a cherry-pick of this PR:
https://github.com/hyperledger/fabric-docs-i18n/pull/816

#### Type of change

- Documentation update

#### Description

There is a double paren when there should be a single paren, which breaks a link

#### Additional details

#### Related issues

#### Release Note

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-10 14:23:48 +0000 UTC
    </div>
</div>

