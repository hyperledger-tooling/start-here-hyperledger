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

