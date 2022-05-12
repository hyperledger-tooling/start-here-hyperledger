---
layout: default
title: iroha-java
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-java
---

# iroha-java <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-java){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-java/pull/220" class=".btn">#220</a>
            </td>
            <td>
                <b>
                    Fix/iroha 213
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Changes:
1. Register event trigger refactoring
2. Cherry-pick iroha-219 issue schema changes
3. Added in-memory changes to iroha_data_model types that contains "data::filters" before generating code. For example this:
iroha_data_model::events::data::filters::FilterOpt<iroha_data_model::events::data::filters::IdFilter<iroha_data_model::account::Id>>
Becomes:
iroha_data_model::events::data::filters::FilterOptIdFilterAccountId
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-11 12:10:55 +0000 UTC
    </div>
</div>

