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
                PR <a href="https://github.com/hyperledger/firefly-common/pull/130" class=".btn">#130</a>
            </td>
            <td>
                <b>
                    Do not log an error if a JSON field is missing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Previously, this code would log an error if an array was not present in the JSON object structure (on the background context). This causes FireFLy Core to log things like this when it starts up:

```
[2024-02-22T17:53:58.799Z] DEBUG Log level: debug pid=1
[2024-02-22T17:53:58.802Z]  INFO Hyperledger FireFly pid=1
[2024-02-22T17:53:58.802Z]  INFO © Copyright 2022 Kaleido, Inc. pid=1
[2024-02-22T17:53:58.803Z]  INFO Starting up pid=1
[2024-02-22T17:53:58.806Z] DEBUG Debug HTTP endpoint listening on localhost:6060 pid=1
[2024-02-22T17:53:58.835Z] ERROR Invalid object value '<nil>' for key 'identity'
[2024-02-22T17:53:58.844Z] ERROR Invalid object value '<nil>' for key 'auth'
```

Even though these fields are optional, the error logs make it look like something is wrong with the config which is confusing to people. I believe we can omit this log entirely in the case that the array is not present `nil`, as the `ok` value will indicate to the calling code whether the field was found or not.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 18:50:30 +0000 UTC
    </div>
</div>

