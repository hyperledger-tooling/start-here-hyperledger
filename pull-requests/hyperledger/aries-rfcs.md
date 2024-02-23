---
layout: default
title: aries-rfcs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-rfcs
---

# aries-rfcs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-rfcs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/815" class=".btn">#815</a>
            </td>
            <td>
                <b>
                    Propose reverting issue-credential-v2 and present-proof-v2 to v2.0, removing v2.1 and v2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Proposes that we remove v2.1 and v2.2 from these two protocols, as they are not implemented, v2.1 is not easily implemented (and is an edge case), and makes upgrading to V3.0 harder for anyone that does actually implement them. The bottom line is that as far as we know, no one has implemented these versions, and we want it to stay that way.

To make this change, I copy/pasted the RFCs from those defined in AIP 2.0, and then put in any clarifications that were unrelated to the v2.1 and v2.2 changes.  The result is (I think) an up to date version of each RFC that reflects the reality and direction of the community.

To be discussed at an upcoming Aries Working Group meeting. 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-16 19:05:35 +0000 UTC
    </div>
</div>

