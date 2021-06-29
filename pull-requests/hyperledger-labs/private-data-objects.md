---
layout: default
title: private-data-objects
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/private-data-objects
---

# private-data-objects <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/private-data-objects){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/private-data-objects/pull/324" class=".btn">#324</a>
            </td>
            <td>
                <b>
                    Take advantage of c++ standard library data structures
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                Finally ready to drop the Wawaka StringArray class and replace it with the c++ standard library datastructures std::string and std::vector.

Two items of note for this PR: 

First, the exchange contract family is completely removed. This is because the effort to move to std library will be significant. Exchange will be housed in a repository of its own. 

Second, the build target was changed from wasm to wasm-wasi to accommodate std::string which requires EOF 
from stdlib. There is some danger that developers will attempt to invoke other operations from stdlib without
wasi support... but that is not different from any other missing function.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-06-28 22:34:45 +0000 UTC
    </div>
</div>

