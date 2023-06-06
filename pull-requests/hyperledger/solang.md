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
                PR <a href="https://github.com/hyperledger/solang/pull/1356" class=".btn">#1356</a>
            </td>
            <td>
                <b>
                    Improve unused variable elimination
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following code causes an invalid memory access:

```solidity
function foo() public pure returns (bytes memory) {
    bytes b1 = hex"41";
    bytes b2 = hex"42";
 
   b2.push(0x41);
   return b1;
}

```

That happens because the unused variable elimination removes the declaration `bytes b2`, but maintains the `push`. This PR improves the elimination algorithms so much so that it removes the unnecessary pushes and pops if there is no actual read to the array in the function. It also takes care not to discard such operations when arrays are pointers to either storage or memory.

In addition, the error message for unused function parameter has been updated to `function parameter 'my_parameter' is unused`. When the parameter is a vector and has a push but no read, writing that it is `never read` is not the proper warning.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-05 21:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1355" class=".btn">#1355</a>
            </td>
            <td>
                <b>
                    Fix Anchor integration test
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
        Created At 2023-06-05 14:04:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1353" class=".btn">#1353</a>
            </td>
            <td>
                <b>
                    Do not pin `ink!` dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This was required for 4.1.0 because back then we were on rust 1.65 while 4.2.0 was on 1.68

Fixes #1351 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-04 08:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1352" class=".btn">#1352</a>
            </td>
            <td>
                <b>
                    fix(docs): Minor typo fixes for installation documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR aims to fix minor typos in the installation documentation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-03 10:07:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1350" class=".btn">#1350</a>
            </td>
            <td>
                <b>
                    Do not allow push and pop in fixed length arrays
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We presently allow pushed and pops from fixed length arrays, leading to a panic in emit. This PR disallows such operations.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 19:14:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1348" class=".btn">#1348</a>
            </td>
            <td>
                <b>
                    Substrate: Custom CI image
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
        Created At 2023-06-02 15:33:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1347" class=".btn">#1347</a>
            </td>
            <td>
                <b>
                    Read compiler configurations from toml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1- Implement taking solang's configurations from toml file. `solang compile --configuration-file`.
2- Implement solang new. a command that creates a new directory with a flipper example as well as the corresponding toml file. `solang new --target substrate`.  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-02 01:48:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1345" class=".btn">#1345</a>
            </td>
            <td>
                <b>
                    `@payer` annotation should declare an account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We aim to declare accounts for a function using only annotations. This PR is the first step towards this. The `@payer` annotation in the constructor now declares an account that is going to appear in the IDL. When a constructor is called from an external function, we automatically generate the `AccountMeta` array for the call so developers do not have to initialize such an array themselves. In addition, as we always need the account key in the transaction, `@payer` does not support addresses literals anymore.

This PR lays ground for the `@reader`, `@mutable` and `@mutableReader` annotations we wish to introduce later #1251 .

This PR already touches 45 files, so these changes are going to be in another PR:
1. When an annotation refers to a constructor argument, it should precede the argument declaration (just like Java). Right now, `@payer(account)` declares something while `@seed(arg1)` points to an argument. Such a syntax will lead to confusion.
2. We can't yet access the payer `AccountInfo` with the syntax `tx.accounts.payer`. This new command needs further changes in sema, codegen and emit.
3. The C function `external_call` will become useless as soon as I implement the account management for external calls, so it will be removed in the future.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-31 20:22:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1343" class=".btn">#1343</a>
            </td>
            <td>
                <b>
                    Substrate: Write assumed environment configuration into metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In `ink!`, certain types are configurable. The latest version of the metadata crate stores this information in the ABI file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 12:08:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1342" class=".btn">#1342</a>
            </td>
            <td>
                <b>
                    Fix build without llvm feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also ensure it is tested in CI.

Fixes https://github.com/hyperledger/solang/issues/1330.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 07:51:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1341" class=".btn">#1341</a>
            </td>
            <td>
                <b>
                    Improve the `contributing` section in our docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Lately, we had a bunch of people opening pull requests where the code did not even compile. But I also realized that the the `contributing` section in our docs could be better on that.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-30 07:29:12 +0000 UTC
    </div>
</div>

