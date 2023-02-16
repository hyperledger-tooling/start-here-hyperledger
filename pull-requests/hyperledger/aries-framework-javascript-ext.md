---
layout: default
title: aries-framework-javascript-ext
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript-ext
---

# aries-framework-javascript-ext <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript-ext){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript-ext/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Optionally use the q/a context provider
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR expands on the work from Sabrina here : https://github.com/hyperledger/aries-framework-javascript-ext/pull/175 to leverage the AFJ dependency manager and check if the optional question and answer module is registered prior to using the context provider and react hooks. Have not yet tested it in an agent not importing the question-answer module, but I'm hoping that since the component isn't rendered it doesn't even try do the imports / cause an error
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-14 14:03:58 +0000 UTC
    </div>
</div>

