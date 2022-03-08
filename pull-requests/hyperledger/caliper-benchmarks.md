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
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    fix java chaincode support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This gets java deploying and for the most part working, however there are problems in the way the java contract-api chaincode is implemented for fxed-asset which results in the benchmarks recording all failures for some of the benchmarks run, this will be addressed in #181 

Also note that go chaincode for fixed-asset has been addressed in another issue and so this enables running the chaincode and benchmark in the build

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 10:32:46 +0000 UTC
    </div>
</div>

