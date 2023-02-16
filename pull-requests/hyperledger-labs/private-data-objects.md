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
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Separate Sawtooth and CCF tests, speed up CI and reduce (unnecessary) logs
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
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 00:14:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/399" class=".btn">#399</a>
            </td>
            <td>
                <b>
                    add infrastructure to capture backtrace when kv test fails
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Generate trace information that can be used to debug the failing kv test. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-09 19:39:03 +0000 UTC
    </div>
</div>

