---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1696" class=".btn">#1696</a>
            </td>
            <td>
                <b>
                    Update version of Indy SKD
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update version of Indy SDK to the same version used in Indy-Plenum which is at `python3-indy==1.15.0-dev-1625`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 16:24:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-node/pull/1695" class=".btn">#1695</a>
            </td>
            <td>
                <b>
                    fix uploading of deb files with the same name but different distribution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR rearranges the uploading structure of the debian files according to the changes made in Indy-Plenum in this [commit](https://github.com/hyperledger/indy-plenum/commit/52ddd72c0dec5f037396bf0e88acbd38d13cdb4d).
The new structure prevents errors in uploading of debian files with the same filename but build from a different distribution.
The new structure will be as follows:
- `indy/pool/xenial/[dev, main, rc, stable]`
- `indy/pool/bionic/[dev, main, rc, stable]`
- `indy/pool/focal/[dev, main, rc, stable]`

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 13:19:09 +0000 UTC
    </div>
</div>

