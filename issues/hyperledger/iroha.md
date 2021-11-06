---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1529" class=".btn">1529</a>
            </td>
            <td>
                <b>
                    Record fields in all logs instead of formatting them
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Now that we have a possibility to output structured logging it is needed to make our logs good for that format. Where possible we should use [log fields](https://docs.rs/tracing/0.1.29/tracing/#recording-fields) instead of usual Rust formatting.

Example instead of `info!("Created block with hash: {}", hash)` it should be `info!("Created block", hash)`. 

While some places are already in the later format, some are still not updated currently.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-18 13:43:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1511" class=".btn">1511</a>
            </td>
            <td>
                <b>
                    Define maximum read buffer size for blocks deserialization in Kura
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                In kura.rs:read_block we currently allocate buffer for data before VersionCommittedBlock deserialization. Buffer size is read from the file and, in case it's malformed, might be huge and we'll panic. 
As a temporary solution, there's a local constant BUFFER_SIZE_LIMIT = 500Kb, which limits maximum sane buffer size. Otherwise we'll throw.

This solution is too rigid. We should think of a more controllable/configurable way of setting this limit.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 11:36:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1315" class=".btn">1315</a>
            </td>
            <td>
                <b>
                    Peer responded with QueryResult instead of VersionedQueryResult
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                When client sends request to endpoint /query, it expects as result `VersionedQueryResult`, but the peer returns `QueryResult`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-05 06:33:19 +0000 UTC
    </div>
</div>

