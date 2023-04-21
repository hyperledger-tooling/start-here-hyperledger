---
layout: default
title: solang
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1284" class=".btn">#1284</a>
            </td>
            <td>
                <b>
                    Fix new clippy 1.69 lint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Contains a drive by fix for the build. My guess is that the `ink` umbrella crate doesn't pin it's dependencies, which results in various `ink_* 4.2.0` dependencies being pulled in, despite explicitly pinning `ink = "=4.1.0"` in our `Cargo .toml`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-21 07:19:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1282" class=".btn">#1282</a>
            </td>
            <td>
                <b>
                    Fixed Duplicate code - 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solving #1262 
Part - 1
I have solved the first using closure and a function. Please give me feedback so that I can finish the other parts. 
Thankyou !
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 11:17:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1281" class=".btn">#1281</a>
            </td>
            <td>
                <b>
                    Do not panic if the value of a constant cannot be evaluated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a constant value makes no sense, then using that constant should not result in any error (previously this paniced).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 09:03:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1280" class=".btn">#1280</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Solang runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 00:01:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1279" class=".btn">#1279</a>
            </td>
            <td>
                <b>
                    Run Ethereum Solidity semantic tests through sema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There are many failures. First there are some tests which cause panics in sema. These are explicitly excluded. There are a further 1062 failures. Note the line:

	assert_eq!(errors, 1062);

To see the failures, see:

	cargo test --test evm ethereum_solidity_tests -- --nocapture
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-18 12:08:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1277" class=".btn">#1277</a>
            </td>
            <td>
                <b>
                    `memory_size_of()` needs guarded recursion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fixes the crash in ` ./solang-parser/testdata/solidity/test/libsolidity/syntaxTests/structs/recursion/return_recursive_structs2.sol`:

```
❯ cargo run -- compile --target substrate  ./solang-parser/testdata/solidity/test/libsolidity/syntaxTests/structs/recursion/return_recursive_structs2.sol

error: struct 'S' has infinite size
  ┌─ /home/cyrill/mess/solang/solang-parser/testdata/solidity/test/libsolidity/syntaxTests/structs/recursion/return_recursive_structs2.sol:4:12
  │
4 │     struct S { uint a; S[2][] sub; }
  │            ^           ---------- recursive field 'sub'

error: missing return statement
  ┌─ /home/cyrill/mess/solang/solang-parser/testdata/solidity/test/libsolidity/syntaxTests/structs/recursion/return_recursive_structs2.sol:6:6
  │
6 │     }
  │      ^
```

Ideally, instead of adding a dedicated test for this bug, we might want to run against all parser tests on CI too?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 11:45:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1276" class=".btn">#1276</a>
            </td>
            <td>
                <b>
                    Outside of modifiers _ is a regular identifier
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 10:05:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1275" class=".btn">#1275</a>
            </td>
            <td>
                <b>
                    Allow this.function.selector as bytesN and in pure mutability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Improve compatibility with solc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 09:23:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1274" class=".btn">#1274</a>
            </td>
            <td>
                <b>
                    [Fix] Removing the duplicate code.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix: #1261

Just wanna know If I am going in the right direction or not. Please guide me so I'll then fix other parts as I am trying to understand the codebase too.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-16 12:10:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1273" class=".btn">#1273</a>
            </td>
            <td>
                <b>
                    modifiers are allowed in libraries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solang did not permit this, but solc does.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-15 12:25:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1272" class=".btn">#1272</a>
            </td>
            <td>
                <b>
                    Encode addreses in base58 for print
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses on Solana and Substrate are often shown in base58 encoding, so we should print them like so.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 21:27:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1271" class=".btn">#1271</a>
            </td>
            <td>
                <b>
                    Enable the `accounts` call argument for constructors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When calling the constructor of a contract, we should be able to specify the account metas for the transaction. We need this feature, so we can automatically pass the accounts for the contract construction.

This PR is the second task in https://github.com/hyperledger/solang/issues/1251
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 19:08:50 +0000 UTC
    </div>
</div>

