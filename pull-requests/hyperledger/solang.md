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
                PR <a href="https://github.com/hyperledger/solang/pull/1409" class=".btn">#1409</a>
            </td>
            <td>
                <b>
                    Fix undefined variable detection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The contract I added in the tests was working properly in Solang v0.3.0, but it caused a panic in [this line](https://github.com/hyperledger/solang/blob/a84b0ad3b67a17b524ef6b7437fd4c5376833807/src/codegen/strength_reduce/expression_values.rs#L79) on the main branch. 

I couldn't identify what has changed from the release till now, but I deemed the logic for reporting undefined variables and stop optimizations erroneous.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 21:11:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1408" class=".btn">#1408</a>
            </td>
            <td>
                <b>
                    Added get_contents_of_file_no
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a public way to get the file contents from a file number. I've defaulted to a verbose function name, but happy to change that if folks like (e.g., maybe just `get_contents(file_no: usize)`, but that's a little awkward because of `set_contents(path: &str, contents: String)`... I feel like `get_XXX` and `set_XXX` should have the same type for `XXX` (in this case `file_no`'s `usize` would conflict with `path`'s `&str`)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 16:53:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1407" class=".btn">#1407</a>
            </td>
            <td>
                <b>
                    Change `log_runtime_error` call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix for a problem resulting from merging #1400.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 14:25:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1405" class=".btn">#1405</a>
            </td>
            <td>
                <b>
                    Substrate: Distinct dispatch CFG for `call` and `deploy`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix an oversight form #1249. The dispatch logic can not be the same for `call` and `deploy` as constructors must _not_ be allowed to be accessed from the `call` function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-28 00:09:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1404" class=".btn">#1404</a>
            </td>
            <td>
                <b>
                    v0.3.1: Göttingen release (aka June release)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release tests are running [here](https://github.com/LucasSte/solang/actions/runs/5395030402).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 22:03:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1403" class=".btn">#1403</a>
            </td>
            <td>
                <b>
                    Move stdlib build output to `target` folder
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a fix for #1321.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 21:11:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1402" class=".btn">#1402</a>
            </td>
            <td>
                <b>
                    Ensure that a constructor cannot be run twice on the same data account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The constructor code path was not checking that the data account magic number is not populated.

The change also exposed another issue: when a pure function is called, there should be no load of data magic number, this may result in a access violation.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 09:22:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1401" class=".btn">#1401</a>
            </td>
            <td>
                <b>
                    Make rust analyzer work again
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This slipped in, nuke it to fix RA
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-27 08:04:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1400" class=".btn">#1400</a>
            </td>
            <td>
                <b>
                    Runtime error strings must be LLVM constant strings instead of dynamically allocated
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The contract linked at #1367 calls `vector_new` too many times, because the runtime error strings are dynamically allocated during execution. This PR makes the runtime error strings constant attributes in LLVM, so they are not allocated.

In addition, this PR has these changes:
1. The test case caused a stack overflow in constant folding, so I split `fn expression` into multiple small functions.
2. `log_runtime_error` contained repeated code for both targets and has been removed from the `trait TargetRuntime`.
3. `error_message_with_loc` now adds the new line character.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 21:26:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1397" class=".btn">#1397</a>
            </td>
            <td>
                <b>
                    Substrate: Implement builtin for `set_code_hash` API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Exposes a low-level builtin function for calling `seal_set_code_hash`. The code hash arguments is of type ~~`bytes`~~ `uint8[N]` intentionally (and not of type `Hash`, so that it matches the the pointer expected by the API function. `Hash`, which is just an alias to `bytes32`, will internally be represented as an `i256`. I came to the conclusion that, given this type conversion can easily be written in Solidity, we do and should not want to deal with that in the compiler, be it in emit or in codegen or elsewhere. 
Instead, a more high level function, that asks for a `Hash` argument and converts that to ~~`bytes`~~ `uint8[N]`, should rather be implement in the substrate Solidity library (once we have it).
Additionally, if some parachain decides to use a hash longer than 32bytes, using just a ~~`bytes`~~ `uint8[N]` pointer will still work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 15:19:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1396" class=".btn">#1396</a>
            </td>
            <td>
                <b>
                    Add markdown formatting to hover messages
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
        Created At 2023-06-26 09:45:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1395" class=".btn">#1395</a>
            </td>
            <td>
                <b>
                    Drop diagnostics on closing the file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When closing a file in VS code, all the warnings and errors remain in the list of problems. This removes all diagnostics pertaining to the close file. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:29:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1394" class=".btn">#1394</a>
            </td>
            <td>
                <b>
                    Pick up unsaved changes in a file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently the language server reads the file, rather than using the source code which is sent to it over language server requests. In order for the language server to update with the latest text of the source file, one needs to save the file. 
These changes enable the language server to update as one types. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:26:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1393" class=".btn">#1393</a>
            </td>
            <td>
                <b>
                    add option to set trace level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows the user to configure the verbosity of trace of messages exchanged between client and the server.
The user can set this in `User Settings` (press ctrl/cmd+,) and then searching for solidity related configuration. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 08:23:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1392" class=".btn">#1392</a>
            </td>
            <td>
                <b>
                    add contract author and version flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR implements a way to specify the author and version of all contracts via the CLI or via "solang.toml"
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-26 02:37:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1391" class=".btn">#1391</a>
            </td>
            <td>
                <b>
                    Optimize modifier CFGs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                Closes #1385 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-25 11:46:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1390" class=".btn">#1390</a>
            </td>
            <td>
                <b>
                    Substrate: Implement `delegatecall()`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Required by upgradable proxy patterns.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 17:29:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1389" class=".btn">#1389</a>
            </td>
            <td>
                <b>
                    Bump Solana, Anchor and Ubuntu
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Solana 1.16.1
Ubuntu 22.04 rather than 20.04
Anchor 0.28.0
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-24 13:20:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1384" class=".btn">#1384</a>
            </td>
            <td>
                <b>
                    Access payer account using `tx.accounts.account_name`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR creates the infrastructure for accessing accounts with `tx.accounts.account_name`. Presently, we can only access accounts declared with the `@payer` annotation, but our goal is to make this possible for all accounts declared with annotations (this is not implemented yet). 

The documentation I wrote is very terse, because my plan is to add more details when I have the `@reader`, `@mutable`, `@signer` and `@mutableSigner` implemented.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-23 14:50:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1383" class=".btn">#1383</a>
            </td>
            <td>
                <b>
                    Update roadmap on README
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
        Created At 2023-06-23 08:15:35 +0000 UTC
    </div>
</div>

