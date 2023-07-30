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
                PR <a href="https://github.com/hyperledger/solang/pull/1468" class=".btn">#1468</a>
            </td>
            <td>
                <b>
                    Decouple data account from contract in the Solana mock VM
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As we start representing contracts by their program id (#1430), we bump into an incompatibility in our VM. The program id and the contract's data account are tightly coupled!

In order for us to decouple them from Solang as whole, we need to refactor the VM so that it accepts contracts without a data account.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-28 20:52:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1467" class=".btn">#1467</a>
            </td>
            <td>
                <b>
                    Revert "Ensure build works with latest contract-build and contract-metadata (#1466)"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The contract-build crate 3.1 was yanked: https://crates.io/crates/contract-build/versions

This reverts commit 665e550c0d5591c0453ddd2f06d455f9fe078d4a.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 13:18:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1466" class=".btn">#1466</a>
            </td>
            <td>
                <b>
                    Ensure build works with latest contract-build and contract-metadata
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The build is failing with errors about missing argument. The argument is for a container image name which we don't support.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 09:47:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1465" class=".btn">#1465</a>
            </td>
            <td>
                <b>
                    Relative imports are only done with relative paths and expose import_no
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When importing in Solidity, `import "foo";` does not check path relative to the currrent file, only `import "./foo";` does.

This work is also a re-write of https://github.com/hyperledger/solang/pull/1443
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-27 08:46:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1464" class=".btn">#1464</a>
            </td>
            <td>
                <b>
                    Remove duplicate dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If a dependency appears under `[dependencies]`, it does not need to be under `[dev-dependencies]`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 18:02:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1462" class=".btn">#1462</a>
            </td>
            <td>
                <b>
                    a.b.selector adds b() as function to current contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Compile the Solidity below and we end up with the non-base function in our contract.

```bash
$ solang compile --target polkadot --emit cfg
# function C::A::function::a public:true selector:0dbe671f nonpayable:true
# params: 
# returns: 
block0: # entry
	return 
```

```solidity
contract C {
    function ext_func_call(uint128 amount) public payable {
        A a = new A();
        (bool ok, bytes b) = address(a).call(
            bytes4(A.a.selector)
        );
	b = abi.encodeCall(A.a);
    }
}

contract A {
    function a() public pure {}
}
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-26 10:23:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1460" class=".btn">#1460</a>
            </td>
            <td>
                <b>
                    Constructors on Polkadot can be non-payable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We use the `seal1` `instantiate` runtime API, and with this runtime host function there is no need to send the minimum balance on instantiation (the comment in the docs is not correct).

Hence, constructors on Polkadot can and should actually be non-payble
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-25 19:47:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1459" class=".btn">#1459</a>
            </td>
            <td>
                <b>
                    Do not overwrite accounts' signer and writer flags
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When we traverse a functions to collect accounts, we may add the same account multiple times. IndexMap overwrites the entry in the table, whenever we add the same key again. We should not overwrite the writer and signer flags, however.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 21:30:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1458" class=".btn">#1458</a>
            </td>
            <td>
                <b>
                    Polkadot does not yet support catching Panics or custom errors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This isn't implemented yet in codegen and it won't make it into the July release (planned for August).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 20:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1457" class=".btn">#1457</a>
            </td>
            <td>
                <b>
                    Bugfix: External functions read their variable if they are called
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
        Created At 2023-07-23 18:59:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1456" class=".btn">#1456</a>
            </td>
            <td>
                <b>
                    Remove unnecessary .into_iter() and raw string
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are clippies in the next rust version.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-23 13:48:20 +0000 UTC
    </div>
</div>

