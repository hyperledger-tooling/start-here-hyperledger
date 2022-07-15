---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/107" class=".btn">#107</a>
            </td>
            <td>
                <b>
                    Serious refactoring + improvements + adding new examples for Iroha 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">iroha1</span>
            </td>
            <td>
                I've made some refactoring similar to https://github.com/hyperledger/iroha-python/pull/103. Changes:
1. Added new examples:
    1. `tx-ordering.py` - example how to use not default ordering in returning from `GetAccountTransactions`
    2. `add-syncing-peer.py` - example how to add new syncing node
1. Refactoring of other examples:
    1. Added docstring for each example file
    2. Change old way of formatting strings into fstrings
    3. Better error handling - not only printing when something wrong but exceptions when error occurs + detecting GRPC connection error.
    4. Improved function wrapper
    5. Correcting functions - less hardcoding, functions more configurable
    6. `if __name__ == '__main__':`
    7. style more PEP8 compatible
    8. Renamed examples to make names more consistent
1. updated README file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 20:09:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/106" class=".btn">#106</a>
            </td>
            <td>
                <b>
                    [documentation] adds more details to the installation instruction
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                Please review and add more detailed installation instructions for the [`iroha2`](https://github.com/hyperledger/iroha-python/tree/iroha2) branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 10:57:45 +0000 UTC
    </div>
</div>

