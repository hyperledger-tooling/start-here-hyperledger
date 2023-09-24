---
layout: default
title: caliper-benchmarks
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper-benchmarks
---

# caliper-benchmarks <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper-benchmarks){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    Delete the old reports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These reports need to be removed for the following reasons
1. 1.4 is so old and is not a release that should be used
2. 2.0 and 2.1 releases were never LTS
3. one of the main goals for these reports were to compare contract-api to base shim for the contract-api developers which although interesting, performance isn't a factor for choice of api.
5. Caliper really shouldn't own these reports they should be owned by fabric. Fabric have PDF copies if really needed
6. There are no 2.2 or 2.5 reports where performance improvements around couchdb were introduced
7. There were some concerns around the numbers it shows so it's possible the reports were incorrect due to unknown influence
8. Fabric has a proper discussion around performance and a blog post of numbers where the environment was stable and resilient to external influences
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-24 09:23:01 +0000 UTC
    </div>
</div>

