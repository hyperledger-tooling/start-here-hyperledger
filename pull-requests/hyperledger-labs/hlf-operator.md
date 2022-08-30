---
layout: default
title: hlf-operator
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hlf-operator
---

# hlf-operator <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hlf-operator){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hlf-operator/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    Fix default channel config name
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Creating a server to expose REST API I got this error:
```shell
Error: Failed to create Channel. channel name should match Regex /^[a-z][a-z0-9.-]*$/, but got _default
```
It seems that the underscore in `_default` is an unsupported symbol, so I solved renaming the default channel in `default` in all the project.
Hope this can help.

P.S.: I think is a good idea to add a "How to contribute" section to explain how to install a custom plugin/operator version to test changes and contribute to the project. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-30 14:25:59 +0000 UTC
    </div>
</div>

