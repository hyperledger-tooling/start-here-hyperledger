---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    added label to pull correct lint image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A small change that pins the `lint` docker image to the `ubuntu-18-04` label

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 15:49:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-plenum/pull/1563" class=".btn">#1563</a>
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
                This small PR changes the structure of the artifacts uploaded to jfrog artifactory. This is because of conflicts that emerge when uploading deb files with the same name but different distributions.
The new structure will be as follows:
- `indy/pool/xenial/[dev, main, rc, stable]`
- `indy/pool/bionic/[dev, main, rc, stable]`
- `indy/pool/focal/[dev, main, rc, stable]`

Thanks to @WadeBarnes for the discussions we had about this.
The current error can be seen at https://github.com/hyperledger/indy-plenum/runs/3325278452?check_suite_focus=true `Publish 3rd Party Dependencies`.

>Note! A manual clean-up of the current artifacts stored in the jfrog artifactory is needed.

Signed-off-by: udosson <r.klemens@yahoo.de>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-30 14:23:16 +0000 UTC
    </div>
</div>

