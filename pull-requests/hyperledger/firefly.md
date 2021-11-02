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

