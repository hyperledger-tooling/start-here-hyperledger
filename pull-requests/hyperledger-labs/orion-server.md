---
layout: default
title: orion-server
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/orion-server
---

# orion-server <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/orion-server){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    documentation updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 12:31:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    decoder decodes data response envelope
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commits add a decoder utility that would decode
a given json data response envelope.

It will get updated to decode the bas64 encoded value
in the subsequent PR.

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-18 08:58:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/261" class=".btn">#261</a>
            </td>
            <td>
                <b>
                    Storing all sample configuration files to same folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Configuration files for local executable, for docker and all certificates moved to same folder (deployment),
subfolder for each type.

Updated docker to have 3 separate volumes - one for configuration, one for crypto and one for ledger.

Signed-off-by: Gennady Laventman <gennady@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 21:04:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    Calculate max-raft-id from members when committing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                The MaxRaftId field in RaftConfig records the highest raft-id ever seen in the cluster.
We calculate it from the members as we build the genesis block, and from then on it is
updated every time a config block commits. The incoming config-tx does not change this value,
and it must be equal to value in the current config. Users can only read this value.
This field is used to ensure that the raft id of added new peers is larger then the current
max-raft-id, and was therefore never used.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 12:12:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/256" class=".btn">#256</a>
            </td>
            <td>
                <b>
                    encoder for value
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This commit adds an utility that can encode the given data to
base64 string. Note that this utility accepts either a JSON or
string value only.

Signed-off-by: senthil <cendhu@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-16 08:50:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/orion-server/pull/249" class=".btn">#249</a>
            </td>
            <td>
                <b>
                    TLS support for comm
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">replication</span>
            </td>
            <td>
                Support TLS for peer server to server communication.
The server accepts only TLS connections, the client dials TLS.
Client authentication is not yet supported (future commit).
Client authorization is not yet supported (future commit).

Some utilities where added to load the CA certificates from disk, verify them,
and pack then all into a single bundle, as the rafthttp transport expects.

Signed-off-by: Yoav Tock <tock@il.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-14 11:02:05 +0000 UTC
    </div>
</div>

