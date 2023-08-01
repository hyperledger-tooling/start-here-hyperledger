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
                PR <a href="https://github.com/hyperledger/solang/pull/1472" class=".btn">#1472</a>
            </td>
            <td>
                <b>
                    Minor fixes to the Solana library
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I fixed an incorrect comment and a wrong index when encoding data.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 17:27:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1471" class=".btn">#1471</a>
            </td>
            <td>
                <b>
                    Automatically apply suggestions of clippy pedantic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I've run `cargo clippy --fix --bin "solang" -- -W clippy::pedantic`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 16:46:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1470" class=".btn">#1470</a>
            </td>
            <td>
                <b>
                    General fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR has general fixes in Solang, namely:

1. Rename `must_fail` to `may_fail` as the usage of this function does not imply the function will fail.
2. Rename `edges` to `successors`, as the function returns the successors of a block.
3. Rename `clone_for_parent_block` to `deep_clone`.
4. Rename `set_maxi_signed` to `get_max_signed`
5. Rename `set_max_unsigned` to `set_max_unsigned`
6. Fix typos in comments and in function names.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 16:37:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1469" class=".btn">#1469</a>
            </td>
            <td>
                <b>
                    Add optimizations test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a test to do the following, with various Solidity programs and associated test vectors:
1. Compile the program with optimizations enabled.
1. Run the resulting binary on the test vectors.
1. Compile the same program with optimizations disabled.
1. Run the resulting binary on the same set of test vectors.
1. Verify that the two binaries’ outputs are equal.

Nits are welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-31 12:00:33 +0000 UTC
    </div>
</div>

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

