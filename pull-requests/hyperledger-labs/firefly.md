---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Enhance blob upload support, to include metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Blobs now can have both a `blob` attachment and `value` JSON
- On upload user can add some extra form parameters - must be before the upload file itself:
  - `metadata` - can be a string or a JSON object
  - `autometa` - if `true` then the `filename`,`size` and `mimetype` are added to JSON metadata
     - Can be combined with `metadata` if the metadata is JSON
  - `datatype.name` - if the metadata needs to be validated per a datatype
  - `datatype.version` - if the metadata needs to be validated per a datatype
  - `validator` - to customize the validator (only `json` is supported today)
- The `hash` of the `data` object created, will be one of:
  - The `value` hash - if just a JSON value
  - The `blob` hash reference - if just a BLOB value
  - A hash of the two HEX hashes concatenated together (no spaces or separators)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 21:54:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/78" class=".btn">#78</a>
            </td>
            <td>
                <b>
                    Get all config on admin, and support flat config records
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - `/admin/api/v1/config` moved to `/admin/api/v1/config/records`
- `GET` `/admin/api/v1/config` added to download full merged config
- Fixed an error restarting when you set a non-object value in `/admin/api/v1/config/records`

In a PR chain with https://github.com/hyperledger-labs/firefly/pull/76
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 16:01:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/76" class=".btn">#76</a>
            </td>
            <td>
                <b>
                    Add pending and rejected fields to messages, and use for clear sort order
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Fixes this error seen after groups were added:
  `"error": "FF10121: Database resultset read error from table 'messages': sql: Scan error on column index 8, name \"group_hash\": encoding/hex: invalid byte: U+0020 ' '"`
  - The problem here was `.Set("group",` code incorrectly using a non-nil string for `nil` values
  - This was because all hashes were using `StringField` in the `QueryFactory` implementations
  - Created a `Bytes32Field` as a partner to `UUIDField` and swapped them all over
- Fixes #72 "Sort messages by confirmed, not the created sequence"
  - This was a little harder than I expected.
  - The absolute order will always be the `/events` sequence (because clocks can jitter in exceptional circumstances), but it is very strange if the order of the messages in the `/messages` collection (and hence the UI) does not match the order you were delivered them
  - To get an order that makes sense I had to add two fields to messages:
    - `pending` - this starts `true`, and goes to false once the message is `confirmed`
    - `rejected` - is set to `true` if a message is confirmed, but with a failure (partners a `message_rejected` event)
  - This was necessary so that I could have a sort order of:
    - `pending,confirmed,created` (all descending) - meaning pending messages are always listed first in created order, then confirmed messages in order - including failed confirmed messages
  - I renamed `message_invalid` to `message_rejected` for consistency
  - There's some faff as PSQL and QL differ on a couple of fundamentals
    - QL does not support sorting `bool` columns - so I went for a `smallint` approach for the `pending` column
    - QL does not support per-column sorting - so I went for a consistent sort order
  - I also made it so you can specify a `-` prefix on individual column sorts on the API
- Small tweak to the `e2e` test to use the `-n` option on `ff start` proposed in https://github.com/hyperledger-labs/firefly-cli/pull/37
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-15 04:54:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Add namespace to ops
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 12:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/70" class=".btn">#70</a>
            </td>
            <td>
                <b>
                    Readme updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 12:42:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/67" class=".btn">#67</a>
            </td>
            <td>
                <b>
                    Add private test to e2e
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Used created timestamp on message query, to allow re-running the test with `go test -v` without rebuilding the env
- Added a common test setup structure
- Added a private messaging test
- Added a `make e2e-rebuild` that just re-runs the e2e test
- Updated the `apiserver` to have a mockable interface, consistent with all other components
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 03:12:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/66" class=".btn">#66</a>
            </td>
            <td>
                <b>
                    Add namespace to operation filter factory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ` "error": "FF10148: Unknown filter 'namespace'"` when querying operations on API
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-11 02:00:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/65" class=".btn">#65</a>
            </td>
            <td>
                <b>
                    Updates to private messaging from e2e testing with CLI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves a few nits in the end-to-end flow:
- Ensuring the group creation event is created, and included in the same namespace as the first message on that group
- Making a batch rewind wake up the event poller immediately, to assemble the message
- Generate a `group_confirmed` event only (no separate `message_confirmed`) when a group arrives
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 22:55:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/64" class=".btn">#64</a>
            </td>
            <td>
                <b>
                    fix proposal link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nick Gaski <nick.gaski@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 21:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/63" class=".btn">#63</a>
            </td>
            <td>
                <b>
                    Fix E2E test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This gets the E2E test running again with the latest API. Can (should) be run manually before commits with `./test/e2e/run.sh`. Eventually will get it added to a GitHub action as well.

It's not as clean or as thorough as it could be, but it's a start. Feedback/future suggestions welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 21:02:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/62" class=".btn">#62</a>
            </td>
            <td>
                <b>
                    Add status API endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `GET` `/api/v1/status` returns a structure containing:

- Org information - name, identity, whether it's registered, and if so what the ID is
- Node information - name, whether it's registered, and if so what the ID is
- Defaults - just the default namespace for now
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 15:42:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/61" class=".btn">#61</a>
            </td>
            <td>
                <b>
                    Rename the go package name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 13:54:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/60" class=".btn">#60</a>
            </td>
            <td>
                <b>
                    Config API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new `/config` endpoint which can be used for dynamically adding or modifying config at runtime via a REST API. Any change in configuration will result in a restart of all services and plugins (not the process itself though).

Due to how powerful (dangerous) the new configuration endpoints are, they have been moved to a separate “admin” HTTP listener which will listen on a separate port, if enabled at all. By default, it is disabled. To enable the admin endpoints, add the following lines to your firefly.core config:

```yaml
admin:
  enabled: true
  address: 0.0.0.0
  port: 5001
```

To set a configuration key make a `PUT` request to `/admin/api/v1/config/{key}` with a JSON request body.


For example, if you want to set the HTTP URL for ethconnct, you would make a `PUT` request to `/admin/api/v1/config/blockchain.ethereum.ethconnect` with a request body of:

```json
{
  "url": "http://some_url"
}
```

The payload will be merged with any existing config. This means that it is not possible to _remove_ configuration keys that are present in the config file, via the REST API.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-10 01:08:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/59" class=".btn">#59</a>
            </td>
            <td>
                <b>
                    Add Docker Build GitHub Action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new GitHub Action that builds and pushes Docker images to GitHub Container Repository.

It also re-enables our normal PR checks after the repo was transferred.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 22:55:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/58" class=".btn">#58</a>
            </td>
            <td>
                <b>
                    Update links in README.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updated links to match new repo URLs
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 22:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/56" class=".btn">#56</a>
            </td>
            <td>
                <b>
                    Update GitHub URL for firefly-ui
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Andrew Richardson <andrew.richardson@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:36:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/55" class=".btn">#55</a>
            </td>
            <td>
                <b>
                    Firefly -> FireFly in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 20:19:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/54" class=".btn">#54</a>
            </td>
            <td>
                <b>
                    Rename kld query strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 19:41:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    initial docs library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nick Gaski <nick.gaski@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-09 19:10:09 +0000 UTC
    </div>
</div>

