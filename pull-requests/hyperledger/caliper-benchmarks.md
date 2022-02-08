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
                PR <a href="https://github.com/hyperledger/caliper-benchmarks/pull/164" class=".btn">#164</a>
            </td>
            <td>
                <b>
                    use test-network instead of custom networks for caliper-benchmarks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                closes #152
closes #154

Note that some chaincodes won't deploy to test network yet and this is
reflected in the README and a new CI pipeline will be required (it's not
working anyway as travis is no more)

The following bug issues cover addressing these

- #155
- #157
- #159
- #162
- #134

Signed-off-by: D <d_kelsey@uk.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-02 16:06:53 +0000 UTC
    </div>
</div>

