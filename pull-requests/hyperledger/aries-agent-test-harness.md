---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/415" class=".btn">#415</a>
            </td>
            <td>
                <b>
                    fixed workflow names to match filename
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This may not clear up the cancelled jobs, but at least we will have a clearer picture of what jobs are being cancelled. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-21 18:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/414" class=".btn">#414</a>
            </td>
            <td>
                <b>
                    further separated crons for less parallel execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sheldon Regular <sheldon.regular@gmail.com>

This may fix the cancelled jobs in the daily interop test runs. If this does work, that means ultimately we need to move to the matrix model so this doesn't happen again. This current submission is just to prove the crons are/were the problem. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-20 13:40:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/413" class=".btn">#413</a>
            </td>
            <td>
                <b>
                    refactor(dotnet): remove credential proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #356

Tested to work with .NET, still running other tests to make sure I didn't break anything else
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 15:23:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/412" class=".btn">#412</a>
            </td>
            <td>
                <b>
                    fix: sleep is not defined
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes an issue with `sleep` not being defined resulting in all present proof tests to fail (not sure how I missed this, as the tests ran successfully yesterday...)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 14:28:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/411" class=".btn">#411</a>
            </td>
            <td>
                <b>
                    fix: rename 0453 to 0454 for present proof
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

Fixes #373
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-19 14:09:17 +0000 UTC
    </div>
</div>

