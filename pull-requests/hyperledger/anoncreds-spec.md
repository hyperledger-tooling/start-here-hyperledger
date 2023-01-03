---
layout: default
title: anoncreds-spec
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-spec
---

# anoncreds-spec <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-spec){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/125" class=".btn">#125</a>
            </td>
            <td>
                <b>
                    revocation list model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Initial attempt to add the revocation list model to the anoncreds spec. It is based on #108 and replaces revocation registry entries. We should probably add some of the stuff about deltas and revocation registry entries to an implementers guide, and add the transformation from deltas/entries to the revocation status list model to the indy anoncreds method spec (is this already defined somewhere?)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 05:34:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    update revocation registry model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the revocation registry model to use camelCase and follow the anoncreds implementation.

I've not updated the revocation registry entry related content as that'll be replaced with the revocation list model (in a follow up PR). 

I've also updated the wording of the tag to follow that of the credential definition tag, but we may want to rewrite this after an decision has been made regarding #123 

Model in AnonCreds RS (same as Indy Shared RS): https://github.com/hyperledger/anoncreds-rs/blob/main/anoncreds/src/data_types/anoncreds/rev_reg_def.rs#L72-L100
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 04:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    update credential definition model to camelCase
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the credential definition model to use camelCase for schemaId property. this is because the AnonCreds data models use camelCase by default.

Model in AnonCreds RS (same as Indy Shared RS): https://github.com/hyperledger/anoncreds-rs/blob/main/anoncreds/src/data_types/anoncreds/cred_def.rs#L46-L52
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 04:23:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-spec/pull/121" class=".btn">#121</a>
            </td>
            <td>
                <b>
                    update schema model to camelCase
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates the schema model to use camelCase for the attrNames property. this is because the AnonCreds data models use camelCase by default. 

Model in AnonCreds RS (same as Indy Shared RS): https://github.com/hyperledger/anoncreds-rs/blob/main/anoncreds/src/data_types/anoncreds/schema.rs#L19-L26
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-03 04:14:49 +0000 UTC
    </div>
</div>

