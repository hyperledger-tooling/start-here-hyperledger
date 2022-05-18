---
layout: default
title: grid-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid-docs
---

# grid-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/336" class=".btn">#336</a>
            </td>
            <td>
                <b>
                    Fix links to Sawtooth documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Sawtooth docs site recently underwent a reorganization. This PR fixes the existing links for the updated Sawtooth docs.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-18 17:24:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/335" class=".btn">#335</a>
            </td>
            <td>
                <b>
                    Update schemaspy java dependency version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Java version was updated in PR
https://github.com/schemaspy/schemaspy/pull/850

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-16 16:49:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid-docs/pull/334" class=".btn">#334</a>
            </td>
            <td>
                <b>
                    Add files to generate mermaid diagrams
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To add a diagram, add the following Jekyll front matter to the
top of the page:

---
tags: [Mermaid]
mermaid: true
---

Next, add the mermaid syntax wrapped in a <div class="mermaid">:

<div class="mermaid">
graph LR
    1 --- 2
    2-->A[foo]
    2-->B(bar)
</div>

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-12 17:36:52 +0000 UTC
    </div>
</div>

