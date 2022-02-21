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
                Issue <a href="https://github.com/hyperledger/iroha/issues/1673" class=".btn">1673</a>
            </td>
            <td>
                <b>
                    Make use of `AsRef`, `AsMut` and `From` for versioned containers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Refactor</span>
            </td>
            <td>
                Our versioned containers implement `into_v1`, `as_v1`, `as_mut_v1` separately. To make this look more rusty I propose:

* find all instances of `into_v1` in the code and replace them with implementation of `From` trait
* find all instances of `as_v1` in the code and replace them with implementation of `AsRef` trait
* find all instances of `as_mut_v1` in the code and replace them with implementation of `AsMut` trait
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 18:43:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1640" class=".btn">1640</a>
            </td>
            <td>
                <b>
                    Generate `config.json` instead of storing it. 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span><span class="chip">Optimization</span>
            </td>
            <td>
                All configuration is done by hand. 

It may be a good idea to generate the `config.json`, `genesis.json` and `trusted_peers.json` programmatically and add explanation to `README.md`. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-26 07:54:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1638" class=".btn">1638</a>
            </td>
            <td>
                <b>
                    Have `configuration` endpoint GET return a subtree of docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                
```
Aleksandr Petrosyan, [25.11.21 13:31]
The docs on the configure endpoint are working. But they're not too intuitive.

Aleksandr Petrosyan, [25.11.21 13:31]
" Logger configuration.\n\nHas type LoggerConfiguration. Can be configured via environment variable IROHA_LOGGER"

Egor Ivkov, [25.11.21 13:32]
[In reply to Aleksandr Petrosyan]
Full path to the type can help

Aleksandr Petrosyan, [25.11.21 13:33]
Which should be returned by the top level field. If I'm querying the configuration docs, I don't know what subtypes are available,

Aleksandr Petrosyan, [25.11.21 13:34]
I think it should return the whole subtree of configurations, and not just the one that it matches

Egor Ivkov, [25.11.21 13:35]
Yes, I think it's a good idea
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-25 09:39:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/iroha/issues/1623" class=".btn">1623</a>
            </td>
            <td>
                <b>
                    Create a `RawGenesisBlockBuilder`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">good first issue</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Motivation

For testing it's better to set up assets/accounts/domains in the genesis block. We currently don't have a convenient interface to do that. 

## example

```rust
RawGenesisBlockBuilder::new()
    .with(Domain("wonderland"))
    .with(Account("alice@wonderland"))
    .with(Asset::BigQuantity("roses")
            .initially(100)
            .owned_by("alice@wonderland"))
    .finish()  
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-19 17:05:24 +0000 UTC
    </div>
</div>

