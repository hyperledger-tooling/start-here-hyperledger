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
                PR <a href="https://github.com/hyperledger/solang/pull/1612" class=".btn">#1612</a>
            </td>
            <td>
                <b>
                    Fix abi.encodeCall() argument parsing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The arguments to the function should be passed as a tuple, if there are more than one. A single argument does not require a tuple.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-16 20:05:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1611" class=".btn">#1611</a>
            </td>
            <td>
                <b>
                    Various fallback improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Allow the following:

	contract A {
		// Take raw calldata as argument and return return data
		fallback(bytes calldata input) external payable (bytes memory) {}
	}

Allow a function to be called fallback:

	contract A {
		// Will give a warning that's not a fallback function,
		// just a regular functon
		function fallback() public {}
	}

This should make proxy contracts much easier to implement. 

Also fixes all fallback/receive related failures in the evm tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-16 08:23:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/solang/pull/1609" class=".btn">#1609</a>
            </td>
            <td>
                <b>
                    Represent type(f) correctly in the ast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes the ast correct, and also the following code is now parsed correctly:
    
            function foo() {
                    type(int);
            }

 `type(enum-type).min` or `type(enum).min` is now supported. 

This fixes all the issues wrt `type(T)`  in the solc tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-12 11:48:59 +0000 UTC
    </div>
</div>

