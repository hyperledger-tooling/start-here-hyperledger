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
                PR <a href="https://github.com/hyperledger/solang/pull/1377" class=".btn">#1377</a>
            </td>
            <td>
                <b>
                    Avoid repeated global strings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When debugging the issue #1367, I found out that we keep emitting repeated global strings. The LLVM IR for the contract pointed in such an issue had the string `math overflow,\0A` defined 1008 times.

This PR DOES NOT solve #1367, but it is something that needed a fix.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 21:13:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1376" class=".btn">#1376</a>
            </td>
            <td>
                <b>
                    Substrate: Implement call flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Substrate knows [flags](https://github.com/paritytech/substrate/blob/6e0059a416a5768e58765a49b33c21920c0b0eb9/frame/contracts/src/wasm/runtime.rs#LL392C27-L392C27) for contract calls. Until now we just always set them to 0. However we'll need them for more ergonomic `delegatecall` support and giving contract authors manual control over contract reentrancy. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-20 19:56:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1374" class=".btn">#1374</a>
            </td>
            <td>
                <b>
                    Implicit accessor function should return struct members, not struct
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the acessor function returns a single struct, then the members should be returned. If any of those members are structs, then those members will remain structs.

	contract C {
		struct S { int a; bool b; }

		S public s;

		function foo() public {
			(int a, bool b) = this.s();
		}
	}

Also, the accesor function should be declared `external` and therefore not accessible as an internal function call.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-19 15:43:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1370" class=".btn">#1370</a>
            </td>
            <td>
                <b>
                    Remove unnecessary code from lexer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The function `Lexer::next` has a `Result` as its returned type, but we never return `Err()`. This PR removes this unnecessary usage of `Result`.

I found this while creating a new token for `@annotation`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 19:31:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1369" class=".btn">#1369</a>
            </td>
            <td>
                <b>
                    Allow returns values to be ignored in try catch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                A try catch statement does not need to decode the return values if it is not interested.

```
interface I {
      function func()   externalpublic returns (int, bool);
}

contract C {
     function test(I i) public {
           try I.func() {
           }
           catch (bytes memory bs) { 
           }
     } 
}
```

Here `func()` returns two values but the try statement does not use them at all. This means they do not have abi decoded either.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 18:21:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1368" class=".btn">#1368</a>
            </td>
            <td>
                <b>
                    salt is of type bytes32
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                solang mistakenly uses `uint256` as the type for the salt argument. Change this to `bytes32` to be compatible with solc.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-16 15:35:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1366" class=".btn">#1366</a>
            </td>
            <td>
                <b>
                    Refactor constructor annotations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Presently, we can declare an account on a Solana constructor using the `@payer(my_account)` annotation, while `@seed(my_seed)` refers to a constructor parameter. Such a construction is confusing for the same syntax have two different meanings.

This PR limits the scope of annotation above a constructor to accept only literals as parameters (e.g. `@seed("pine_tree")`). Annotations that refer to function parameters must appear before them: `constructor (@seed bytes arg1)`. This is another in #1251.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-14 21:06:26 +0000 UTC
    </div>
</div>

