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
                PR <a href="https://github.com/hyperledger/solang/pull/1448" class=".btn">#1448</a>
            </td>
            <td>
                <b>
                    Allow modification of AcconuntInfo lamports field
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
        Created At 2023-07-18 14:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1447" class=".btn">#1447</a>
            </td>
            <td>
                <b>
                    Bugfix: Accessing virtual function selectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The added test case panics in current `main` because accessing the selector of a virtual function which is not used in any other way will put the function in `all_functions` but not `virtual_functions`.  `check_inheritance` will insert the function into `all_functions` because we have this symbol, however because we only access the selector it's not a virtual function to the contract. The fix is that when we walk `all_functions` to find the externally callable ones, do not assume every function marked `virtual` is present in the `virtual_functions` of this contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 12:59:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1446" class=".btn">#1446</a>
            </td>
            <td>
                <b>
                    Add debug implementations required to print Namespace
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Derive `Debug` implementations for structs and enums required to print `struct Namespace`. This is of use when one needs to print `Namespace` struct for debugging purposes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 01:29:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1443" class=".btn">#1443</a>
            </td>
            <td>
                <b>
                    Make import_no Optional
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR does 2 things:
1. Makes `ResolvedFile::import_no` an `Option<usize>`
2. Improves test suite for import logic

This is a first attempt, I imagine there are a few things that can be improved.

Possible issues include:
1. Some `import_no`s are set to `0` when no import is used [per this conversation](https://github.com/hyperledger/solang/pull/1419#discussion_r1259358226); in this case, the `import_no` should be set to `None`. However, I imagine others are set to 0 because it is the first import that is performed. I currently just changed all literal `import_no: 0` to `import_no: Some(0)` to get it to type check, but I'm guessing they may actually want to be `import_no: None`.
2. @seanyoung you wanted more tests, and in particular for:
    1. when no import path is used, and
    2. "when a file is resolved via relative paths and not via import paths/maps". 
  Could you expand on these more? For (i), how would I set up a case when no import path is used? For (ii), do you mean in an import statement (like `import ./blah.sol`)? I have a test that does this (imports `integrations/polkadots/createpair.sol` which has a relative import), but I'm not sure exactly what we want to test.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 21:08:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1442" class=".btn">#1442</a>
            </td>
            <td>
                <b>
                    Update Release Checklist
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We must update the parser version on Anchor's repository.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 19:15:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1441" class=".btn">#1441</a>
            </td>
            <td>
                <b>
                    Fix compiler output section in solang.toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The compiler output section was not desterilized correctly from the `solang.toml` file created by `solang new`. this adds a fix for this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-14 02:34:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1440" class=".btn">#1440</a>
            </td>
            <td>
                <b>
                    Bump should be hashed by last
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, we hash include the bump in the `seeds` array passed to a Solana runtime call in the same order specified by developers when they are writing the contract's constructor. This is not the intended behavior, though. The bump must always be the last element in the array. This PR ensures that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 18:38:16 +0000 UTC
    </div>
</div>

