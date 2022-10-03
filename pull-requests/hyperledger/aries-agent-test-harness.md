---
layout: default
title: aries-agent-test-harness
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-agent-test-harness
---

# aries-agent-test-harness <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-agent-test-harness){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/571" class=".btn">#571</a>
            </td>
            <td>
                <b>
                    Add ability to run the test scope of a runset normally executed daily by GitHub Actions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

A command that given the name of a runset (e.g. the tests run each night by GitHub Actions), grabs from that "workflow" YAML file the combination of agents used and the test scope, and then runs those.  Makes it easy to try out a runset to see where it is failing on your local system.  

Optionally allows you to do a `build` or `rebuild` before running the tests, and allows for doing a "dry-run" to printout what would be run.

Run `./manage runset -h` to get full help information and the list of runsets available.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-02 21:53:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-agent-test-harness/pull/570" class=".btn">#570</a>
            </td>
            <td>
                <b>
                    Update aries-vcx backchannel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-29 15:36:17 +0000 UTC
    </div>
</div>

