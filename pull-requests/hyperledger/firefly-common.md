---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/16" class=".btn">#16</a>
            </td>
            <td>
                <b>
                    Add API framework and Swagger generator, plus enum support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This allows use of the FireFly API framework as `ffapi` in other microservices, adding to the `httpserver` which is already available.

There is an extension point in the `Route` object, to allow the Filter syntax that is needed by FF Core to be extended on top of this.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-02 17:48:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/15" class=".btn">#15</a>
            </td>
            <td>
                <b>
                    Remove FFCAPI for updated architecture
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                When events are involved, the coupling between the FFTM and the connector code is just too intertwined to support separate runtime processes. So a refactor of the FFCAPI needs to happen, and it makes sense for that to happen within a refactored FFTM.

So it should be removed from here.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-01 14:47:37 +0000 UTC
    </div>
</div>

