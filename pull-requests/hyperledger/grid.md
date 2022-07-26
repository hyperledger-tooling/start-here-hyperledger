---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1462" class=".btn">#1462</a>
            </td>
            <td>
                <b>
                    Add just recipe for fixing typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-26 17:01:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1461" class=".btn">#1461</a>
            </td>
            <td>
                <b>
                    Update Ubuntu / OS X build dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                Replaced postgres with libpq / libpq-dev, as a full postgres
installation is not strictly necessary.

For Ubuntu: Replaced insufficient libprotobuf-dev with the more accurate
protobuf-compiler dependency. Added required openssl, libsasl2-dev,
libxml2-dev, libsqlite3-dev, pkg-config, and build-essential.

Signed-off-by: Amelia Bradley <bradley@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-21 17:03:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1460" class=".btn">#1460</a>
            </td>
            <td>
                <b>
                    Update ci-test just recipe so unit-tests pass in GHA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                The GHA provided runners have limited free space so after building Docker
images necessary for the test they can easily run out of disk, causing the
test to fail. Removing unecessary prepopulated Docker images and some
large android libraries ensures there's plenty of headroom for our builds.

Link to list of pre-installed software:
https://github.com/actions/virtual-environments/blob/main/images/linux/Ubuntu2004-Readme.md

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 21:44:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    Fix typos and add PR test for typos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-20 19:24:42 +0000 UTC
    </div>
</div>

