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
                Issue <a href="https://github.com/hyperledger/iroha/issues/2056" class=".btn">2056</a>
            </td>
            <td>
                <b>
                    Create a iroha procedural macro for impl FromStr for AssetValueType and other C like enums
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                The following macro invokation
```
easy_from_str_impl! {AssetValueType, Quantity, BigQuantity, Fixed, Store}
```

does not automatically generate code for all variants. This should be replaced with a custom derive macro for FromStr.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 16:20:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2053" class=".btn">2053</a>
            </td>
            <td>
                <b>
                    Unit test the `private_blockchain` permissions validators
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Tests</span>
            </td>
            <td>
                At present we don't have any unit tests for the `private_blockchain` use case. It would be important to include them in the test coverage of the integration tests. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-04 08:42:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2047" class=".btn">2047</a>
            </td>
            <td>
                <b>
                    Add `non_zero` numeric types where acceptable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Optimization</span>
            </td>
            <td>
                Discriminant elision may sometimes be effected if the underlying type has a [niche](https://github.com/rust-lang/unsafe-code-guidelines/blob/master/reference/src/layout/enums.md). This fact can be exploited to save one machine word's worth of space in enumerations which are option-like (i.e. can be discriminated using a single bit). 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-01 12:33:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2035" class=".btn">2035</a>
            </td>
            <td>
                <b>
                    Add macro to remove boilerplate from `client/tests/integration`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                ```rust
    let (_rt, _peer, mut test_client) = <TestPeer>::start_test_with_runtime();
    wait_for_genesis_committed(&vec[test_client.clone()], 0);
```

is repeated at the top of almost every test. 

We should have a proc-macro `#[integration]` which adds this boilerplate, but allows specifying the number of peers, the genesis, the configuration options and a few other things. 

#### Optional 

Remove the `start_test_with_runtime` and replace it with the most general `fn` from `test_network`. Instead use the `proc_macro` args to add optional customisation. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-30 07:27:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2017" class=".btn">2017</a>
            </td>
            <td>
                <b>
                    Integration test to check if role is removed from accounts after burning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Tests</span>
            </td>
            <td>
                There was a bug, when role was removed only from domain and not from accounts. This is fixed in #1984. Now we need a test for it
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-28 10:36:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2009" class=".btn">2009</a>
            </td>
            <td>
                <b>
                    Create an easy way to register trigger using `Client`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                 Most of our downstream clients may want a feature to easy register trigger. So it should be a new method in `Client` structure. It should be looking something like `build_register_tirgger_isi()` in `client/tests/integration/triggers/*`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 11:29:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2007" class=".btn">2007</a>
            </td>
            <td>
                <b>
                    Grant and revoke role emit `PermissionAdded`/`PermissionRemoved` events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">good first issue</span><span class="chip">question</span><span class="chip">iroha2</span>
            </td>
            <td>
                take a look at `smartcontracts/isi/account.rs` implementation of `Execute` for grant/revoke of `Role` and you will see that permission events are returned for granting and revoking both roles and permission tokens. Is this fine?

Also `PermissionRemoved` event is emitted in `Unregister<Role>` in `smartcontracts/isi/domain.rs`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-25 07:42:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2004" class=".btn">2004</a>
            </td>
            <td>
                <b>
                    Compile time checking for architecture dependent types on serialized structures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                It would be useful to have compile time checks that ensure our serialized and deserialized types are identical across architectures so that we don't reintroduce fields containing eg usize/isize in future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-24 19:47:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/2000" class=".btn">2000</a>
            </td>
            <td>
                <b>
                    Disallow empty `Identifiers`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span><span class="chip">iroha2</span>
            </td>
            <td>
                At the moment it is allowed to create empty `Name`, `DomainId`, `AccountId`, etc. Should we continue to allow empty string identifiers or should we forbid them. What about using `Option`? 

It should be noted that empty string is a well defined identifier
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 08:14:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1996" class=".btn">1996</a>
            </td>
            <td>
                <b>
                    Move `GenesisDomain` and `GenesisAccount` to `iroha_core`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Currently, genesis domain and account are in `iroha_data_model`. It is my understanding that they are only used in `iroha_core` and should in fact not be presented to the user through data model API. Therefore, they should be moved into `iroha_core`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 14:39:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1995" class=".btn">1995</a>
            </td>
            <td>
                <b>
                    `serde` validation hook in deserialize
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                It is quite often that we need to write custom `serde::Deserialize` implementations just to validate structure's invariants. If possible, we should write some sort of a hook into serde macro system that would take validation function and generate deserialize implementation for a struct. 

Also, maybe there is some crate offering this functionality or it can be done with serde.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 13:24:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1992" class=".btn">1992</a>
            </td>
            <td>
                <b>
                    Consolidate supporting tools in the `tools` folder of the project. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Iroha is shipped with multiple supporting binaries that can be classified as tools. 

I propose moving 
- iroha_docs
- iroha_crypto_cli
- iroha_schema_bin

into the `tools` folder in the project. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 06:45:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1990" class=".btn">1990</a>
            </td>
            <td>
                <b>
                    Support running Iroha without `config.json` using pure environment variables. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-22 05:48:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1988" class=".btn">1988</a>
            </td>
            <td>
                <b>
                    `PartialEq` and `PartialOrd` of `Identifiable` structures 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Identifiable structures, such as `Domain`, derive their implementation of `PartialEq`, but have the following implementation of `PartialOrd`:
```rs
impl PartialOrd for Domain {
    #[inline]
    fn partial_cmp(&self, other: &Self) -> Option<Ordering> {
        Some(self.id().cmp(&other.id))
    }
}
```

Would it make sense to have equivalent implementation of `PartialEq` instead of deriving it?
Other `Identifiable` structures should be considered as well
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-21 19:32:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1974" class=".btn">1974</a>
            </td>
            <td>
                <b>
                    Replace `blocks()` with `visit_blocks()` in WSV
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                Right now `WorldStateView::blocks()` has locking behaviour if user stores somewhere an iterator from this function. This can be fixed by replacing it with `visit_blocks()` function, which looks something like this:

```rust
/// Visit and apply `f` for every block
///
/// # Errors
/// Throws up first `f` error
pub fn visit_blocks<F>(&self, f: F) -> Result<(), Error>
where
    F: Fn(&VersionedCommittedBlock) -> Result<(), Error>,
```

In this way user can't store reference to a block, cause it is passed as a function parameter and **Rust** won't allow to save references like that
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-16 10:09:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1934" class=".btn">1934</a>
            </td>
            <td>
                <b>
                    Handle every `torii::Error` into appropriate response
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">UI</span>
            </td>
            <td>
                An unhandled custom rejection returns 500 ISE.
https://docs.rs/warp/latest/warp/reject/fn.custom.html
So every `torii::Error` case should be converted into explicit response in `iroha_core::torii::routing::handle_rejection`.
Remark that `torii::Error` has already `impl Reply`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 07:08:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1926" class=".btn">1926</a>
            </td>
            <td>
                <b>
                    Add explicit signal handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-20 15:49:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1914" class=".btn">1914</a>
            </td>
            <td>
                <b>
                    Store rejection reasons for blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">UI</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 11:24:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1913" class=".btn">1913</a>
            </td>
            <td>
                <b>
                    Refactor `DEADLOCK_ACTOR` to use `once_cell` in `iroha/actor/src/deadlock.rs`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-17 11:17:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1896" class=".btn">1896</a>
            </td>
            <td>
                <b>
                    Investigate what happens when events sender is not configured
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                This [piece of code](https://github.com/hyperledger/iroha/blob/iroha2-dev/core/src/wsv.rs#L223) in `core/src/wsv.rs` should be investigated:
```rs
    fn produce_events(&self, events: impl IntoIterator<Item = DataEvent>) {
        let events = events.into_iter().map(Event::from);
        let events_sender = if let Some(sender) = &self.events_sender {
            sender
        } else {
            return warn!("wsv does not equip an events sender");
        };
        for event in events {
            drop(events_sender.send(event))
        }
    }
```

I can't say why this compiles, maybe it `panics` inside the macro. Probably an error should be returned or events just dropped 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-09 20:47:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1885" class=".btn">1885</a>
            </td>
            <td>
                <b>
                    Add complete IPFS path validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Complete validation requires checking if path is composed only from valid hashes

[ipfs](https://docs.rs/ipfs/latest/ipfs/) crate source code can be helpfull

##  Alternative implementations

https://github.com/hyperledger/iroha/issues/1606
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 18:24:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1883" class=".btn">1883</a>
            </td>
            <td>
                <b>
                    Remove sample configs from the Docker container
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">api-changes</span>
            </td>
            <td>
                > Aleksandr Petrosyan, [2022/02/08 15:19]
> Another point that Bogdan raised is that we should stop including default configuration files inside containers. People boot up the container, see no error messages, assume everything is fine, when it isn't.
> 
> S Sato, [2022/02/08 16:30]
> [In reply to Aleksandr Petrosyan]
> The following would be one of the solutions:
> - Convert config.json to sample.env
> - Specify env_file: peer0.env .. for each peer in docker-compose.yml
> - Direct users to edit and rename sample.env and use docker compose
> https://docs.docker.com/compose/environment-variables/
> 
> S Sato, [2022/02/08 16:42]
> [In reply to S Sato]
> Not so much difference from directly writing environment section as current though
> 
> Aleksandr Petrosyan, [2022/02/08 16:42]
> [In reply to S Sato]
> This is a simplification, however.
> 
> Aleksandr Petrosyan, [2022/02/08 16:43]
> If we can reduce the number of places where Iroha can be configured to just one, I don’t see an issue.
> 
> S Sato, [2022/02/08 16:57]
> [In reply to Aleksandr Petrosyan]
> Yes, at least we can merge peer/config.json into environment variables,
> but instead, iroha_config will have to have dotenv
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-08 08:30:16 +0000 UTC
    </div>
</div>

