---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/indy-sdk/issues/2395" class=".btn">2395</a>
            </td>
            <td>
                <b>
                    Remove blocking manual check for "indy-sys is available on crates.io"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span>
            </td>
            <td>
                The following blocking input is causing issues with build resources.  As the builds encounter this line they eventually block builds from happening on all Jenkins nodes consuming all resources and blocking any other builds from happening.

This line is the issue: 
https://github.com/hyperledger/indy-sdk/blob/master/Jenkinsfile.cd#L869
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-27 14:45:13 +0000 UTC
    </div>
</div>

