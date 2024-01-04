---
layout: default
title: did-webs-resolver
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/did-webs-resolver
---

# did-webs-resolver <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/did-webs-resolver){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/did-webs-resolver/pull/34" class=".btn">#34</a>
            </td>
            <td>
                <b>
                    Add __init__ modules to enable subpackages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I have installed did-webs-resolver as a git dependency. The `dkr` entry point is found, but when trying to run the console tool it raises:

```
from dkr.core import didding
ModuleNotFoundError: No module named 'dkr.core'
```

This is probably due to  `dkr.core` not including a `__init__.py. I have added those to both `core`  and `didcomm` subpackages.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-04 12:27:37 +0000 UTC
    </div>
</div>

