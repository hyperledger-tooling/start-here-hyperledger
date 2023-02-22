---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Fix a problem with the client build and canonicalize python clean
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix client flags in the python setup file.

Fix a problem with dependency on SGX_SDK (not required for the client) when cleaning. Basically this makes clean in the python directory the same as it is in all of the other directories.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-21 20:34:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Remove tinyscheme download from pdo-dev image
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
        Created At 2023-02-21 19:48:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Separate Sawtooth and CCF tests, speed up CI, reduce (unnecessary) logs and solve double build (with possible corruption) issue
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR reduce the run time of the CI by ~30% by:
1. separating the tests for sawtooth and ccf, thus running them in parallel
2. removing the upgrade of the packages -- which was performed on all packages in pdo-dev, not just those necessary for PDO
3. redirecting the stdout/err of the sgxssl/openssl build to /dev/null -- importantly, this also reduces the CI logs from ~30K lines to **~8K lines**!!!

Additionally, it solves an issue with a duplicate build (of setup.py in /python).
The issue was caused by a misrepresented rule. The rule has 2 targets, which are all generated in one execution. However, by listing the 2 targets as dependencies and running make with multiple threads, make does not know that those targets should be grouped, so it runs the rule twice in parallel.
The result is a double build, which sometimes succeeds and sometimes corrupts the outputs (and later builds fail).
It is quite possible that the issues experienced so far on the system tests of the key-value store were due to this problem.
In fact, the python and the swig files used in the tests (which sometimes failed with an "illegal instruction") were part of the double build output.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 00:14:38 +0000 UTC
    </div>
</div>

