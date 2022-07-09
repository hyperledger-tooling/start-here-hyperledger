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
                PR <a href="https://github.com/hyperledger/fabric/pull/3519" class=".btn">#3519</a>
            </td>
            <td>
                <b>
                    fix(security): Path Traversal Bug
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unsanitized input from open tar file flows into os.Open, where it is used as a path. This may result in a Path Traversal vulnerability and allow an attacker to open arbitrary files.

primary changes :
	1.updates to archive.go

Signed-off-by: Bhaskar <ram@hacker.ind.in>

- Bug fix
- Improvement (improvement to code, performance, etc)

#### Description

Unsanitized input from open tar file flows into os.Open, where it is used as a path. This may result in a Path Traversal vulnerability and allow an attacker to open arbitrary files.

## Data flow:
22 steps in 1 file
vendor/github.com/docker/docker/pkg/archive/diff.go
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-09 14:44:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3517" class=".btn">#3517</a>
            </td>
            <td>
                <b>
                    Updates in main for Fabric CA release v1.5.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Josh Kneubuhl <jkneubuh@us.ibm.com>

#### Type of change

- Documentation update

#### Description

This PR updates the documentation and client installation scripts to install the fabric CA v1.5.5 release binaries.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 12:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3516" class=".btn">#3516</a>
            </td>
            <td>
                <b>
                    Update gateway.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Correct some typos

Signed-off-by: Muhammad Reza Z'aba <muhdreza@gmail.com>

#### Type of change
- Documentation update
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 03:27:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3508" class=".btn">#3508</a>
            </td>
            <td>
                <b>
                    Correct typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Correct some typos in the documentation

Signed-off-by: mrzgh <muhdreza@gmail.com>

#### Type of change

- Documentation update

#### Description

Correct some typos in the documentation.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-06 03:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3506" class=".btn">#3506</a>
            </td>
            <td>
                <b>
                    fix some typos
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
        Created At 2022-07-05 12:14:55 +0000 UTC
    </div>
</div>

