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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1865" class=".btn">#1865</a>
            </td>
            <td>
                <b>
                    fix: warnings in tests from IndySdkProfile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes some minor tweaks to tests involving `IndySdkProfile`s to prevent them from emitting warnings. Based on my analysis, the warnings are a result of how the event loop is managed in asynchronous testing with pytest. The profile reference falls out of scope at the same time as the event loop is closed for a test and what results are `Coroutine never awaited` errors.

This may not be the best solution (open to thoughts) but in most cases, I simply monkeypatched the `_make_finalizer` call where the behavior of the finalizer was not what was under test. Where it was under test, I opted to manually call the finalizer before the end of the test (or as a part of fixture clean up) and, therefore, before the event loop starts to close.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 17:04:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1864" class=".btn">#1864</a>
            </td>
            <td>
                <b>
                    RFC 0593 Compliance: Allow issuing JSON LD Credentials with credentialStatus
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the documentation for JSONLD Credentials, there is a parameter
for adding `credentialStatus` to a credential:
https://github.com/hyperledger/aries-rfcs/blob/main/features/0593-json-ld-cred-attach/README.md

However, adding the parameter causes all flows to fail due to the
credentialStatus never making it into the credential. I don't know the
history of this parameter, but in order to follow RFC 0593 a bit more
closely, I have fixed up the flow so that it doesn't fail issuance.

Signed-off-by: Colton Wolkins (Indicio work address) <colton@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-19 16:36:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1863" class=".btn">#1863</a>
            </td>
            <td>
                <b>
                    fix: resolve dids following new endpoint rules
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Naive solution to the issue raised by @TimoGlastra in #1313.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-18 18:04:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1858" class=".btn">#1858</a>
            </td>
            <td>
                <b>
                    Unit test fixes for python 3.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This partially implements the updates in #1717, for the specific tests that were failing under 3.9. There is some overlap with #1854.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 17:42:16 +0000 UTC
    </div>
</div>

