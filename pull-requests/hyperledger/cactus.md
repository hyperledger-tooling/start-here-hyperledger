---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/922" class=".btn">#922</a>
            </td>
            <td>
                <b>
                    docs(faq): internal watch failed: watch ENOSPC
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 18:16:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/921" class=".btn">#921</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): config-service example - authorization JSON
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">bug</span>
            </td>
            <td>
                The custom formatter that was introduced the parse the JSON
config for the authorizer was causing problems.
This was overlooked at the time of the implementation of the authz
feature because Peter (yours truly) is an idiot but also to a smaller
extent because there was no automated test coverage for this specific
issue which this commit is now rectifying by adding a new test case.

Longer term we should look into using a different configuration
parsing library that has more flexibility on how to handle JSON
and validations around it.

There was a second bug masked by the first which is that the
"algorithms" array property of the express-jwt middleware
options was also not being used correctly, but to get to that
first the initial bug with the parsing had to be fixed.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 18:15:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/920" class=".btn">#920</a>
            </td>
            <td>
                <b>
                    fix(connector-besu): removed repeated check
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">dependent</span>
            </td>
            <td>
                Resolve #882 
Depends on #915 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-05 14:44:25 +0000 UTC
    </div>
</div>

