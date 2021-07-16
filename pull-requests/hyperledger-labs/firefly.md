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
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/131" class=".btn">#131</a>
            </td>
            <td>
                <b>
                    Create CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-15 14:10:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Rename topic field to topics
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In a message header, previously there was a field named `topic` but it was of type `[]string`. It makes more sense to call this field `topics` because it is a list of several topic names. This PR changes this, but it is important to note that this is an API breaking change (though small in size).

Example message:

```json
{
  "header": {
    "tag": "new_widget_created",
    "topics": ["widget_id_12345"]
  },
  "data": [
    {
      "value": {
        "id": "widget_id_12345",
        "name": "superwidget"
      }
    }
  ]
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 19:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/128" class=".btn">#128</a>
            </td>
            <td>
                <b>
                    Update addressable in Gemfile.lock for vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See https://github.com/hyperledger-labs/firefly/security/dependabot/docs/Gemfile.lock/addressable/open
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 03:47:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    Latency optimize event delivery by default
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Early adopter feedback suggests that latency of event delivery is more important than throughput optimization, in the most common scenarios. Particularly in non-blockchain backed event scenarios, and even more in request/reply scenarios.

Currently we use a 250ms default latency on event delivery, to reduce pressure on the DB in high throughput scenarios by giving time for messages to arrive between queries.

This PR proposes making the default 0, optimizing for latency by default (before we cut the first release).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-14 03:16:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Database events across all objects
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #109 

- Doesn't include docs - need to do reference docs for WebSockets to cover the new `&changeevents=.*` option
- Updates e2e test with change events - turned on for all tests, so they're chatty, but hopefully that makes it easier to debug if they fail too
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-12 04:53:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/125" class=".btn">#125</a>
            </td>
            <td>
                <b>
                    Remove QL pure Go database, in favour of SQLite - pure Go and CGO
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Goodbye QL 😢 , Hello SQLite 🚀 

When we originally built FireFly's SQL implementation, the pure Go SQLIte implementation was not supported by the `goland-migrate` package.

As we wanted unit tests to be able to fully verify the SQL database layer with a real database, we introduce [QL](https://pkg.go.dev/modernc.org/ql) as a database that was supported by the migration tool.

Along the journey, we also added a super trivial "fake" blockchain interface for some early experimentation that worked on top of this.

Since then we've learned:
- QL is missing large pieces of functionality that we had to work around
  - A full types system
  - Individual column sorting
  - A "normal" column that can be auto-incremented as an ID (worked around with an `id(tableName)` function
  - Database triggers (see #109)
- The QL transaction model is very limited
  - Seems to only support one active transaction
  - When not used fully in line with the model, it results in deadlocks (rather than errors)
- QL 

This lead to code complexity to work around the limitations in unit tests, and also some costly investigations when attempts were made to use QL outside of the unit tests in a full FireFly runtime environment.

Now [golang-migrate](https://github.com/golang-migrate/migrate/tree/master/database/sqlite) has support of the pure Go implementation, I propose this PR to *completely remove all traces of QL* from the codebase.

We think it would be the wrong thing for anyone to pick up QL with FireFly, compared to the much more mature SQLite technology - which now has all the same non-functional characteristics (in process execution, option of a pure Go implementation as required)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 18:00:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Add support for tokens
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
        Created At 2021-07-09 16:44:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/firefly/pull/122" class=".btn">#122</a>
            </td>
            <td>
                <b>
                    E2E Enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves https://github.com/hyperledger-labs/firefly/issues/121

This PR adds the ability to run the E2E tests against any FireFly environment. If someone wants to run the tests against a remote FireFly (not on their local dev machine) they will need to create or modify a `stack.json` file to add some new fields that are not currently added by the CLI. These changes are still backwards compatible with existing `stack.json` files created by the CLI.

Here's an example of a new `stack.json` file that points to remote FireFly instances and also uses HTTPS and basic authentication.
```json
{
 "name": "dev",
 "members": [
  {
   "id": "0",
   "index": 0,
   "address": "0xac9c1260fb2ad017de65ce7cf68c0142903357ab",
   "privateKey": "0x02e9b8465ea1b585c2050b1fdf2fbe642c92b74192a0fb6f403ce2d91b5f5fdc",
   "exposedFireflyPort": 443,
   "exposedFireflyAdminPort": 5101,
   "exposedEthconnectPort": 5102,
   "exposedPostgresPort": 5104,
   "exposedDataexchangePort": 5105,
   "exposedIPFSApiPort": 5106,
   "exposedIPFSGWPort": 5107,
   "exposedUiPort ": 5103,
   "fireflyHostname": "zzglm93oa9-zzpl2jzg7u-firefly-os.dev2-ws.photic.io",
   "username": "username1",
   "password": "super-secret-password1",
   "useHttps": true
  },
  {
   "id": "1",
   "index": 1,
   "address": "0xd3ecae28b94b67c3b1651aa6c2efead818b3fca1",
   "privateKey": "0x49733950a87b2d78e6fd768057ccdcf7d957028f7b1fb50b405505d2495d11dd",
   "exposedFireflyPort": 443,
   "exposedFireflyAdminPort": 5201,
   "exposedEthconnectPort": 5202,
   "exposedPostgresPort": 5204,
   "exposedDataexchangePort": 5205,
   "exposedIPFSApiPort": 5206,
   "exposedIPFSGWPort": 5207,
   "exposedUiPort ": 5203,
   "fireflyHostname": "zzglm93oa9-zzmxfv7oo0-firefly-os.dev2-ws.photic.io",
   "username": "username2",
   "password": "super-secret-password2",
   "useHttps": true
  }
 ],
 "swarmKey": "/key/swarm/psk/1.0.0/\n/base16/\n1d699874aebc4e2f4f5ca66346f6e1048a9e5be639a60b374136a0c2b012f5f2",
 "exposedGanachePort": 5100
}
```


This PR also includes two other, unrelated fixes to database transaction contexts and logging. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-09 16:20:54 +0000 UTC
    </div>
</div>

