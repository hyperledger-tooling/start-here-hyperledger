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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2674" class=".btn">#2674</a>
            </td>
            <td>
                <b>
                    docs: create design doc for adding W3C VC format support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains one main document:

- `AnoncredsW3CCompatibility.md` - the design document for implementing w3c vc/vp format support
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 20:52:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2672" class=".btn">#2672</a>
            </td>
            <td>
                <b>
                    Anoncreds - Add unit testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds unit tests for routes, holder, verifier, issuer.

![Screenshot from 2023-12-13 10-50-52](https://github.com/hyperledger/aries-cloudagent-python/assets/31809382/96589ed6-0add-4cef-bc64-66974229eacd)

There is still more unit testing to do. Mainly the `revocation.py` file. Also, there was a tricky part with scanning the wallet in holder and using `async for` I haven't figured out yet. Also there is some error handling I haven't covered. 

I tried to create objects with the `anoncreds` library as much as possible to catch problems in the future when using the library. When I couldn't manage to make that work I would mock the object a minimally as possible. I also had some trouble creating some DB/wallet `Entry` responses. To get around this i created some minimal class objects. These are used in holder and issuer files.

I made 2 small changes to src code. In verifier.py changed an error handling message and in holder.py added the mime-types attribute constant that seemed to be missing.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 19:10:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    Remove if condition which checks if the `credential.type` array is equal to 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses  #2669

There is currently a validation that prevents credential with only the base type from being signed. The data model spec states that additional credential types are optional. This also prevents conforming to some test-suites where [single credential type](https://github.com/w3c/vc-data-model-2.0-test-suite/blob/main/tests/input/credential-ok.json) credentials are used as test data.

This is a minor change with no impact.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-13 04:47:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2664" class=".btn">#2664</a>
            </td>
            <td>
                <b>
                    Ensure "preserve_exchange_records" flags are set.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Not all cases on issue credential (v1 and v2) were respecting the system default. 

There was a bug on issue credential v1 where `auto_remove` flag was set then ignored before the record was saved.


So behaviour has been tested for issue credential (v1 & v2) and proof presentation (v1 & v2); exchange records are preserved if the `--preserve-exchange-records` is `true` and `auto_remove` has not been set to `True` on API calls that accept it (ie `send-offer`, `send-request`).

Fixes #2656

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-09 00:45:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2663" class=".btn">#2663</a>
            </td>
            <td>
                <b>
                    fix: link to raw content change from master to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Link to image is broken after [RFCs PR#703](https://github.com/hyperledger/aries-rfcs/pull/703) which renamed the "master" branch to "main". It appears that other references (tree, blob) redirect from the URL containing "master" to the equivalent with "main", but URLs with "raw" do not(‽).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 22:28:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2662" class=".btn">#2662</a>
            </td>
            <td>
                <b>
                    Tweak scope of GHA integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move the @GHA tag to the scenarios of each test to allow for some fine tuning of what is included in the github actions.  Exclude most of the AnonCreds tests (but keep a representative sample included).  Add tags for Askar vs Askar-anoncreds wallet types.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 20:03:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2661" class=".btn">#2661</a>
            </td>
            <td>
                <b>
                    fix: open-api generator script
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes the openapi generator script after recent changes. I also did some minor cleanup to make the generated openapi more usable.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-08 04:37:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2660" class=".btn">#2660</a>
            </td>
            <td>
                <b>
                    Additional anoncreds integration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">AnonCreds</span>
            </td>
            <td>
                Review of aca-py integration tests, and include some additional anoncreds scenarios
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 21:53:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2659" class=".btn">#2659</a>
            </td>
            <td>
                <b>
                    Improve Per Tenant Logging: Fix issues around default log file path
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
        Created At 2023-12-07 19:55:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2658" class=".btn">#2658</a>
            </td>
            <td>
                <b>
                    Update snyk workflow to execute on Pull Request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - run on pull_request not push
- only when PRs change /aries_cloudagent files or /docker files.

Not sure how to test this... 

fixes #2526 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-07 18:18:10 +0000 UTC
    </div>
</div>

