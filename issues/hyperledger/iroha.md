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
                <span class="chip">help wanted</span><span class="chip">iroha2</span>
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
                Issue <a href="https://github.com/hyperledger/iroha/issues/1975" class=".btn">1975</a>
            </td>
            <td>
                <b>
                    Make automatic doc generator note optional features inside the documentation. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                When generated with `iroha_docs`, `config.md` can contain information about optional features. We want to make the addition of those features optional too, so that distribution packagers can remove the flags that they don't need, but by default if you just cloned the repository, you should be shown all of the optional features, explained how to use them and all of that be included in the docs. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-17 06:28:04 +0000 UTC
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
                Issue <a href="https://github.com/hyperledger/iroha/issues/1966" class=".btn">1966</a>
            </td>
            <td>
                <b>
                    `FindAllParameters` query cannot be used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                Since `ValidQuery` is not implemented for `FindAllParameters` it's not possible to execute this query. Either this query should be removed entirely or it should be enlisted in the `QueryBox` enum
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-10 16:45:47 +0000 UTC
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

