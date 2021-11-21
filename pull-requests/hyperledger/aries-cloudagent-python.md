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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1504" class=".btn">#1504</a>
            </td>
            <td>
                <b>
                    Remove Streetcred references
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 16:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1501" class=".btn">#1501</a>
            </td>
            <td>
                <b>
                    Outbound Queue - more usability improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR improves the usability of outbound queues by:
- Fixing a bug where a queue instance was created twice when loading the class
- Add explicit startup and shutdown methods that are called in startup and shutdown of the conductor. This makes it so we can hold connections to external queues and give the outbound queue implementation the flexibility to determine how long those connections should live.
- Add `open` and `close` method to be used as `start` and `stop` were previously used. These methods are called by `aenter` and `aexit` on the base class and are therefore used each time a message is enqueued.
- All the `start`, `stop`, `open`, and `close` methods are now optional. If no special behavior is required, the inheriting class need not define an empty method.
- Outbound queue accepts a `Profile` instance for configuration instead of `Settings`. This allows the queue to subscribe to an publish events through the root profile.

This represents a BREAKING CHANGE in the outbound queue interface as the semantics of `start` and `stop` have been altered. Additionally, queue implementation init methods will need to be reconfigured to accept a profile instead of a settings object.

I think these changes, while breaking changes, go a long way towards improving the outbound queue interface and will better support a wider variety of external queue implementations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 02:56:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1500" class=".btn">#1500</a>
            </td>
            <td>
                <b>
                    Discover Features Protocol: v1_0 refactoring and v2_0 implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolves #1466
- v1.0 refactoring/rewrite - workflow should now be compliant with [RFC0031](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0031-discover-features)
Earlier implementation involved calling `/featues` endpoint [under `server` tag] to disclose protocols for that agent. It did not involve the flow of `Aries` messages as specified in the RFC.
- v2.0 implementation [RFC0557](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0557-discover-features-v2)

Major Changes
- Startup arguments
  - `--auto-disclose-features` Enables [proactive disclosure](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0557-discover-features-v2#requester) for v2.0. Such agent will automatically disclose features to another agent when an active connection gets established. `--disclose-features-list` can be used to limit what to disclose and if not specified, then all are disclosed.
  - `--disclose-features-list` Provides control over what features to publish. Accepts a path to YAML config file [example structure below]. This is valid for both v1.0 and v2.0
- Removed `/features under server` endpoint
- Added these endpoints:
  -  `discover-features` tag
     -  /discover-features/query
     - /discover-features/records
  -  `discover-features v2.0` tag
     - /discover-features-2.0/queries
     - /discover-features-2.0/records
- Added Controller class to protocols to specify, manage and load goal-codes
YAML config file structure, such agent will only disclose `did:sov:BzCbsNYhMrjHiqZDTUASHg;spec/action-menu/1.0` protocol and/or `aries.vc` goal-code
```
   protocols: ["did:sov:BzCbsNYhMrjHiqZDTUASHg;spec/action-menu/1.0"]
   goal-codes: ["aries.vc"]
```

Testing
- For v1.0, execute query using ` /discover-features/query`. If no `connection_id` is specified then it processes the query on the same agent (disclose features of the same agent). This essentially mimics what can be achieved using `/features` [under `server`]. To look up either all records or a record by `connection_id`, use `/discover-features/records`.
- For v2.0, execute queries using `/discover-features-2.0/queries`. Same logic when no `connection_id` is specified as above. To look up either all records or a record by `connection_id`, use `/discover-features-2.0/records`.
`connection_id` is an unique identifier for these records.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-17 17:21:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1496" class=".btn">#1496</a>
            </td>
            <td>
                <b>
                    Add RTD configs to get generator working
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Needed (I think) to get ReadTheDocs generation working again.  Currently not working because of a way that RTD works. Generation is no longer working because of a change in a default dependency, per [this bug report](https://gitanswer.com/build-failed-typeerror-generator-object-is-not-subscriptable-python-readthedocs-org-1036337375) and [guidance](https://docs.readthedocs.io/en/stable/guides/reproducible-builds.html#using-a-configuration-file).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 20:31:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1494" class=".btn">#1494</a>
            </td>
            <td>
                <b>
                    Fix TypeError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling /schemas/{schema_id}/write_record, a server error 500 occurrs. The log output says

    TypeError: inject() got an unexpected keyword argument 'required'

Other code in this file seems to indicate that the proposed change is what is needed to prevent the error from being thrown.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 12:37:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1493" class=".btn">#1493</a>
            </td>
            <td>
                <b>
                    DIF PresExch - ProblemReport and "is_holder"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - resolve #1486 
- review all tests involving `TEST_CRED_DICT` and `TEST_CRED_WILDCARD` with `FHIR` contexts to mock `pyld` returns.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 20:56:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1492" class=".btn">#1492</a>
            </td>
            <td>
                <b>
                    Aries Cloud Agent Python Release 0.7.2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 18:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1491" class=".btn">#1491</a>
            </td>
            <td>
                <b>
                    DIF PresExch Tests - temporary update to fix pyld.jsonld.JsonLdError
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a repeat of #1251 , then it started working without any updates after sometime.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-15 17:10:08 +0000 UTC
    </div>
</div>

