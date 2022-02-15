---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/716" class=".btn">#716</a>
            </td>
            <td>
                <b>
                    added single quotes on file patterns in prettify command for frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                On Mac, when I run
```sh
cd frontend/
npm install
```

I get errors like

```
[error] No files matching the pattern were found: "**/*.tsx".
[error] No files matching the pattern were found: "**/*.yml".
```

The quotations around the file patterns solve it.

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/716"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-14 11:58:37 +0000 UTC
    </div>
</div>

