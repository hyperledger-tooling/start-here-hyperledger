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
                PR <a href="https://github.com/hyperledger/iroha/pull/1329" class=".btn">#1329</a>
            </td>
            <td>
                <b>
                    refactor(irohad): add config order ENV -> FILE
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes it possible to change the precedence order via
the passing in of a new flag called --legacy_config_precedence
which takes a boolean true/false and defaults to true in order
to make this change backwards compatible.

In order to override the pg creds via the enviornment variables
you need to do two things:
1. Specify the postgres credentials via environment variables
2. Pass in to the irohad binary the --legacy_config_precedence=false
command line argument when starting it.

Fixes #1314

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

<!-- ### Requirements -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

### Benefits

Flexibility in containerized environments where the config file is set at build time and tricky to change.

### Possible Drawbacks

People may get confused  by the additional flag I had to add to maintain backwards compatibility, but I wanted to make sure it's not a breaking change.

### Usage Examples or Tests *[optional]*

Shell 1

```sh
docker run --rm -p 5432:5432 -e POSTGRES_PASSWORD=x postgres:9.5
```

Shell 2

```sh
IROHA_POSTGRES_HOST=127.0.0.1 IROHA_POSTGRES_PORT=5432 IROHA_POSTGRES_USER=postgres IROHA_POSTGRES_PASSWORD=x IROHA_POSTGRES_DATABASE=postgres IROHA_POSTGRES_MAINTENANCE_DATABASE=postgres  ./build/bin/irohad --config ./example/config.sample --verbosity=trace --legacy_config_precedence=false
```

Then you can observe that it connects to the postgres that was specified in the environment variables which was the point.
You can also observe that if you omit the `--legacy_config_precedence=false` flag or say `--legacy_config_precedence=true` instead then it reverts back to ignoring the env variables for the legacy behavior for those who need it.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-11 00:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1328" class=".btn">#1328</a>
            </td>
            <td>
                <b>
                    Docs: General Metrics Part II
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Sara <lira.lemur@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

Second try of the https://github.com/hyperledger/iroha/pull/1299

General information about metrics

### Benefits

Metrics in docs

### Possible Drawbacks

Not very full info. Yet.

Closes #1280 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-10 09:12:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1327" class=".btn">#1327</a>
            </td>
            <td>
                <b>
                    [OS] batches cache + small block fixup
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Avoids small blocks on a high load.

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

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
        Created At 2021-08-10 07:33:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1326" class=".btn">#1326</a>
            </td>
            <td>
                <b>
                    Add commands and queries to burrow integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
Adds Iroha commands and queries to burrow integration
Examples for the integration have also been added
List of commands/queries integrated:
1)Add Asset
2)Add Peer
2)Add signatory
4)Append Role
5)Create Account
6)Create Asset
7)Create Domain
8)Detach Role
9)Remove peer
10)Remove Signatory
11)Set Account Detail
12)Set Account Quorum
13)Subtract Asset
14)Transfer Asset
15)Get Account
16)Get Block
17)Get Signatories
18)Get Account Asset
19)Get Account detail
20)Get Asset Info
21)Get Role
22)Get Role Permissions
23)Get Peers



<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits
This will extend HL Burrow integration into HL Iroha , so more commands can be used
<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks
All the commands and queries haven't been integrated like GrantPermission and GetAccountTransactions, etc.
<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests 
Examples have been added under /example/burrow_integration
<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->



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
        Created At 2021-08-09 17:52:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1325" class=".btn">#1325</a>
            </td>
            <td>
                <b>
                    Introduces multiple broker fixes 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Egor Ivkov <e.o.ivkov@gmail.com>

<!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change
1. Unsubscribe from broker on actor stop
2. Support multiple subscriptions from the same actor type (previously a TODO)
3. Fixes a bug where broker always put self as an actor id.
<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Broker Bug

#### Demo Test Case
Check out `Broker bug - test showcase` commit and run the tests added there - you will notice it fails.
The test case just tries to send a message of one type to two subscribers - should be perfectly okay logically.

#### Bug Description
Broker in the function `subscribe_recipient` adds self in the place, where I deduce should have been an actual actor type id. Therefore as this place always contains one value - type id of the broker - when several actors/channels subscribe to one message type - only the first actor/channel that subscribed to it will receive it.

While the *expected behavior* is for all actors that subscribed to the same message type to receive this message when it is published.

#### Place in code of this bug
```rust
impl Broker {

    // ... code ..

    fn subscribe_recipient<M: BrokerMessage>(&self, recipient: Recipient<M>) {
        let mut entry = self
            .message_entry(TypeId::of::<M>())
            .or_insert_with(|| Vec::with_capacity(1));
        if entry
            .iter()
            .any(|(actor_id, _)| *actor_id == TypeId::of::<Self>()) // BUG!
        {
            return;
        }
        entry.push((TypeId::of::<Self>(), Box::new(recipient))); // BUG!
    }

    /// Subscribe actor to specific message type
    pub fn subscribe<M: BrokerMessage, A: Actor + ContextHandler<M>>(&self, ctx: &mut Context<A>) {
        self.subscribe_recipient(ctx.recipient::<M>()) // Notice how `A` actor type is not used at all
    }

    /// Subscribe with channel to specific message type
    pub fn subscribe_with_channel<M: BrokerMessage + Debug>(&self) -> mpsc::Receiver<M> {
        let (sender, receiver) = mpsc::channel(100);
        self.subscribe_recipient(sender.into());
        receiver
    }
}
```

<!--
NOTE: User may want skip pull request and push workflows with [skip ci]
https://github.blog/changelog/2021-02-08-github-actions-skip-pull-request-and-push-workflows-with-skip-ci/
Phrases: [skip ci], [ci skip], [no ci], [skip actions], or [actions skip]
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-08-09 17:24:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/1320" class=".btn">#1320</a>
            </td>
            <td>
                <b>
                    [RDB] migration-tool
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CircleCI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

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
        Created At 2021-08-06 07:32:47 +0000 UTC
    </div>
</div>

