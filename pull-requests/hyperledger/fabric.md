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
                PR <a href="https://github.com/hyperledger/fabric/pull/3522" class=".btn">#3522</a>
            </td>
            <td>
                <b>
                    Update fabric-chaincode-go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Latest version includes purge private data support

Signed-off-by: James Taylor <jamest@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 15:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3521" class=".btn">#3521</a>
            </td>
            <td>
                <b>
                    WIP: Orderer v3: Kafka integration tests cleanup
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

Clean up kafka related infrastructure from integration tests.

#### Additional details

#### Related issues

Epic: #3511 
Issue: #3513 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 14:51:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3520" class=".btn">#3520</a>
            </td>
            <td>
                <b>
                    WIP: Orderer v3: disable kafka and remove integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: Icba69b9e104377337adefc466745ad5548b4fbab

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

- Disable kafka in server/main by not creating the kafka consenter.

- Remove kafka specific integration tests.

- Move consensus migration tests to raft (solo to raft).

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

Issue: #3513 
Epic: #3511 

#### Release Note
The kafka consensus protocol is no longer supported.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-10 13:31:20 +0000 UTC
    </div>
</div>

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

