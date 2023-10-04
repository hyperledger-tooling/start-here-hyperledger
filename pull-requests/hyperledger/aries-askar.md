---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/189" class=".btn">#189</a>
            </td>
            <td>
                <b>
                    Adjust lower maximum number of connections for sqlite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Based on testing against ACA-Py. I believe that the `available_parallelism` method comes up with a lower number than `num_cpus::count` did on Github CI, but in general a maximum of 2 connections does seem too low.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-28 17:23:28 +0000 UTC
    </div>
</div>

