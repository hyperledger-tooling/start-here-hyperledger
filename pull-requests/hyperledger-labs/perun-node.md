---
layout: default
title: perun-node
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/perun-node
---

# perun-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/perun-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Impl contract registry & use it in node init
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->

- Contract registry is implemented to keep track of adjudicator and
  asset ETH and asset ERC20 contracts.

- This is initialized by the node and it is passed onto each of the
  sessions with a read-only access.

- In upcoming changes, APIs will be added in node to add new ERC20 asset
  contracts to the contract registry.

Also,

- Update SetupContracts test helper function to setup ERC20 assets and
  return a contract registry instead of contract addresses.

- Update the reference templates for node & session config.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Resolves #193.

#### Testing
<!-- Tell us how you have tested the changes. -->

Tests have been updated to cover the new functionality. 

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-22 07:00:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/210" class=".btn">#210</a>
            </td>
            <td>
                <b>
                    Add funcs to validate,deploy ERC20 asset contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->

- ROChainBackend and ChainBackend are updated to include the newly added
  functions.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Relates to #193.

#### Testing
<!-- Tell us how you have tested the changes. -->

Tests have been added (in `blockchain/ethereum/internal/chain_test.go`) to cover the newly added functionalities.

One error path is excluded, as it is unreachable under normal circumstances. Rest of the code is covered.

##### Steps run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 07:32:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/209" class=".btn">#209</a>
            </td>
            <td>
                <b>
                    Impl currency registry & store it in the node
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->
- Done in preperation to adding support for ERC20 tokens.

- Previously currency parsers for different currencies where stored in
  and fetched from a singleton instance of a map in the currency
  package.

- Using singleton instance works fine since only one type of currency
  was used, but does not work well when many symbols (one for each ERC20
  token) are to be registered when the node is running.

- Because, the node will register the currency in currency registry and
  the asset contract address in contract registry (to be done), it is
  better to store these two registries in the node.

- Hence, implemented a contract registry & added it as a field in the
  node. Also, added a test helper package with a registry that has all
  the required symbols pre-registered.

- Also, moved the constant values of the channel struct in session
  package to a new struct called params. It is easier to pass this field
  rather than passing "parts", "currency", "id" etc., individually.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task 

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Relates to #193.

#### Testing
<!-- Tell us how you have tested the changes. -->

Add tests for the newly added currency registry and updated existing tests.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 06:50:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/perun-node/pull/208" class=".btn">#208</a>
            </td>
            <td>
                <b>
                    Rename: consistently use assetETH instead of asset
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- Provide a general summary of your changes in the title above

Please read our contribution guidelines and sign the Contributor License
Agreement (CLA) before submitting the pull request. Also, check if there are no
other open pull requests targeting the same issue. -->

#### Description
<!-- Describe your changes in detail. -->


- Unitl now, since only ETH asset holder contract is used. Hence 'asset'
  is used to denote the ETH asset holder contract address.

- Now, rename is done in preparation for adding erc20 token support,
  where in addition to the ETH asset holder, one ERC20 asset holder
  contract will exist for each erc20 token.

##### Category
<!-- Tell us what type of issue does your pull request target.
You can uncomment one of the following options: -->

<!-- Bug Fix -->
<!-- Improvement -->
Implementation Task

##### Relevant issue
<!-- Provide a link to the related issue. You can use the following keywords
and the issue number: "fixes", "resolves", "relates to". E.g.: closes #21

We accept only pull requests related to open issues. If you're suggesting a new
feature, improvement or fixing a bug that is not yet reported, please discuss it in
an issue before submitting a pull request. -->

Relates to #193.

#### Testing
<!-- Tell us how you have tested the changes. -->

In this PR, only rename is done without modifying any functionality. All tests in CI pipeline should pass as before.

##### Steps to run the tests
<!-- Describe a set of steps to run the tests relevant to this change. -->

1. 
2. 
3.  

#### Checklist 
<!-- Please check if the pull request fulfils these requirements: -->

- [x] Name is added to the NOTICE file, if it is not present already.
- [x] Changes are rebased onto the target branch.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-21 06:47:06 +0000 UTC
    </div>
</div>

