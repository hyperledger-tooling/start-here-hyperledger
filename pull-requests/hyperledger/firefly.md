---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/577" class=".btn">#577</a>
            </td>
            <td>
                <b>
                    Add missing itype column in SQLite migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The testing for #549 focussed on PostgreSQL and one of the updates to the migration got missed in the SQLite one.

Raising and will do a test before looking for a review.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 14:23:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Update manifest versions
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
        Created At 2022-03-01 21:12:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/555" class=".btn">#555</a>
            </td>
            <td>
                <b>
                    Explicitly name all subscriptions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #554 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 23:33:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/553" class=".btn">#553</a>
            </td>
            <td>
                <b>
                    Documentation updates from @TheSwarnim
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a build fix to https://github.com/hyperledger/firefly/pull/451
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 18:14:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    Docs "bundle update" to pick up new nokogiri build
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves a dependabot notification: https://github.com/hyperledger/firefly/security/dependabot/7
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 18:11:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/551" class=".btn">#551</a>
            </td>
            <td>
                <b>
                    Roll requestConflictEmptyResult from Group to Data and Message too
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #550

The comment in https://github.com/hyperledger/firefly/pull/513#issuecomment-1036844541 held true - we need to roll the `requestConflictEmptyResult` tweak out to the other optimization cases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 17:58:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/549" class=".btn">#549</a>
            </td>
            <td>
                <b>
                    FIR-9: Identity enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger/firefly-fir/pull/9

@awrichar - the E2E is passing on these changes, but leaving PR in review state as I'd like to add some more E2E tests and do migration testing before pulling it out of draft.

I will put comments in-line in the code to help orient your review
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 21:57:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/548" class=".btn">#548</a>
            </td>
            <td>
                <b>
                    Rename contract subscriptions to contract listeners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes several noteworthy changes:

- Contract Subscriptions have now been renamed to Contract Listeners everywhere, to reduce confusion. This includes the `/contracts/subscriptions` endpoint. It is now `/contracts/listeners`
- The `/subscribe` endpoints on Contract Interfaces and APIs have been dropped
- The `/contracts/listeners` endpoint can now take a interface reference to point it at an existing FFI, rather than putting the full FFI for the event inline
- `blockchain_event` has been renamed to `blockchain_event_received`
- The FFI generator endpoint for Ethereum now expects the ABI nested one level deeper. The payload should now look like:

```json
{
  "input": {
    "abi": []
  }
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-24 21:38:29 +0000 UTC
    </div>
</div>

