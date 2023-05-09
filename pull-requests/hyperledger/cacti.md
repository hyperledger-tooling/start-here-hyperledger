---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2419" class=".btn">#2419</a>
            </td>
            <td>
                <b>
                    chore(ci): Update codeql action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also, commitlint was out-of-date.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-09 01:40:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2418" class=".btn">#2418</a>
            </td>
            <td>
                <b>
                    feat: add private htlcs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                adds private htlcs to the htlc package (with tests)
updates non-rivate htlc contract
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 23:59:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2417" class=".btn">#2417</a>
            </td>
            <td>
                <b>
                    feat(connector-tcs-huawei):  Initial commit of feature tcs-huawei connector.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                tcs-huawei and the blockchains connected to tcs-huawei can be integrated to cactus by this connector.

Signed-off-by: Wang Yinglun wangyinglun3@huawei.com 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-08 06:19:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2416" class=".btn">#2416</a>
            </td>
            <td>
                <b>
                    fix(vscode/devcontainer): unexpected exit stdout /etc/passwd
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Moved away from trying to handroll an Ubuntu-22.04 image for the dev container
and instead used the "features" feature (no pun intended) of the dev container
spec: https://code.visualstudio.com/blogs/2022/09/15/dev-container-features
2. This produces a container that builds and launches reliably without the
issues the previous version was suffering from (which was that to some people
the container would just exit randomly during the launch)
3. Our future goal of having the dev container being built in a reproducible
way is still not achieved, but we've gotten closer because in the meantime
while working on this issue it was discovered that we can re-build the images
directly from the CLI by using the dev container CLI package:
https://github.com/devcontainers/cli
4. The upside of not building the image from scratch is that we can count on
future improvements/maintenance from others who are working on these images.
5. The downside of not building the image from scratch is that if we end up
finding something that does not work due to the customizations, it might be
more difficult to figure that out compared to if we had just build our own.
6. It is hard to predcit right now whether 4) or 5) will end up being having
the stronger effect, but we can cross that bridge when we get to it.
7. In the meantime I've started working on a contribution to the dev container
CLI itself for a dockerfile ejection feature (meaning that we'll be able to
render a single Dockerfile for the dev container (that right now the CLI only
stores/uses internally in it's own code at runtime). This eject feature will
be good for debugging purposes in case anything goes wrong with the image in the
future.

Fixes #2404

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 17:34:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2415" class=".btn">#2415</a>
            </td>
            <td>
                <b>
                    chore(ci): publish weaver go modules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Chore:
- chore(ci): publish weaver go modules
   This way of publishing all go modules in single commit will work as long as in the release commit, only version files are changed and script `go-gen-checksum.sh` in root directory is run, and no other changes are made between that commit and actual releasing (i.e. no other PR is merged affecting these go modules till release PR is merged).

Fixes:
- fix(ci): update version only if tag has version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-05 06:37:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2414" class=".btn">#2414</a>
            </td>
            <td>
                <b>
                    feat(openssl): version upgrade to v0.10.48 in cactus-plugin-keychain-vault
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: issue #2365
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-04 10:58:52 +0000 UTC
    </div>
</div>

