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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1478" class=".btn">#1478</a>
            </td>
            <td>
                <b>
                    Clean up old docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 14:18:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1476" class=".btn">#1476</a>
            </td>
            <td>
                <b>
                    fix: use named tuple instead of dataclass in mediation invite store
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dataclass wasn't added until python 3.7 and we're on 3.6. Not sure how this wasn't failing tests :thinking: we must have a backport package installed in the base image or similar but at any rate, I'm hopeful this will resolve issues @swcurran raised in #1473 for this module's doc generation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 20:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1475" class=".btn">#1475</a>
            </td>
            <td>
                <b>
                    Update credential and proof mappings to allow negative encoded values
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue https://github.com/hyperledger/aries-cloudagent-python/issues/1462

@jsyro
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 18:13:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1473" class=".btn">#1473</a>
            </td>
            <td>
                <b>
                    WIP: Updating the RTDs code for Release 0.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update the the Read The Docs material in preparation for the next release of ACA-Py.  We'll leave this as a WIP until 0.7.2 is ready to be released, to catch the latest updates.

Currently getting generation errors from the [coordinate_mediation](https://github.com/hyperledger/aries-cloudagent-python/blob/main/aries_cloudagent/protocols/coordinate_mediation/mediation_invite_store.py) module. Help on these would be appreciated -- it's something to do with the formatting of the documentation for the listed methods:

``` bash
WARNING: error while formatting arguments for aries_cloudagent.protocols.coordinate_mediation.mediation_invite_store.MediationInviteRecord.from_json: Handler <function update_annotations_using_type_comments at 0x7f18ab6a5ae8> for event 'autodoc-before-process-signature' threw an exception (exception: wrapper loop when unwrapping dataclasses.dataclass.from_json)
WARNING: error while formatting arguments for aries_cloudagent.protocols.coordinate_mediation.mediation_invite_store.MediationInviteRecord.to_json: Handler <function update_annotations_using_type_comments at 0x7f18ab6a5ae8> for event 'autodoc-before-process-signature' threw an exception (exception: wrapper loop when unwrapping dataclasses.dataclass.to_json)
WARNING: error while formatting arguments for aries_cloudagent.protocols.coordinate_mediation.mediation_invite_store.MediationInviteRecord.unused: Handler <function update_annotations_using_type_comments at 0x7f18ab6a5ae8> for event 'autodoc-before-process-signature' threw an exception (exception: wrapper loop when unwrapping dataclasses.dataclass.unused)
/home/swcur/repos/aries-cloudagent-python/aries_cloudagent/protocols/coordinate_mediation/mediation_invite_store.py:docstring of aries_cloudagent.protocols.coordinate_mediation.mediation_invite_store.MediationInviteStore.get_mediation_invite_record:10: WARNING: Field list ends without a blank line; unexpected unindent.
```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 14:56:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1472" class=".btn">#1472</a>
            </td>
            <td>
                <b>
                    Fixed potential deadlocks by opening sessions only on demand (Wallet endpoints)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Removed potential deadlocks for Wallet endpoints

Additional info in this issue: #1417 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 09:10:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1469" class=".btn">#1469</a>
            </td>
            <td>
                <b>
                    Fix connection record response for mobile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

See issue: https://github.com/hyperledger/aries-cloudagent-python/issues/1441

This is a bit of a shot in the dark, the connection auto-replies aren't following the same convention as other protocols.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 22:29:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1465" class=".btn">#1465</a>
            </td>
            <td>
                <b>
                    Fix error removing proof req entries by timestamp
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issue https://github.com/hyperledger/aries-cloudagent-python/issues/1455

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-30 00:12:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1464" class=".btn">#1464</a>
            </td>
            <td>
                <b>
                    Implement Revocation Notification v1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements revocation notifications following the RFC: https://github.com/hyperledger/aries-rfcs/blob/main/features/0183-revocation-notification/README.md

Currently, `~please_ack` support is not implemented and there is no way to propagate a comment from issuer to recipient. Hopefully this serves as a good starting point to collect feedback.

I've done some testing using the [revocation demo](https://github.com/Indicio-tech/acapy-revocation-demo) I put together a while ago and everything worked as expected but I plan to implement some tests (at a minimum unit tests, perhaps integration test with some direction from @ianco) before we merge this one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 20:57:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1463" class=".btn">#1463</a>
            </td>
            <td>
                <b>
                    Allow base wallet to connect to a mediator after startup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Connecting the base wallet to a mediator is supported through command line arguments but not the Admin API. In our experience, it is often simpler to establish the base wallet's mediator after startup through the Admin API. That being said, there could be consequences to this change that I'm not seeing yet so hoping @ianco and @TimoGlastra could give their thoughts on this change.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-29 13:01:25 +0000 UTC
    </div>
</div>

