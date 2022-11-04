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
                PR <a href="https://github.com/hyperledger/fabric/pull/3765" class=".btn">#3765</a>
            </td>
            <td>
                <b>
                    Add private write-set for purge operation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds a private write-set for a purge operation. The private write-set contains the delete operation on the key getting purged.

Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature

#### Related issues
Closes #3761 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-03 20:26:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3762" class=".btn">#3762</a>
            </td>
            <td>
                <b>
                    Commit path changes for private data purge (backport #3705)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3705 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 18:06:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3760" class=".btn">#3760</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove solo from orderer/consensus
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

Remove solo from orderer/consensus

#### Related issues

Issue: #3514 
Epic: #3511 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 14:42:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3759" class=".btn">#3759</a>
            </td>
            <td>
                <b>
                    Orderer v3: clean solo from integration framework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I4c2f64caff2c44f9706f4a4cde3f6200fa610737

#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: clean solo from integration framework

#### Related issues

Issue: #3514 
Epic: #3511 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-31 14:02:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3758" class=".btn">#3758</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove solo from integration (4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: I1c422996895620f26fd3125caf3dd2143f9396d3


#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Orderer v3: remove solo from integration - part 4.

Change consensus-type migration tests to use raft as the starting point instead of solo, while maintaining as much as possible the testing infrastructure for a future consensus-type.

#### Related issues

Issue: #3514 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-30 17:53:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3757" class=".btn">#3757</a>
            </td>
            <td>
                <b>
                    Orderer v3: remove solo from integration (3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Yoav Tock <tock@il.ibm.com>
Change-Id: Ie5a8430bb70d6ebfd2a56a9eb0fdfc3e9d645a5f

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Orderer v3: remove solo from integration - part 3

#### Related issues

Issue: #3514 
Epic: #3511 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-30 10:03:00 +0000 UTC
    </div>
</div>

