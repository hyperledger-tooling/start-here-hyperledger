---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1676" class=".btn">#1676</a>
            </td>
            <td>
                <b>
                    Fix DIF PresExch and OOB request_attach delete unused connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1608 
- resolve #1609
- Fixed an issue with OOB workflow, unused connections were not deleted with invitation containing request attachments.
- DIF PE: fixed an issue where numerical comparisons are requested for an attribute that could be included as a number string.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 16:00:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1675" class=".btn">#1675</a>
            </td>
            <td>
                <b>
                    [#1674] Add basic DOCKER_ENV logging for run_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 15:32:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1672" class=".btn">#1672</a>
            </td>
            <td>
                <b>
                    Add an integration test for mixed proof with a revocable cred and a n…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …on-revocable cred

Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

(the branch is incorrectly named against the wrong issue oops)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 17:17:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1671" class=".btn">#1671</a>
            </td>
            <td>
                <b>
                    Add pre-commit as optional developer tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds [pre-commit](https://pre-commit.com/) and associated configuration. This is more or less a tool for installing git hooks that check flake8 and black before committing. When used, this helps prevent follow up commits for formatting changes with black or correcting complaints from flake8.

There is also a configuration for installing hooks for checking that the commit message conforms to [conventional commits](https://www.conventionalcommits.org/en/v1.0.0/).

It is possible to use the pre-commit hooks (flake8 and black) without the commit-msg hooks (commitlint) and vice-versa. Contributors can also ignore pre-commit altogether -- this is purely opt-in and must be explicitly installed.

Pre-commit is a pretty widely used tool in the python community and is analogous to [husky](https://typicode.github.io/husky/) in the javascript community. I've had these configuration files hanging out in my local fork of the ACA-Py repo and have been happily using them for more than a year.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 01:13:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1670" class=".btn">#1670</a>
            </td>
            <td>
                <b>
                    Qualify did exch connection lookup by role
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Fixes issue #1541

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 00:22:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1668" class=".btn">#1668</a>
            </td>
            <td>
                <b>
                    Fixes for credential details in issue-credential webhook responses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Attempt to fix an issue with blank credential values seen in the test harness.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 22:35:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1667" class=".btn">#1667</a>
            </td>
            <td>
                <b>
                    Fix: present-proof v2 send-proposal [issue#1474]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <shaangill025@users.noreply.github.com>

resolve #1474 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-14 16:01:10 +0000 UTC
    </div>
</div>

