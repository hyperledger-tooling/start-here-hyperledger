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
                PR <a href="https://github.com/hyperledger/fabric/pull/3167" class=".btn">#3167</a>
            </td>
            <td>
                <b>
                    Maintain Pvt data hashed index
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds code for creating hashed index entries during block commit and deleting the hashed index entries during purge triggered by _Block to live_ based expiry

#### Type of change
- New feature

#### Additional details
The indexes needs also to be maintained when the private data is committed via reconciliation. However, this will be covered in a separate story (issue #3027) because, during reconciliation we need to take care of trimming the already purged data, if any.

#### Related issues
issue #3023 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-12 05:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3163" class=".btn">#3163</a>
            </td>
            <td>
                <b>
                    Update test_network.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Entry in troubleshooting if iptables error occurs

- Documentation update

The entry describes a possible error that occured to me, when I wanted to run the test-network. Since I found many entries regarding iptables and unknown option --dport I thought it could concern others, too. 

Signed-off-by: Jannes Klee jannes.klee@gmail.com

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-07 14:36:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3160" class=".btn">#3160</a>
            </td>
            <td>
                <b>
                    Add initial v2.5.0 release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add initial v2.5.0 release notes.
Also remove the v2.4.x release notes from main branch, as they get maintained in release-2.4 branch instead.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 22:16:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3159" class=".btn">#3159</a>
            </td>
            <td>
                <b>
                    Updates in main for v2.4.1.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and scripts in main to reflect latest v2.4.1 release.
Also update Makefile to reflect next release (v2.5.0).

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-05 21:43:23 +0000 UTC
    </div>
</div>

