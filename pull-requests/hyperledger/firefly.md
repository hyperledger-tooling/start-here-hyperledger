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
                PR <a href="https://github.com/hyperledger/firefly/pull/299" class=".btn">#299</a>
            </td>
            <td>
                <b>
                    Add `?fetchdata` on messages collection to include data, and make consistent with get by ID
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Deprecates existing `data` query param on `/messages/:id`
- Adds consistent `fetchdata` query param on both `/messages` and `/messages/:id`
- Bit of restructuring in line with recent directions on code style around use of `bool` params
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-27 13:16:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/298" class=".btn">#298</a>
            </td>
            <td>
                <b>
                    Add check before writing to websocket channel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is supposed to fix https://github.com/hyperledger/firefly/issues/265

I'm not 100% sure my unit test accurately reproduces the exact situation we're running into in that issue though. Adding the extra check does indeed make this test pass. However, I'm not sure we can count on `ws.closed` to be set correctly 100% of the time before writing to the channel. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 21:13:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/297" class=".btn">#297</a>
            </td>
            <td>
                <b>
                    Only send transfer message if token transfer is successful
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a rework of #279 - please see the original notes on that PR, which still apply here.

Falls under architecture item #218.

It contains the commits from #283 and #296 as pre-requisites, so those should be reviewed first. Only the last 2 commits are net new code.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 20:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/296" class=".btn">#296</a>
            </td>
            <td>
                <b>
                    Collapse message bools into a new "state" field
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This needs a careful look. It's not a particularly large change, but it does alter the fundamental flags we use
for message transmission and ordering. E2E tests are good and the UI looks sane to me, but I'm happy to test
anything else that might be needed.

Currently (prior to this change), the `messages` table has 3 boolean fields: `local`, `pending`, and `rejected`.
These are use to determine when a message needs to be sent and when it has been confirmed or rejected.

With the new change, these are collapsed into a single `state` enum with 4 values: `ready`, `pending`,
`confirmed`, `rejected`. I think this is cleaner overall and allows for defining new states as well.

Side note on ordering: we want to be able to list messages in an order that shows `pending` messages first
(ordered by creation time descending) and then all confirmed/rejected messages interleaved (ordered by
confirmation time descending). The separate `pending` bool was being used to enable this search, but now
the query is entirely based upon the `confirmed` timestamp field, with a `NULLS FIRST` suffix to ensure the
pending items are ordered first.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 19:41:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/295" class=".btn">#295</a>
            </td>
            <td>
                <b>
                    Fix duplicate db migration 00037
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
        Created At 2021-10-26 18:34:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/294" class=".btn">#294</a>
            </td>
            <td>
                <b>
                    Add jobs for database migration and auto-registration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds a couple of simple jobs, with configuration options to enable them:

- `config.postgresMigrationJob: true`
   - Creates a k8s Job to perform the migrations, which runs on each new FireFly tag deployed
- `config.registrationJob: true`
    - Creates a k8s Job to ensure registration is performed, which runs once (unless the org name changes)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 18:26:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/292" class=".btn">#292</a>
            </td>
            <td>
                <b>
                    Add scheduled E2E test using latest services
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
        Created At 2021-10-26 15:06:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/290" class=".btn">#290</a>
            </td>
            <td>
                <b>
                    Add topic+tag index to messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The intention of the topics field, is that you can create a stream of data that is grouped on a particular ordered business context, and the tag sub-classifies messages within that.

This means that querying by topic and tag is a primary use case, for which index(es) should exist.

This PR proposes a single combined index, on topic then tag, as I believe that's the most likely combination of filter across use cases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 12:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/289" class=".btn">#289</a>
            </td>
            <td>
                <b>
                    Fix PSQL migration with invalid AUTOINCREMENT
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hit the following error running the migrations in `v0.10.1-20211025-7`:

