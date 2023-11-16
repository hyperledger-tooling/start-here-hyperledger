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
                PR <a href="https://github.com/hyperledger-labs/hlf-connector/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    Introduce capability for publishing error Records to Dead letter topic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR contains the changes for publishing failed consumer Records polled from the Integration topic(s) to a configured error Event listener Topic.

The changes would effectively allow the Connector to publish the Error record to a topic based on the following criteria :-

- If the Event-Listener topic (Block & Chaincode) has the optional field `listenToFailedMessages` set as true, the failed message will be published back to Event listener topic (this is the current behaviour).
- If the Kafka properties of a dedicated Dead letter topic is configured, the errored message will be published to the configured dead letter topic.
- If the configuration `listenToFailedMessages` is set to true as well as a dedicated Dead letter topic is configured, the dead letter topic will take priority and record will be dispatched to it.
- If none of the above options are available, the listener will attempt retries and log the failed record by committing the offset.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-16 09:46:07 +0000 UTC
    </div>
</div>

