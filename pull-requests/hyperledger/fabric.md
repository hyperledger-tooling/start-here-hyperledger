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
                PR <a href="https://github.com/hyperledger/fabric/pull/4578" class=".btn">#4578</a>
            </td>
            <td>
                <b>
                    Directly check the return error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I1138688b89200c6bcb0b18f854c46f03815ad15d

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The patchset simplifies the code by directly checking the return error,
    which follows the Go style.

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
        Created At 2023-12-15 22:41:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4577" class=".btn">#4577</a>
            </td>
            <td>
                <b>
                    Private data purge test improvements - release-2.5 backport
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport private data purge test improvements to release-2.5.
This should resolve the flake failures in release-2.5 branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-15 19:14:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4576" class=".btn">#4576</a>
            </td>
            <td>
                <b>
                    Add doc links to chaincode access control
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add doc links to chaincode access control in the private data doc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-14 14:41:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4575" class=".btn">#4575</a>
            </td>
            <td>
                <b>
                    Revert image FABRIC_CFG_PATH to /etc/hyperledger/fabric (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The updated image for v2.5 release set FABRIC_CFG_PATH to /var/hyperledger/fabric/config.

Historically the value has been /etc/hyperledger/fabric, and it is more typical for configs to exist in /etc than /var.

Additionally the code defaults to /etc/hyperledger/fabric and the docs still mention /etc/hyperledger/fabric, therefore this commit sets it back to /etc/hyperledger/fabric.

Ultimately, it shouldn't really matter since the core.yaml and orderer.yaml are copied to FABRIC_CFG_PATH, and the executables reference the configs using FABRIC_CFG_PATH. So the change is a noop at runtime, but better to get the image back to consistency with the code, docs, and historical precedents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 18:00:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4574" class=".btn">#4574</a>
            </td>
            <td>
                <b>
                    Revert image FABRIC_CFG_PATH to /etc/hyperledger/fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The updated image for v2.5 release set FABRIC_CFG_PATH to /var/hyperledger/fabric/config.

Historically the value has been /etc/hyperledger/fabric, and it is more typical for configs to exist in /etc than /var.

Additionally the code defaults to /etc/hyperledger/fabric and the docs still mention /etc/hyperledger/fabric, therefore this commit sets it back to /etc/hyperledger/fabric.

Ultimately, it shouldn't really matter since the core.yaml and orderer.yaml are copied to FABRIC_CFG_PATH, and the executables reference the configs using FABRIC_CFG_PATH. So the change is a noop at runtime, but better to get the image back to consistency with the code, docs, and historical precedents.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 17:57:32 +0000 UTC
    </div>
</div>

