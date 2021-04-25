---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/caliper
---

# caliper

You can clone this repo on <span class="fs-3">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div class="code-example" markdown="1">
    <table>
        <tr>
            <td>
                PR [#1135](https://api.github.com/repos/hyperledger/caliper/pulls/1135)
            </td>
            <td>
                <b>
                    Resolve issue in which only first round would be docker-monitored
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is an issue that docker containers are only monitored during the first round of a multi-round benchmark as described in issue #1134.
The problem is caused by the fact that the `stop()` command sets the `this.containers` property to the empty array `[]`, while it expects a `null` value to (re)set the containers list. By setting this to `if (!this.containers || this.containers.length == 0)`, we account for both cases.

Resolves #1134

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 09:30:31 +0000 UTC
    </div>
</div>

