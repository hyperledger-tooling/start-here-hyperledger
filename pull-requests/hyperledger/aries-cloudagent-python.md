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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1565" class=".btn">#1565</a>
            </td>
            <td>
                <b>
                    Update docker scripts to use new & improved docker IP detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Required to support newer versions of docker

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 18:02:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1564" class=".btn">#1564</a>
            </td>
            <td>
                <b>
                    Fix the inconsistency of invitation_msg_id between invitation and response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi!
This PR fixes the inconsistency of invitation_msg_id between invitation and response when connection is reused.

### example of problem
`receive-invitation` with invitation
{"@type": "did:sov:BzCbsNYhMrjHiqZDTUASHg;spec/out-of-band/1.0/invitation", "@id": "**6ccba5e9-2b8d-4071-bd91-0058d5187d79**", "services": ["did:sov:2ACCk6nnJQmaibXp5yiXZA"], ...

The response of `receive-invitation`
{"my_did": "VrN5qwVB7ewV43C679ekUx", "invitation_msg_id": "**a7753007-5e3f-4583-826b-ae94550fed15**", "their_public_did": "2ACCk6nnJQmaibXp5yiXZA", ...

### solution
Fetch the connection record after reuse handshake.

Thanks!

Signed-off-by: Ethan Sung <baegjae@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-17 07:06:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1563" class=".btn">#1563</a>
            </td>
            <td>
                <b>
                    Typo vdr service name
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
        Created At 2021-12-16 21:46:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1562" class=".btn">#1562</a>
            </td>
            <td>
                <b>
                    chore: update pydid to ^0.3.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should have a pretty minimal impact on things while enabling resolution of Documents with nonconforming `@context` attributes (spec defines that context must be a list of strings, some docs have embedded contexts). Also solves the bug mentioned in this comment from forever ago: https://github.com/hyperledger/aries-cloudagent-python/pull/1218#issuecomment-890591874
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-16 20:19:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1561" class=".btn">#1561</a>
            </td>
            <td>
                <b>
                    Add alias field to didexchange invitation UI
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
        Created At 2021-12-16 17:56:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1558" class=".btn">#1558</a>
            </td>
            <td>
                <b>
                    Await asyncio.sleeps
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes a few warnings during tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 22:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1557" class=".btn">#1557</a>
            </td>
            <td>
                <b>
                    ACA-Py Upgrade command implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
- `upgrade` command
  **Example**
  ```
  ./scripts/run_docker upgrade --upgrade-config ./aries_cloudagent/acapy_upgrade_config.yml \
  --from-version 0.7.2 \
  --wallet-type indy \
  --wallet-name issuer \
  --wallet-key mykey \
  --wallet-storage-type postgres_storage \
  --wallet-storage-config '{"url":"host.docker.internal:5432","max_connections":5}' \
  --wallet-storage-creds '{"account":"postgres","password":"pwd","admin_account":"postgres","admin_password":"pwd"}'
  ```
    - `--upgrade-config` - path to YAML config file
      **Example YAML config**
      ```
      0.6.0:
      ...
      0.7.1:
      ...
      0.7.2:
        resave_records:
          base_record_path:
            - "aries_cloudagent.connections.models.conn_record.ConnRecord"
          base_exch_record_path:
            - "aries_cloudagent.protocols.issue_credential.v1_0.models.credential_exchange.V10CredentialExchange"
        update_existing_records: false
      ```
      The above will re-save `ConnRecord` and `V10CredentialExchange`. `update_existing_records` can be used to handle 
      changes where existing records need to be updated, for instance, if a new required field has been added to Marshmallow 
      schema. The steps/logic for this can be implemented [here](https://github.com/hyperledger/aries-cloudagent-python/blob/473e1053da9fb278d39d2a863598f5671ec51466/aries_cloudagent/commands/upgrade.py#L40) and [here](https://github.com/hyperledger/aries-cloudagent-python/blob/473e1053da9fb278d39d2a863598f5671ec51466/aries_cloudagent/commands/upgrade.py#L131), this will have to be managed every release.
    - `--from-version` is used to specify the ACA-Py version from which to upgrade.
    - Also accepts `WalletGroup` arguments

Thanks @ianco for suggesting the command approach. This is an initial implementation, for now, it can only handle re-save and/or update records but it can be expanded upon. @andrewwhitehead, @swcurran, and @ianco I will appreciate any feedback.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 17:31:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1556" class=".btn">#1556</a>
            </td>
            <td>
                <b>
                    Added event queue support as an alternative to webhook notifications
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## What is this PR for?

- Added external queue support as an alternative to HTTP webhook events
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-13 14:51:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1553" class=".btn">#1553</a>
            </td>
            <td>
                <b>
                    PR#1543 Follow up - Adding invitation_msg_id and their_public_did back to record_value.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shaanjot Gill <gill.shaanjots@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-11 20:13:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1551" class=".btn">#1551</a>
            </td>
            <td>
                <b>
                    Update demo requirements
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
        Created At 2021-12-11 00:45:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1550" class=".btn">#1550</a>
            </td>
            <td>
                <b>
                    Remove required dependencies from multi-ledger code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also adjusts the return value from `get_ledger_for_identifier` for consistency.

Fixes #1549 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-10 23:55:24 +0000 UTC
    </div>
</div>

