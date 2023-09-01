---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/965" class=".btn">#965</a>
            </td>
            <td>
                <b>
                    Extract message sending from prover & verifier SMs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">refactoring</span>
            </td>
            <td>
                Extracts message sending out of prover and verifier state machines and handlers. Transition functions are now returning messages constructed to be sent and are not accepting message-sending closures.

## Prover
### Handlers

- `send_proposal` -> `build_presentation_proposal`
- `send_presentation` -> `mark_presentation_sent`
- Removed `set_presentation`

### State machine

- `send_presentation_proposal` -> `build_presentation_proposal`
- `send_presentation` -> `mark_presentation_sent`
- Added `get_problem_report`, `get_presentation_proposal`
- Removed `set_presentation`

## Verifier
### Handlers

- `send_presentation_request` -> `mark_presentation_request_sent` (TODO: better name)
- `set_request` -> `set_presentation_request`
- Removed `mark_presentation_request_msg_sent`, `get_presentation_request`

### State machine

- `set_request` -> `set_presentation_request`
- `mark_presentation_request_msg_sent` -> `mark_presentation_request_sent`
- Added `get_final_message`

`verify_presentation` now generates and stores either presentation or problem report, which can then be retrieved via `get_final_message`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-31 07:15:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/964" class=".btn">#964</a>
            </td>
            <td>
                <b>
                    Enable compiling the workspace with --tests --all-features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span>
            </td>
            <td>
                See #890 .
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-30 10:03:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/961" class=".btn">#961</a>
            </td>
            <td>
                <b>
                    Prover: fix credx credential retrieval
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes retrieval of credentials for prover. When multiple restriction objects are specified, they should be treated as `OR` instead of `AND`. Verifier is asking prover to satisfy at least 1 restriction object, not all of them.

- Adds test `test_agency_pool_it_should_select_credentials_for_satisfiable_restriction` which was failing without modifications to WQL made in the PR. Passes with the modifications. See anoncreds spec https://hyperledger.github.io/anoncreds-spec/#restrictions

> A boolean expression is formed by ORing and ANDing the source credential properties. The following JSON is an example. Any of the source credential properties listed above can be used in the expression components:
> 
>       "restrictions": [
>         {
>           "issuer_did": "<did>",
>           "schema_id": "id"
>         },
>         {
>           "cred_def_id" : "<id>",
>           "attr::color::marker": "1",
>           "attr::color::value" : "red"
>         }
>       ]
> The properties in each list item are AND’d together, and the array elements are OR’d together. As such, the example above defines the logical expression:
> 
> The attributes must come from a source verifiable credential such that:
>    issuer_did = <did> AND
>      schema_id = <id>
>    OR
>    cred_def_id = <id> AND
>       the credential must contain an attribute name "color" AND
>       the credential must contain an attribute name "color" with the attribute value "red"

- Test refactoring also uncovered that test `test_agency_pool_it_should_fail_to_select_credentials_for_predicate` is not working with credx implementation; see: https://github.com/hyperledger/aries-vcx/issues/962
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 18:04:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/960" class=".btn">#960</a>
            </td>
            <td>
                <b>
                    Fix profile building in tests, considering vdrtools is default feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - When profile is selected dynamically based on feature flags (in testing), it would previously always select always `vdrtools` profile, regardless of `modular_libs` feature being enabled.
- This bug was probably brought in some of the relatively recent test setup / feature refactoring.
- Nevertheless the modular libs (which were apparently not being tested in CI since introduction of the bug) are passing fine ✅ 

Proper solution though, should be removing `vdrtools` as default feature
- had a quick shot at it, but it's a bit trickier, as tests require vdrtools wallet regardless of whether we are running with credx/vdrtools anoncreds
- it's possible to address, but figured it'll be easier just to wait out for vdrtools anoncreds to die out
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-29 16:48:44 +0000 UTC
    </div>
</div>

