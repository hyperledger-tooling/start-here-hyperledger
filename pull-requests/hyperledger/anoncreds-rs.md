---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/32" class=".btn">#32</a>
            </td>
            <td>
                <b>
                    Remove the V1 suffix from the cred def
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dependent upon #23, #27, #30, #31

- Remove enum wrapper around the cred def
- Remove V1 suffix after the cred def
- Removes now useless get_attribute function in the FFI layer

I will leave the revocation stuff for now. @whalelephant Feel free to pick this up (removing the V1 suffix after the structures.)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 15:05:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/31" class=".btn">#31</a>
            </td>
            <td>
                <b>
                    Update schema data model
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dependent on #23, #27 and #30

- Removes the ver from the schema
- Rename attrNames to attr_names
- remove internal SchemaV1 enum wrapper
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 14:46:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    Remove seq no
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Dependent #25 and #27

Removes the seq_no internally (quite a small change)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-12 14:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Update to idiomatic rust
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Dependent on #25 
- Resolved some issues that clippy was giving. 
- renamed some functions to not make them collide with functions from std

Also fixed some small stuff from indy-utils, just to make clippy be quiet.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-10 15:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/25" class=".btn">#25</a>
            </td>
            <td>
                <b>
                    No id creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #4
closes #13 
closes #23 

It also picks up some tasks from other tickets. Mainly with regards to the "remove to_unqualified...".

Might have to do some clean up (most `String` can be converted to `&str`).

There are two major TODOs which I need some help with. 

Right now we have some presentation filter, like: schema issuer, schema name, etc. Before we could derive this from the schema id, but not anymore. How will we deal with this? As the schema id has no guarantee of being "qualified" we can not use it. 

I believe we can do these from the filters without changing anything:

```rust
    Ok(Filter {
        schema_id,         // YES
        schema_name,       // NO
        schema_issuer_did, // NO
        schema_version,    // NO
        cred_def_id,       // YES
        issuer_did,        // NO
    })
```
We can allow for more data to be passed in which can be gotten from an object resolution on the ledger or whatever.

The second one is the wrappers. I did not update them, but updating them would be trivial as they are just FFI-wrappers without complex logic build atop. I can create an issue for that if there is none. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 16:43:22 +0000 UTC
    </div>
</div>

