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
                PR <a href="https://github.com/hyperledger/aries-rfcs/pull/789" class=".btn">#789</a>
            </td>
            <td>
                <b>
                    Add clarification to thread RFC about handling an empty thread decorator
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

See issue [#875 in Aries VCX](https://github.com/hyperledger/aries-vcx/issues/875).  This PR clarifies that while it is not recommended, an Aries agent MAY put an empty `~thread: {}` item in the first message of a protocol instance, and a recipient Aries agent MUST be able to handle that.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 18:39:15 +0000 UTC
    </div>
</div>

