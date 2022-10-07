---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/628" class=".btn">#628</a>
            </td>
            <td>
                <b>
                    Operator view for methane app, drop RegisterIndustry from Net
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                *Frontend modifications*

- Drop RegisterIndustry component from NET My Roles page Only dealer role can register industry

- Operator view page for methane app Queries to methane-server 
 -- general operator details 
 -- wallet credentials assigned to operator
 -- assets owned by operator 
 -- products associated with operator by date range (work in progress) 
  - linked directly to operator (Aggregate) 
  - product totals linked to assets owned by operator 
 

- Static Product table renamed to ProductToken 
 -- ProductToken defined in NET portral app/frontend/react-app 
 -- Avoid naming conflict with static Product table used to organize raw oil and gas data (pre-token)

See the Oil and gas data description within the app/methane/README.md for details

*Data schema modificaitons*

- Uniquness constraint on AssetOperator 
 -- Postgres table considers null values as distinct 
 -- set unique index on AssetOperator table when thru_date is null 
 -- Prevents multiple active AssetOperators with the same operatorUuid during active operation (null thru_date).

- Introduce conjunction on QueryBundle type used to buildQueries 
 -- Optional conjunction attribute 
 -- Used to setup intersection queries (AND only) 
 -- DOES NOT support combination of multiple mixed conjunctions and disjunctions

Signed-off-by: brioux <Bertrand.rioux@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-07 18:19:24 +0000 UTC
    </div>
</div>

