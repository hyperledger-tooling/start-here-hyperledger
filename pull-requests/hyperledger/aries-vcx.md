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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/966" class=".btn">#966</a>
            </td>
            <td>
                <b>
                    Updates and fixes to sync this branch with changes of #937
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
        Created At 2023-09-01 11:45:34 +0000 UTC
    </div>
</div>

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
- `send_presentation` -> `mark_presentation_sent` (now throws in invalid state)
- Added `get_problem_report`, `get_presentation_proposal`
- Removed `set_presentation`

## Verifier
### Handlers

- `send_presentation_request` -> `mark_presentation_request_sent` (now throws in invalid state, TODO: better name)
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

