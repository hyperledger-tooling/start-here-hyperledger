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
                Issue <a href="https://github.com/hyperledger-labs/solang/issues/755" class=".btn">755</a>
            </td>
            <td>
                <b>
                    Comparisons should support constants
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                When we declare a constant variable that has an initializer, e.g. `bool x constant = 0 < 2`, we evaluate the actual constant value in compiler time. Currently, there is no support to evaluate constants in comparisons, so the aforementioned example is evaluated in run time.

We need to calculate comparisons with constants during compilation. Ideally, this can be created in `src/sema` and the comparison can be evaluated in compile time.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 11:38:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/solang/issues/754" class=".btn">754</a>
            </td>
            <td>
                <b>
                    Overflow checking in constant arithmetic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                There should be overflow checking in arithmetic operations using constants.
E.g. `uint8 = 128 + 128` should raise an error.

Ideally, this check can be done in function `eval_const_number` in `src/sema`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 11:30:29 +0000 UTC
    </div>
</div>

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

