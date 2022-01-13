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
                PR <a href="https://github.com/hyperledger/fabric/pull/3172" class=".btn">#3172</a>
            </td>
            <td>
                <b>
                    Close connections to stale ordering nodes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes grpc connections to ordering nodes when they are no longer part of any channel configuration.

Resolves https://github.com/hyperledger/fabric-gateway/issues/345

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 13:52:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3171" class=".btn">#3171</a>
            </td>
            <td>
                <b>
                    Refactor gateway Endorse() method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To improve readability and ease of maintenance

Resolves #3122 

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-13 13:50:16 +0000 UTC
    </div>
</div>

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

