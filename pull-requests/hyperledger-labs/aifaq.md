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
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/3" class=".btn">#3</a>
            </td>
            <td>
                <b>
                    Change repo cloning, file splitting and general refine, second attempt
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hello @gcapuzzi,
this is a second attempt after PR https://github.com/hyperledger-labs/aifaq/pull/2

I changed how the repo is cloned: no more github api and **no more need to use a github PAT** but just a simple git clone running a bash command in a subprocess.

The **files are filtered by a list of allowed extensions** called ext_whitelist, this way you can grab md, mdx, and other files all together.

The files that pass the filter are splitted using a **specific splitter for markdown files that creates metadata** about the titles in the file itself, this is good for the quality and i think the speed of the research in the vector db. But the problem is that it works only with markdown, so, if your ext_whitelist has .js files, those should actually use a different splitter. The splitter selection should be based on the extension and more splitters should be used dynamically.

I took a stab at using [Langchain LCEL](https://python.langchain.com/docs/expression_language/) but I couldn't implement memory the way that I wanted so it is commented.

The rest is just a refine but nothing important.

p.s. _keeping the code in a notebook is pretty inconvenient because in this PR you cannot really see what I have changed unless you go to my project and try that, the history of the changes in the file is non-existent too._
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 20:52:33 +0000 UTC
    </div>
</div>

