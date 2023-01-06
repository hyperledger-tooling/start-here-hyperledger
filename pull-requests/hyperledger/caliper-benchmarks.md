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
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/236" class=".btn">#236</a>
            </td>
            <td>
                <b>
                    Remove old fabric performance reports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                2 reasons for this

Reason 1:
1.4 LTS Fabric version should not be being used any more 2.1.0 was never an LTS version and is not representive of Fabric 2.2 or the upcoming 2.5 nor the chaincode implementations used to test performance

Reason 2:
Caliper should not be hosting this. It's not Caliper's responsibity to provide performance reports for SUTs. SUTs themselves should do this and upto them whether they want to use Caliper or not as the load generator. If people want to know the performance of an SUT then this location is not exactly the obvious go to place.

Signed-off-by: Dave Kelsey <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 14:55:51 +0000 UTC
    </div>
</div>

