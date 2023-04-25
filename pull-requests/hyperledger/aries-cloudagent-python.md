---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2216" class=".btn">#2216</a>
            </td>
            <td>
                <b>
                    Add updated ELK stack for demos/testing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The EFK stack was out of date and updating it was not as simple as changing version numbers. Decided to bring in a more robust, current and reliable stack to use for tracing demos. The main impetus for the ELK stack is for monitoring performance for the mediator service. 

Documentation has been updated to reflect the removal of the EFK.

Have also included examples for running the demos and the `multi-demo` with tracing events into ELK. Bumping the multi-demo postgres to 14.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-24 22:54:44 +0000 UTC
    </div>
</div>

