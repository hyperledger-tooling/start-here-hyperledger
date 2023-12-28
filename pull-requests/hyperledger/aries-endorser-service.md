---
layout: default
title: aries-endorser-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-endorser-service
---

# aries-endorser-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-endorser-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/42" class=".btn">#42</a>
            </td>
            <td>
                <b>
                    Rebased new migrations on the original migrations
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This resolves https://github.com/bcgov/DITP-DevOps/issues/138 by correcting the alembic migration error.

Before granular configuration was implemented the original migration file initial_db_tables_d925cb39480e.py was used.

Due to an over site this file was removed and a new complete_regeneration_bc503ce16d6d.py was produced.

While this would work for new deployments this broke backwards compatibility with existing deployments. For this reason we restored initial_db_tables_d925cb39480e.py and based updated_to_support_granular__e6afa1dce289.py on it to preserve this compatibility.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-27 20:41:20 +0000 UTC
    </div>
</div>

