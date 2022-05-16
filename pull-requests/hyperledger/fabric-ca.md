---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    escape special charecters that can be set through the command line ar…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …guments

Signed-off-by: Rohan Shrothrium <rohan.shrothrium@intellecteu.com>

#### Type of change

- Bug fix

#### Description

When we initialise a fabric ca server with an admin and adminpw, if they have special characters the ca behaves not as expected.
These special characters can be in anything that can be passed through the command line arguments.
This PR is meant to escape these special characters in the `yml` file.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-15 19:16:44 +0000 UTC
    </div>
</div>

