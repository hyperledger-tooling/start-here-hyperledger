---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/solang/issues/707" class=".btn">707</a>
            </td>
            <td>
                <b>
                    compiler message for overloaded functions is not great
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                Given this solidity:
```
contract C {
	function foo(int a) public {}
	function foo(int a, int b) public {}
	function foo(int a, int b, int c) public {}
	function bar() public {
		foo(true);
	}
	function bar2() public {
		foo({a:true});
	}
}
```
The error message you get is:

```
/home/sean/git/solang/overloaded.sol:6:3-12: error: cannot find overloaded function which matches signature
Line 6:
	foo(true);
	^^^^^^^^^
/home/sean/git/solang/overloaded.sol:9:3-16: error: cannot find overloaded function which matches signature
Line 9:
	foo({a:true});
	^^^^^^^^^^^^^
```
That is not useful. The error message should list the overloaded functions which were tried, and the error message for each of them.

The same handling should be used for overloaded constructors when deploying a new contract.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-23 12:59:56 +0000 UTC
    </div>
</div>

