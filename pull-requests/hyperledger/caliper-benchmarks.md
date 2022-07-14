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
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/220" class=".btn">#220</a>
            </td>
            <td>
                <b>
                    fixed paginatRichQuery and paginatedRangeQuery chaincode and benchmark
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The node chaincode uses default parameters while the go one doesn't

In the benchmark we do provide only the required parameters(2 out of 3 for rich query and 3 out of 4 for range query), which works for the node chaincode that has the last parameter as an optional default one while it does not work for the go one.

However, if you try to actually set the third parameter (forth for range query) the go one works fine but the node one doesn't
as far as I understood chaincode functions have a fixed signature with no optional parameters. This is an arbitrary choice since GRPC supports optional parameters by setting them to a default value if missing.

I removed the optional parameter from the node chaincode and provide all of the arguments in the benchmark call.

By reducing the number of assets created everything works fine. however, if we keep the current setting, creating 8000 assets for each worker and size, then around a third of query timeout.
By looking at the couch db logs we see that they eventually finish but after more than 20 seconds.
I solved the issue so that the builds can now pass without errors by reducing the number of asset created. I will close this issue #189 , but open a more specific one on the issues with Couchdb. 

Closes #189

Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 15:44:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    add good starter benchmarks for using caliper with hyperledger fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: fraVlaca <ocsenarf@outlook.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 09:23:31 +0000 UTC
    </div>
</div>

