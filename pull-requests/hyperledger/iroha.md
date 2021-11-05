---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1578" class=".btn">#1578</a>
            </td>
            <td>
                <b>
                    [GHA] fix pretty version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                /build all

Signed-off-by: kuvaldini <ivan@kuvaldini.pro>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-04 14:45:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1576" class=".btn">#1576</a>
            </td>
            <td>
                <b>
                    Add endpoint for internal metrics for administration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                ### Description of the Change

### Issue
Close #1387

### Benefits

### Possible Drawbacks
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 16:47:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1575" class=".btn">#1575</a>
            </td>
            <td>
                <b>
                    Fix the push pipeline.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Signed-off-by: Aleksandr <a-p-petrosyan@yandex.ru>


### Description of the Change

Fix the Docker pipeline to work on `push`. 

### Issue

Unable to push github docker images. 


### Benefits

Able to push docker images from CI

### Possible Drawbacks

None
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 10:03:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1574" class=".btn">#1574</a>
            </td>
            <td>
                <b>
                    Reconnect telemetry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Alexey Kalita <kalita.alexey@outlook.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
If telemetry fails to send a message, the node is going to reconnect in a few seconds.
While the telemetry is down, messages are skipped.
The period between reconnects can be customized with MIN_PERIOD and MAX_POWER
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Issue

Closes #1546 

<!-- If it is not a GitHub issue but a JIRA issue, just put the link here -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 09:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1573" class=".btn">#1573</a>
            </td>
            <td>
                <b>
                    refactor of the `p2p` crate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">refactor</span>
            </td>
            <td>
                ### Description of the Change

`p2p` crate refactoring. 

### Issue

#1171 

### Benefits

Peer now has several dependent datatypes: `Connection` and `Cryptographer<T, K, E>`, which make the depedency graph clearer. 

The `handshake` method either returns a `State::Ready` peer or terminates. 

The handler can no longer end up in an infinite loop if `handshake()` method returns anything other than a peer in `State::Ready`. 

The `State::Error` peer now records the error. 

Error handling is (mostly) monadic. 

The state `enum` now only derives `Debug`, which should reduce compilation time. 

Each stage of the handshake now asserts that it came from the previous stage, and raises an `Error::Handshake` if it didn't. Trivial handling of this error is to change the `peer.state`. 

### Possible Drawbacks

None known. 

### Alternative implementations. 

Turning `peer` into an enum necessitates one of several modifications. The `impl Peer` needs to pass by value and take ownership of the data, of which neither TCPStream nor the cryptographic primitives can be cloned. As a result each function has the potential of losing the peer entirely on error. This precludes recovery. 

Additionally, most functions upon which `handshake` depends, pass by mutable reference which means that they cannot change the `enum` variant themselves, and neither can `handshake`. To get around this issue we could swap into `self` a Dummy varialbe, and change the freed copy based off of the new information. This 1) making the code more obtuse, 2) requires creating a dummy default constructable peer, which would be equivalent to it being nullable, 3) does not communicate the intention more clearly. 

Moving all state except `broker` and `id` into the `enum` state has the benefit of clarifying that at certain stages the peer doesn't have to have certain types of data. However, because the state needs to be changed, said data (which is not `Clone`), will need to be moved into dummy variables of the same type, which has the same result as making `peer` an `enum`. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 06:48:23 +0000 UTC
    </div>
</div>

