---
layout: default
title: solang
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang
---

# solang <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/562" class=".btn">#562</a>
            </td>
            <td>
                <b>
                    Minor fixes
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
        Created At 2021-11-12 15:45:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/560" class=".btn">#560</a>
            </td>
            <td>
                <b>
                    Support disabling optimization (-O none) during code generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi,

I created this PR to support the feature `-O none` that disables code optimization during code generation.
This is discussed in the issue: https://github.com/hyperledger-labs/solang/issues/551

Here is an example of how it works:

- Input file: `count_input1.sol`:

  ```solidity
  pragma solidity ^0.4.19;

  contract CountInput {
      uint private count = 1;

      function run(uint256 input) public {
          count += input;
      }
  }
  ```

- Compile without `-O none`:

  ```sh
  $ solang count_input1.sol --emit cfg --target ewasm
  
  count_input1.sol:4:5-27: warning: storage variable 'count' has been assigned, but never read
  Line 4:
      uint private count = 1;
      ^^^^^^^^^^^^^^^^^^^^^^
  #
  # Contract: CountInput
  #


  # function CountInput::CountInput::function::run__uint256 public:true selector:a444f5e9 nonpayable:true
  # params: uint256
  # returns: 
  block0: # entry
      ty:uint256 %input = (arg #0)
      return 

  # function CountInput:storage_initializer public:false selector:00000000 nonpayable:false
  # params: 
  # returns: 
  block0: # entry
      store storage slot(uint256 0) ty:uint256 = uint256 1
      return 

  # constructor CountInput::CountInput::constructor::861731d5 public:true selector:861731d5 nonpayable:true
  # params: 
  # returns: 
  block0: # entry
      return 
  ```
  
- Compile with  `-O none`:

  ```sh
  $ solang count_input1.sol --emit cfg --target ewasm -O none
  
  count_input1.sol:4:5-27: warning: storage variable 'count' has been assigned, but never read
  Line 4:
      uint private count = 1;
      ^^^^^^^^^^^^^^^^^^^^^^
  #
  # Contract: CountInput
  #

  # function CountInput::CountInput::function::run__uint256 public:true selector:a444f5e9 nonpayable:true
  # params: uint256
  # returns: 
  block0: # entry
      ty:uint256 %input = (arg #0)
      %temp.2 = load storage slot(uint256 0) ty:uint256
      ty:uint256 storage %temp.1 = (%temp.2 + (arg #0))
      store storage slot(uint256 0) ty:uint256 = %temp.1
      return 

  # function CountInput:storage_initializer public:false selector:00000000 nonpayable:false
  # params: 
  # returns: 
  block0: # entry
      store storage slot(uint256 0) ty:uint256 = uint256 1
      return 

  # constructor CountInput::CountInput::constructor::861731d5 public:true selector:861731d5 nonpayable:true
  # params: 
  # returns: 
  block0: # entry
      return 

  ```
  
  In this run, the original code of `function::run__uint256` is generated: no optimization is enabled to remove the unused variable `count`.

Could you help to review this PR?

Thank you!

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-12 08:55:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Fix recursive structs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Iwan Waitusenok <sleepplease@protonmail.ch>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-11 12:56:31 +0000 UTC
    </div>
</div>

