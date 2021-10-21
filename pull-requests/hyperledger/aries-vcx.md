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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/365" class=".btn">#365</a>
            </td>
            <td>
                <b>
                    Release 0.22.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">changelog-excluded</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 17:48:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/362" class=".btn">#362</a>
            </td>
            <td>
                <b>
                    Presentation proposal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">breaking</span>
            </td>
            <td>
                Implement [presentation proposal](https://github.com/hyperledger/aries-rfcs/blob/main/features/0037-present-proof/README.md) API.

The state mappings changed from
```
            ProverState::Initial => 0,
            ProverState::PresentationPrepared => 1,
            ProverState::PresentationPreparationFailed => 2,
            ProverState::PresentationSent => 3,
            ProverState::Finished => 4,
            ProverState::Failed => 5
...
            VerifierState::Initial => 0,
            VerifierState::PresentationRequestSent => 1,
            VerifierState::Finished => 2,
            VerifierState::Failed => 3
```
to
```
            ProverState::Initial => 0,
            ProverState::PresentationProposalSent => 1,
            ProverState::PresentationRequestReceived => 2,
            ProverState::PresentationPrepared => 3,
            ProverState::PresentationPreparationFailed => 4,
            ProverState::PresentationSent => 5,
            ProverState::Finished => 6,
            ProverState::Failed => 7
...
            VerifierState::Initial => 0,
            VerifierState::PresentationRequestSet => 1,
            VerifierState::PresentationProposalReceived => 2,
            VerifierState::PresentationRequestSent => 3,
            VerifierState::Finished => 4,
            VerifierState::Failed => 5
```

Verifier initial state was renamed from `Initiated` to `Initial`, so verifier SM now deserializes into
```
{
  "version": "2.0",
  "data": {
    "verifier_sm": {
      "source_id": "123",
      "state": {
        "Initial": {
...
```
instead of
```
{
  "version": "2.0",
  "data": {
    "verifier_sm": {
      "source_id": "123",
      "state": {
        "Initiated": {
...
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 19:07:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/361" class=".btn">#361</a>
            </td>
            <td>
                <b>
                    Update reqwest, tokio, futures dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">update</span>
            </td>
            <td>
                CI fix https://github.com/hyperledger/aries-vcx/pull/360 should be merged first

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 16:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/360" class=".btn">#360</a>
            </td>
            <td>
                <b>
                    Update reqwest, tokio, futures dependencies, fix CI iOS build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci</span>
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-15 14:56:36 +0000 UTC
    </div>
</div>

