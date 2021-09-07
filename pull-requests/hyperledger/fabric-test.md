---
layout: default
title: fabric-test
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-test
---

# fabric-test <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-test){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    Go1.16.7 release 2.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 18:28:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Go1.16.7 release 2.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 18:25:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/333" class=".btn">#333</a>
            </td>
            <td>
                <b>
                    Update go modules (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run "go mod tidy" on release-2.2.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 18:15:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    Update go modules (release-2.3)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Run "go mod tidy" on release-2.3.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 18:12:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/331" class=".btn">#331</a>
            </td>
            <td>
                <b>
                    Remove indirect upgrade test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The indirect upgrade test (v1.4 to v2.0 to v2.2) does not work with Go 1.16
since it steps through release-2.0 which does not
work with Go 1.16.
This commit stops running the test on the environment that
was recently updated to Go 1.16.

There is still a direct upgrade test from v1.4 to v2.2 which works.
This is the recommended path for users (LTS release to LTS release).

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 15:49:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-test/pull/330" class=".btn">#330</a>
            </td>
            <td>
                <b>
                    Improve upgrade test (release-2.0)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix issues with upgrade test and add logging in release-2.0.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-03 15:20:24 +0000 UTC
    </div>
</div>