```
1/u create_messages_table (69.483333ms)
2/u create_data_table (136.900657ms)
3/u create_message_data_join_table (171.928524ms)
4/u create_batches_table (226.524985ms)
5/u create_transactions_table (280.778146ms)
6/u create_datatypes_table (326.177263ms)
7/u create_offsets_table (360.316827ms)
8/u create_operations_table (415.27669ms)
9/u create_namespaces_table (451.860266ms)
10/u create_subscriptions_table (496.59108ms)
11/u create_events_table (533.731258ms)
12/u create_pins_table (503.899115ms)
13/u create_orgs_table (482.438813ms)
14/u create_nodes_table (498.472389ms)
15/u create_config_table (487.192335ms)
16/u create_groups_table (465.819233ms)
17/u create_members_table (458.316196ms)
18/u create_nonces_table (460.794609ms)
19/u create_nextpins_table (442.013818ms)
20/u create_messages_pending (433.319376ms)
21/u create_data_blob (445.455735ms)
22/u create_blobs_table (446.289939ms)
23/u alter_subscriptions_offsets (431.96207ms)
25/u create_tokenpool_table (440.276511ms)
27/u add_operations_input (409.269762ms)
28/u add_tokenpool_fields (387.214256ms)
29/u add_tokenpool_created (375.234798ms)
30/u create_key_fields (359.340222ms)
31/u create_tokentransfer_table (370.982178ms)
error: migration failed: syntax error at or near "AUTOINCREMENT" (column 48) in line 5: BEGIN;
DROP TABLE IF EXISTS tokenaccount;

CREATE TABLE tokenaccount (
  seq              INTEGER         PRIMARY KEY AUTOINCREMENT,
  pool_protocol_id VARCHAR(1024)   NOT NULL,
  token_index      VARCHAR(1024),
  identity         VARCHAR(1024)   NOT NULL,
  balance          VARCHAR(65)
);

CREATE UNIQUE INDEX tokenaccount_pool ON tokenaccount(pool_protocol_id,token_index,identity);

COMMIT;
 (details: pq: syntax error at or near "AUTOINCREMENT")
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 04:14:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/288" class=".btn">#288</a>
            </td>
            <td>
                <b>
                    Fix image repos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Helm chart still had `-labs` in the names
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-26 02:58:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/287" class=".btn">#287</a>
            </td>
            <td>
                <b>
                    Add namespace field to token accounts and transfers
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
        Created At 2021-10-25 20:14:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/286" class=".btn">#286</a>
            </td>
            <td>
                <b>
                    Update GitHub actions to build every merge to main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a new GitHub action to build a docker image for every merge to `main`, but it is not designated as a "release" on GitHub. This allows us to use and test any commit, but won't clutter up our releases page. The image will be tagged with a date-stamped release number, and the newest build will also be tagged with `head`. This means if someone wants the latest, bleeding edge build of firefly, the can just pull `docker pull ghcr.io/hyperledger/firefly:head` and they will get whatever is the latest commit in `main.

The images area also labeled (separate from being tagged) with the Git commit that they were built from, as well as the date and build number.

The `manifestgen.sh` script also gets an update with this, allowing it to pull the `head` tag for all services and create a `manifest.json` with those images. To do this, run:

```
./manifestgen.sh head
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 19:47:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/285" class=".btn">#285</a>
            </td>
            <td>
                <b>
                    Update DX dependency, and go deps including bluemonday for CVE-2021-42576
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updates dependencies for security issues
- Pulls in all the latest images of downstream deps
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-25 15:24:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/284" class=".btn">#284</a>
            </td>
            <td>
                <b>
                    Update docs and add new guides
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Contributor's Guide has seen some meaningful updates in this PR. There are some additional, brand new guides added here too.

Relevant changes can be previewed here:

- Contributor's Guide: https://nguyer.github.io/firefly/contributors/contributors.html
- Contributing to Documentation: https://nguyer.github.io/firefly/contributors/docs_setup.html
- Advanced CLI Usage: https://nguyer.github.io/firefly/contributors/advanced_cli_usage.html
- Versioning Scheme: https://nguyer.github.io/firefly/maintainers/version_scheme.html
- Release Guide: https://nguyer.github.io/firefly/maintainers/release_guide.html
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 20:23:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/283" class=".btn">#283</a>
            </td>
            <td>
                <b>
                    Replace BeforeSend callback with a Prepare method
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This instructs the sender to prepare the message for sending, but return before
actually sending it. Re-invoking Send or SendAndWait on the same sender should
dispatch the prepared message.

Further aligned methods between transfers and messaging for consistency.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-22 16:05:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/280" class=".btn">#280</a>
            </td>
            <td>
                <b>
                    pools-by-connector Add connector field to TokenPoolQueryFactory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support the new [Tokens Page in the UI](https://github.com/hyperledger/firefly-ui/issues/65), filtering that supports getting pools by connector is needed

```GET /namespaces/<namespace>/tokens/pools?connector={connectorName}``` returns all token pools with specified connector
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 15:36:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    tokens-by-id getTokenPoolByNameOrID() and getTokenTransfersByID()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To support the new [Tokens Page in the UI](https://github.com/hyperledger/firefly-ui/issues/65), an endpoint to get token pools by name or ID and to get token transfers by ID is needed.

```GET /namespaces/<namespace>/tokens/pools/{nameOrID}``` returns all token pools with specified name or ID
```GET /namespaces/<namespace>/tokens/transfers/{transferID}``` returns token transfer with specified ID
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-21 01:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    introduce FFTime.Time()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - Converts FFTime -> Time
 - some misc. changes my linter pointed out
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-20 20:25:07 +0000 UTC
    </div>
</div>

