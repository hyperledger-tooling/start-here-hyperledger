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
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/332" class=".btn">#332</a>
            </td>
            <td>
                <b>
                    Working with the cryptographic keys
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds previous work on the topic of cryptographic keys.
I've been looking into KeePass `gpg-agent` integration and am still seeking a solution.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-27 07:56:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/328" class=".btn">#328</a>
            </td>
            <td>
                <b>
                    [refactor]: migrate from `windicss` to `unocss`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                This is a housekeeping PR. WindiCSS is not going to be actively maintained, so I migrate the project to UnoCSS instead. More info: [Windi CSS is Sunsetting | Windi CSS](https://windicss.org/posts/sunsetting.html)

These libraries are used for CSS customisations - they provide a ton of class-utilities for a large variety of purposes. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 06:53:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/327" class=".btn">#327</a>
            </td>
            <td>
                <b>
                    [feature] #326: use local search
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #326 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 06:36:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/325" class=".btn">#325</a>
            </td>
            <td>
                <b>
                    [feature] #307: support Mermaid diagrams
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Render diagrams with [Mermaid | Diagramming and charting tool](https://mermaid.js.org/). Re-write existing diagrams with Mermaid syntax.

### Features

- Specify Mermaid blocks with <code>\`\`\`mermaid</code> (use `mmd` if you want just a code snippet with mermaid syntax highlighting)
- Renders diagrams on **front-end**, dynamically. Back-end rendering increases compilation time and **resulting bundle size** a lot.
- Reports error if the diagram is invalid

### Downsides

- I was not rewriting each diagram **VERY** carefully, so there might be semantic mistakes because of the syntax difference between Mermaid and PUML. Please review carefully.
- There is no compile-time check whether a diagram is valid (e.g. will render without an error) or not

### Related issues

Closes #307
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-26 02:09:04 +0000 UTC
    </div>
</div>

