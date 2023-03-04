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
                PR <a href="https://github.com/hyperledger/cacti/pull/2310" class=".btn">#2310</a>
            </td>
            <td>
                <b>
                    feat(quorum-connector): add script for checking connection status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Simple script will check ledger connection by getting block through the connector.

Closes: #2309
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 13:59:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2307" class=".btn">#2307</a>
            </td>
            <td>
                <b>
                    fix: cannot read config eslint-config-prettier/@typescript-eslint.js
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For now the ./weaver/ folder has been ignored by the root ESLint config.
This is a temporary fix given that ultimately we should be linting the
entire codebase.

I'll open a follow-up issue to cover the task of turning ESLint back on
for the code under ./weaver/

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 22:39:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2305" class=".btn">#2305</a>
            </td>
            <td>
                <b>
                    docs(maintainers/codeowners): update Sandeep's GH user to sandeepnRES
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Housekeeping of the documents that mention usernames.

Had to skip changing the username in the ./weaver/*.md because of the
newline index corruption problem explained in
https://github.com/hyperledger/cacti/issues/2302

Resolves #2304

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 21:27:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2303" class=".btn">#2303</a>
            </td>
            <td>
                <b>
                    fix(git): broken line endings corrupt git index after weaver merge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not yet sure if this will fix the issue, but based on my research this
is the easiest and most probable solution.

Leaving a "paper trail" of the magical git commands that were executed
in order to have an idea in the future on how to fix potential negative
side-effects that might come out of this later (not likely but if it
does happen this should be immensely helpful information)

Without further ado, the list of commands executed to achieve this diff:

git rm --cached -r .

git config core.autocrlf input

git diff --cached --name-only -z | xargs -0 git add

Fixes #2302

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 21:09:19 +0000 UTC
    </div>
</div>

