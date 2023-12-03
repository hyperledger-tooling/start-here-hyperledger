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
                PR <a href="https://github.com/hyperledger/fabric/pull/4562" class=".btn">#4562</a>
            </td>
            <td>
                <b>
                    Added description for indexing CouchDB. (backport #4560)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4560 done by [Mergify](https://mergify.com).


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
        Created At 2023-11-30 19:45:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4561" class=".btn">#4561</a>
            </td>
            <td>
                <b>
                    Migration from Raft to BFT test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Test Improvement 
- Test update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 16:27:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4560" class=".btn">#4560</a>
            </td>
            <td>
                <b>
                    Added description for indexing CouchDB.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Documentation update

#### Description

Added more examples for CouchDB indexing. Explained the possibility of speeding up the query and adding sorting.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-30 13:22:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4559" class=".btn">#4559</a>
            </td>
            <td>
                <b>
                    Removes methods of legacy chaincode lifecycle from nwo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit concludes removal of the legace lifecycle methods from integration tests nwo package.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 22:40:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4558" class=".btn">#4558</a>
            </td>
            <td>
                <b>
                    Raft to BFT migration
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
        Created At 2023-11-28 21:06:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4557" class=".btn">#4557</a>
            </td>
            <td>
                <b>
                    Direct check the value from dict
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The patchset follows golang best practice to simplify the code.

Change-Id: I134babd9cb6bf8f173fd2a891bde06e95c62c76b

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Simplify code by checking dict value directly, aligned with golang best practice.

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
        Created At 2023-11-28 19:44:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4556" class=".btn">#4556</a>
            </td>
            <td>
                <b>
                    Unit tests bv
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Unit tests 

#### Description

This PR aims to provide unit tests for the Block Verification Assistant unit. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-28 12:50:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4555" class=".btn">#4555</a>
            </td>
            <td>
                <b>
                    Remove chaincode deploy legacy from pvt data tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit removes usages of the chaincode legacy deploy code from private data integration tests.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-27 23:24:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4554" class=".btn">#4554</a>
            </td>
            <td>
                <b>
                    Ensure channelID in transaction matches chain instance
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
        Created At 2023-11-27 16:18:15 +0000 UTC
    </div>
</div>

