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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1270" class=".btn">#1270</a>
            </td>
            <td>
                <b>
                    Use rationals rather than float for calculating flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Flow calculation involves division followed by addition, e.g. 10/3 + 10/3 + 10/3 is not exactly 10 when using floats. So, use rationals instead.

I *think* `Rational<usize>` will suffice but I chicked out and used BigRational instead.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 10:21:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1269" class=".btn">#1269</a>
            </td>
            <td>
                <b>
                    Rename more unchecked to overflowing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Recently unchecked was renamed overflowing in CFG. A few renames were missed.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 15:04:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1268" class=".btn">#1268</a>
            </td>
            <td>
                <b>
                    Disallow dynamic arrays for account metas
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Account metas do not support dynamic arrays and we do not inform that to the user.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 21:57:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1267" class=".btn">#1267</a>
            </td>
            <td>
                <b>
                    Test large github runners
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
        Created At 2023-04-12 15:46:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1266" class=".btn">#1266</a>
            </td>
            <td>
                <b>
                    Remove redundancies in `is_next_reachable()`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                After merging #1260 , I noticed the checks in my code were redundant.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 15:35:41 +0000 UTC
    </div>
</div>

