---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/38" class=".btn">#38</a>
            </td>
            <td>
                <b>
                    misc: format sources, fix sidebar links, prettify queries guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Run auto-formatting on source files
- Fix links at sidebar config (missing leading slash)
- Transpose advanced guides in sidebar config. From WASM, Triggers, Queries to reversed order. I think it would be more like "in order of advancement" - queries are the most clear topic, wasm is the most complex.
- Hugely refactor queries guide. I am trying to make it more dense and more easy-to-read. As reference approach I am using this API guide: https://vuejs.org/api/reactivity-advanced.html
- Change some ordered-lists (1, 2, 3...) to unordered (dots), in triggers guide. Only in a single place it is necessary to have an order, because the following text references to it. In all other places order is unnecessary and brings a little mental overload.
- Some other _mostly subjective_ edits
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-29 09:24:30 +0000 UTC
    </div>
</div>

