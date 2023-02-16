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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/45" class=".btn">#45</a>
            </td>
            <td>
                <b>
                    Support GetInteger from JSONObject when value in map is integer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While the normal JSON parsing in Go doesn't result in a `map[string]interface{}` that has any other number types in it than `float64`, the parsing of YAML in `viper` does.

So in the case you do a `config.GetObject()` call, and the YAML value in there is set as a number, you might get `0` back from a `GetNumber()` on it - even if the value is set.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-12 22:18:38 +0000 UTC
    </div>
</div>

