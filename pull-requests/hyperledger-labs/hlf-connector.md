---
layout: default
title: hlf-connector
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-connector
---

# hlf-connector <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-connector){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/72" class=".btn">#72</a>
            </td>
            <td>
                <b>
                    Increment version after release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">auto-version-increment</span>
            </td>
            <td>
                Automated changes by [create-pull-request](https://github.com/peter-evans/create-pull-request) GitHub action
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-26 08:39:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Process Data-ingestion messages through Batched async mechanism to improve throughput.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Current Problem :** 
Presently, only a single Listener container is generated to consume messages from the Connectors ingestion Topic (across all the partitions) . This Listener sequentially processes each record returned by the internal ```poll()``` method which eventually affects the overall throughput of Connector, since the downstream ```TransactionConsumer#listen``` does a blocking call for writing transactions which could span for few seconds. 
Therefore given a scenario where ```TransactionConsumer#listen``` takes 2 seconds complete, in order to process 100 incoming records fetched by the ```poll()``` method it takes around 50 seconds. 

 **Proposed Fix :** 
Assign a dedicated Listener Container for each partition in the Topic, per connector instance (capped to a max of 6 Listeners, in order to avoid spawning a large number of Listeners for high-partitioned Topics ).
Each Listener gets a batch of Messages from the Partition it is assigned to, this batch is processed asynchronously by submitting it to a task executor in one go. The Listener thread defers the next poll until the entire records are processed parallelly. Once the batch is processed, Listener gets the next Batch from poll()
In case one of the records encounters an exception while processing parallelly, we perform a partial Batch commit and the failed and unprocessed records are sent again in the next poll()
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-26 08:12:47 +0000 UTC
    </div>
</div>

