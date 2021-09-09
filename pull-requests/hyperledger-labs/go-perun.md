---
layout: default
title: go-perun
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/go-perun
---

# go-perun <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/go-perun){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/go-perun/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    174 Implement local watcher
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Overview

- This PR implements the server side component local watcher as per the design described in [proposal#4](https://github.com/hyperledger-labs/perun-proposals/blob/main/design/004-IoT-Adoption-Watcher.md). 
- This component should be initialized by the user of the framework and pass it as an argument to the `client.New` API.

### Implementation details

- The interface definitions are located in a package: `go-perun/watcher`.
- The implementation of local watcher is located in a `go-perun/watcher/local`.

#### Data structures

1. **Watcher**: 
    - This represents the watcher instance, initializes using the `NewWatcher` function.
    - It contains 
        - `channel.RegistererSubscriber` instance for interacting with the blockchain.
        - `registry` that holds a map of all the channels currently registered with the Watcher.
    - Both the above data structures are safe for concurrent use.

2. **ch**:
    - Represents the data corresponding to a channel.
    - It contains
        - `id` of the channel.
        - `params` of the channel. Required while registering dispute for the channel. This will be passed when registering the channel with the `Watcher` via `StartWatching` function.
        - `parent` of this channel. For ledger channels, this is set to `channel.Zero`.

        - `subChsAccess`, (relevant only for ledger channel) a mutex used for concurrency safe access of a family of channels. When a dispute registration is required for a channel, we traverse back to the parent and lock this mutex. It is unlocked only after the dispute registration is completed. This also ensures, we lock only the relevant channels and not the entire registry when registering disputes.

        - `registeredVersion`: when a dispute is registered for a ledger, sub or virtual channel, this field is updated. This is used to ensure, we do not register the same version more than once.
        - `requestLatestTx` and `latestTx` are a set of channels used for retrieving the latest state of this channel without use of mutex locks.

3. **registry**: Used to store and retrieve channels registered with the watcher. It is protected by a mutex.

4. **StatesPubSub** and **AdjudicatorPubSub** implements the functionalities exactly as described in the proposal.
        
#### Methods

1. `NewWatcher` initializes the watcher.
2. `Watcher.StartWatchingForLedgerChannel` and Watcher.StartWatchingForNonLedgerChannel` APIs are used to register a channel with the watcher. Though the implementations of both the APIs are same, two APIs are provided because
    - LedgerChannel does not require parent while,
    - Sub-Channel requires a parent.
    - Regarding the names, I also think we need a better name, used this for time being. 
3. `AdjudicatorSub.Next` can be used by the client for receiving adjudicator events from the watcher.
4. `StatesPub.Publish` can be used by the client to send newer transactions to the watcher.
5. `Watcher.StopWatching` and `Watcher.Shutdown` are yet to implemented.

#### Tests

It was difficult for me to figure out how to add tests using the simulated backend. Particularly, I couldn't figure out how to make the watcher send events to the watcher.

However, I implemented some tests based on generated mocks. This covers both happy path and most of the corner cases. I used these to guide my development. I have added them in the PR (in separate commits). If it is possible, we could replace them with tests using simulated backend or remove them (if they don't fit the testing style used in the project).

#### Resolves #174
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-09 17:53:48 +0000 UTC
    </div>
</div>

