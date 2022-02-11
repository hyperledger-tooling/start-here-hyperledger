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
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-11 03:52:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    feat(afj): enable revocation tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Enables revocation tests for AFJ in the holder role. Will enable AFJ in the role of verifier soon.

I've added `@RFC0441` to revocation tests that follow RFC0441, as we don't support revocation not adhering to the best practices.

There are still quite some tests failing, but would like to merge (once the PR in AFJ is merged) so we can get a daily update of the interop status for revocation.

It's weird as some tests are failing where it expects the verification to fail, but it actually succeeds. ACA-Py is the verifier so I'm not sure how it is possible for ACA-Py to return verified=true if the credential was revoked. Maybe AFJ is doing something incorrect, but ACA-Py shouldn't accept the presentation in that case. See [this comment](https://github.com/hyperledger/aries-framework-javascript/pull/592#issuecomment-1033053705) for more context. Will need to dig deeper into this


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 23:15:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    style: format with black
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Format all python files with black. Mostly to prevent a lot of formatting noise in upcoming PRs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 10:37:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Changes by create-pull-request action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-05 03:52:24 +0000 UTC
    </div>
</div>

