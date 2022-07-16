---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1458" class=".btn">#1458</a>
            </td>
            <td>
                <b>
                    Add REST API module to griddle
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Epic: Griddle</span><span class="chip">main</span>
            </td>
            <td>
                This adds a rest api with a builder, runnable, and running instances. This allows for the rest api to be stood up and taken down more easily. The running instance of the rest api implements the `ShutdownHandle` trait from the threading::lifecycle module.  

Technically, this also updates Griddle to use actix web 4. The rest api module is behind the experimental `rest-api` feature. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-15 19:32:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/1457" class=".btn">#1457</a>
            </td>
            <td>
                <b>
                    Jammy upgrade
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">backport-triage</span><span class="chip">main</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-11 20:25:10 +0000 UTC
    </div>
</div>

