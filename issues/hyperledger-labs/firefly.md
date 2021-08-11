---
layout: default
title: firefly
parent: Hyperledger Labs
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger-labs/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger-labs/firefly/issues/44" class=".btn">44</a>
            </td>
            <td>
                <b>
                    Tests fail if firefly.core file is present
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">good first issue</span>
            </td>
            <td>
                If the config file `~/.firefly/firefly.core` exists, then `make test` fails (presumably because the config in that file overrides the config in the tests).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-07 17:54:09 +0000 UTC
    </div>
</div>

