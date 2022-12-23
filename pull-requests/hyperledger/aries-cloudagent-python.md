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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2060" class=".btn">#2060</a>
            </td>
            <td>
                <b>
                    Do not reject OOB invitation with unknown handshake protocol(s)
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
        Created At 2022-12-22 23:01:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2059" class=".btn">#2059</a>
            </td>
            <td>
                <b>
                    ci: test additional versions of python nightly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This will help unblock efforts to move off of python 3.6.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 20:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2058" class=".btn">#2058</a>
            </td>
            <td>
                <b>
                    ci: add gha for pr-tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds GitHub Actions for testing PRs. This is pulled from work on #1888. These tests are ready for easy use with other python versions, when we get to that point.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 16:44:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2055" class=".btn">#2055</a>
            </td>
            <td>
                <b>
                    Additional integration tests for revocation scenarios
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Additional tests for multi-credential proofs with a mix of revocable and non-revocable credentials

These tests pass:
- @T003-RFC0454.1 - two credentials, one revocable one not, neither revoked, "non_revoked" is requested at the attribute level
- @T003-RFC0454.2 - two credentials, one revocable one not, one revoked, proof checks for revocation (attribute level) and fails
- @T003-RFC0454.3 - two credentials, one revocable one not, one revoked, proof *doesn't* check for revocation (attribute level) and passes

This test "fails" - the proof doesn't verify even though it should:
- @T003-RFC0454.1f - two credentials, one revocable one not, neither revoked, "non_revoked" is requested at the*request* level

For the failing scenario, it fails with indy-sdk and credx.  I believe  the underlying library is not creating the proof properly, and/or the underlying anoncreds itself has a bug.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-21 00:15:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2054" class=".btn">#2054</a>
            </td>
            <td>
                <b>
                    fix: indy dependency version format
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix python-indy version restrictions format.

Previous format was breaking for poetry-based builds: `Invalid constraint (python3-indy (>=1.11.1<2) ; extra == 'indy') found in aries-cloudagent-1.0.0rc1 dependencies, skipping`

Version restrictions are supposed to be conformant to: https://peps.python.org/pep-0440/#version-specifiers

Signed-off-by: Clément Humbert <clement.humbert@sicpa.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-19 08:02:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2053" class=".btn">#2053</a>
            </td>
            <td>
                <b>
                    Code formatting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Issue https://github.com/hyperledger/aries-cloudagent-python/issues/2052

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-18 23:52:13 +0000 UTC
    </div>
</div>

