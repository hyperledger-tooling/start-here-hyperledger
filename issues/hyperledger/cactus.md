---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/1653" class=".btn">1653</a>
            </td>
            <td>
                <b>
                    fix(docs/examples): cockpitEnabled default value confusion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span><span class="chip">API_Server</span><span class="chip">Nice-to-Have</span><span class="chip">dependencies</span><span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">good-first-issue-400-expert</span><span class="chip">Tests</span><span class="chip">P4</span>
            </td>
            <td>
                There's a problem with the supply chain example app where some changes to the
API server broke it, but the breakage could not be consistently reproduced nor
could we figure out what was the root cause.

There is a suspicion that it is due to the out of bounds yarn install process
that is executed from the `./examples/supply-chain-app/` directory (a `yarn install`)
but there's no proof for this just yet.

If the latter turns out to be the root cause then to fix this bug the fix would
be likely to abandon the directory structure where we have a separate
`./examples/supply-chain-app/` that installs the `...-backend` package and
instead the documentation should instruct the readers to run the supply chain
backend package's entrypoint directly after a monorepo install so that the
dependencies are in-bound instead of out-of-bound (e.g. the local changes
are applied instead of the npm published packages being pulled down).

See the bottom comments on this PR: 
https://github.com/hyperledger/cactus/pull/1623

Specifically: 
https://github.com/hyperledger/cactus/pull/1623#issuecomment-989594072
and
https://github.com/hyperledger/cactus/pull/1623#issuecomment-992472050



<!-- Edit the body of your new issue then click the ✓ "Create Issue" button in the top right of the editor. The first line will be the issue title. Assignees and Labels follow after a blank line. Leave an empty line before beginning the body of the issue. -->
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 23:15:02 +0000 UTC
    </div>
</div>

