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
                <nil>
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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1340" class=".btn">#1340</a>
            </td>
            <td>
                <b>
                    Allow .wrap() and .unwrap() user defined type methods in constants
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is valid Solidity:

```
type Int is int8;

Int constant zero = Int.wrap(0);
```
Also, on solc `delete` on a local variable is a no-op. Make the error a warning.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 19:48:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1339" class=".btn">#1339</a>
            </td>
            <td>
                <b>
                    created calculate_mul_ovf to clean the repetitive code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #1263 

cleaned up the duplicate code by creating `calculate_mul_ovf` function
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 14:56:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1338" class=".btn">#1338</a>
            </td>
            <td>
                <b>
                    functions that use .call() should be allowed to declared view or default mutability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Functions that modify the state, like the SPL-token `mint_to`, are not `view` functions, but the compiler warns that they can be declared as view.

Example: 
```solidity
	function mint_to(address mint, address account, address authority, uint64 amount) internal {
		bytes instr = new bytes(9);

		instr[0] = uint8(TokenInstruction.MintTo);
		instr.writeUint64LE(amount, 1);

		AccountMeta[3] metas = [
			AccountMeta({pubkey: mint, is_writable: true, is_signer: false}),
			AccountMeta({pubkey: account, is_writable: true, is_signer: false}),
			AccountMeta({pubkey: authority, is_writable: true, is_signer: true})
		];

		tokenProgramId.call{accounts: metas}(instr);
	}
```

Warning:
```
warning: function can be declared 'view'
   ┌─ /solang/solana-library/spl_token.sol:46:2
   │
46 │     function mint_to(address mint, address account, address authority, uint64 amount) internal {
   │
```

Fixes https://github.com/hyperledger/solang/issues/997
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 14:00:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1337" class=".btn">#1337</a>
            </td>
            <td>
                <b>
                    @inheritdoc should work with bases of bases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We were only checking the immediate base contracts of the current contract, not their bases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 13:07:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1336" class=".btn">#1336</a>
            </td>
            <td>
                <b>
                    Destructure can assign to storage variables
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix building of the following:

        contract c {
            address factory;
            int decimals;

            constructor() {
                (factory, decimals) = foo();
            }

            function foo() internal pure returns (address, int) {
                return (address(2), 5);
            }
        }
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-29 09:45:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1332" class=".btn">#1332</a>
            </td>
            <td>
                <b>
                    Update substrate docker to use cargo contract 3.0
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
        Created At 2023-05-26 09:15:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1331" class=".btn">#1331</a>
            </td>
            <td>
                <b>
                    Update link to solang-llvm releases in `installing.rst`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change link to LLVM releases

#1330
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 07:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1329" class=".btn">#1329</a>
            </td>
            <td>
                <b>
                    Bump lalrpop and other dependencies
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
        Created At 2023-05-25 21:27:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1328" class=".btn">#1328</a>
            </td>
            <td>
                <b>
                    Make GetAddress return a pointer to an address
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In the same lines of #1325, loading addresses in codegen instead of emit allows us to leverage pointers to create `AccountMeta` arrays.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-25 20:41:36 +0000 UTC
    </div>
</div>

