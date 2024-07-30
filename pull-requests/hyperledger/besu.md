---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7378" class=".btn">#7378</a>
            </td>
            <td>
                <b>
                    Add integration tests on block processing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
This PR aims to enhance block processing testing, inspired by [this comment](https://github.com/hyperledger/besu/pull/7296#discussion_r1683570569) from @garyschulte regarding test coverage. The goal is to develop unit tests that focus on executing block transactions without concerning header and body validations. For each scenario specified by @matkt, we test both sequential and parallel processing to ensure state changes remain consistent.

The tested cases are:

- Test 1
  - Trx1: Transfer from a to b
  - Trx2: Transfer from a to c

- Test 2
  - Trx1: Transfer from a to b
  - Trx2: Transfer from b to c

- Test 3
  - Trx1: Transfer from a to b
  - Trx2: Transfer from c to d

- Test 4
  - Trx1: Transfer from a to b
  - Trx2: Transfer from c to coinbase

- Test 5
  - Trx1: Contract with read from account A
  - Trx2: Contract with update to account A

- Test 6
  - Trx1: Contract with update to account A
  - Trx2: Contract with read from account A
  
- Test 7
  - Trx1: Contract with update to account A
  - Trx2: Contract with read from account B

- Test 8 (Slots)
  - Trx1: Contract with read from slot S1
  - Trx2: Contract with update to slot S1
  
- Test 9 (Slots)
  - Trx1: Contract with update to slot S1
  - Trx2: Contract with read from slot S1
  
- Test 10 (Slots)
  - Trx1: Contract with update to slot S1
  - Trx2: Contract with read from slot S2

The Solidity contract file has been added for reference. It represents the smart contract that the bytecode is included in the genesis file. Including this file in the PR helps in understanding the tests.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 14:07:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7377" class=".btn">#7377</a>
            </td>
            <td>
                <b>
                    Update GeneralStateTestCaseEipSpec for use in linea-arithmetization
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
In linea arithmetization we are updating unit tests to use the GeneralStateTestCaseEipSpec for testing. For that I need to 

1. Update the constructor to public so that it can be instantiated in other packages.
2. Include multiple transactions as we have unit tests that test multiple transactions.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-25 08:27:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/7374" class=".btn">#7374</a>
            </td>
            <td>
                <b>
                    Add EXTCODE* unit Tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description

Add unit tests to the EXTCODE* series operations.
Also, put all operations tests in the proper package.

## Fixed Issue(s)
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [ ] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [ ] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [ ] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [ ] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [ ] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-24 13:19:34 +0000 UTC
    </div>
</div>

