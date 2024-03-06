---
layout: default
title: aifaq
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/aifaq
---

# aifaq <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/aifaq){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/2" class=".btn">#2</a>
            </td>
            <td>
                <b>
                    Change repo cloning, file splitting and general refine
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi @gcapuzzi 
if you look at what's committed it may seem a lot but it is actually just a refine of your awesome work.

I transfered the code to a py file and now the colab version can be accessed by a badge on the README.md file, this will open Colab on a new minimal notebook that only clones the repo, installs the requirements and run the script.
This can be refined more adding parameters about the repo to clone and the file extensions of interest.

I changed how the repo is cloned: no more github api and no more need to use a github PAT but just a simple `git clone` running a bash command in a subprocess.

The files are filtered by a list of allowed extensions called ext_whitelist, this way you can grab md, mdx, and other files all together.

The files that pass the filter are splitted using a specific splitter for markdown files that uses metadata about the titles in the file itself, this is good for the quality and i think the speed of the research in the vector db. But the problem is that it works only with markdown, so, if your ext_whitelist has `.js` files, those should actually use a different splitter. The splitter selection should be based on the extension and more splitters should be used dynamically.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-05 20:14:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/1" class=".btn">#1</a>
            </td>
            <td>
                <b>
                    Poc new release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Release a new proof-of-concept version
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-03 09:16:22 +0000 UTC
    </div>
</div>

