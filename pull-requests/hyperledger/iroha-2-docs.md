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
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/278" class=".btn">#278</a>
            </td>
            <td>
                <b>
                    Add java snippets
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-03 11:00:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/277" class=".btn">#277</a>
            </td>
            <td>
                <b>
                    [feature]: feedback form
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-02 02:56:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    [style]: use code-format for queries in Permissions guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 04:35:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/271" class=".btn">#271</a>
            </td>
            <td>
                <b>
                    [style]: format query names as code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 04:17:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/270" class=".btn">#270</a>
            </td>
            <td>
                <b>
                    [documentation]: fix small outdated info in JS guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 13:10:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/269" class=".btn">#269</a>
            </td>
            <td>
                <b>
                    [documentation]: use ANSI code snippet in Quick Start guide
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Close #266 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 12:51:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/268" class=".btn">#268</a>
            </td>
            <td>
                <b>
                    [docs] #267: Update sh-lang code blocks
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #267 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 10:04:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/265" class=".btn">#265</a>
            </td>
            <td>
                <b>
                    Update VitePress and other dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Notable VitePress changes:

- https://github.com/vuejs/vitepress/issues/1876. Now colored terminal output could be displayed nicely. I think it will be useful for [Quick Start guide](https://hyperledger.github.io/iroha-2-docs/guide/quick-start.html) where we have a terminal screenshot.
  - https://github.com/hyperledger/iroha-2-docs/issues/266
- Code groups - https://vitepress.vuejs.org/guide/markdown#code-groups. I removed our custom implementation.
- Interpolation inside code blocks, i.e. we can compute content and put it there using `{{ }}` syntax.
- https://github.com/vuejs/vitepress/pull/1339! Now we have a framework for translating documentation into different languages. 
- Multiple style fixes and improvements

Also, what do you think about moving some of section to the nav bar instead of having a single huge side bar?

Btw, VitePress has a feature for `sh` code blocks - you can add `$` to distinguish commands from their output. Might be useful sometimes. It doesn't affect "copy to clipboard" content. Issue:

- https://github.com/hyperledger/iroha-2-docs/issues/267
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 04:03:09 +0000 UTC
    </div>
</div>

