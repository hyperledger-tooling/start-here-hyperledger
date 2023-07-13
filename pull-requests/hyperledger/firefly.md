---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1369" class=".btn">#1369</a>
            </td>
            <td>
                <b>
                    Backport: FabConnect does not / can not set transactionIndex and eventIndex
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is a PR to backport https://github.com/hyperledger/firefly/pull/1345 into the 1.2 release branch. I did have to tweak the tests slightly because there are other somewhat related changes around event batching that were not pulled in.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-12 18:54:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1368" class=".btn">#1368</a>
            </td>
            <td>
                <b>
                    docs: Add webhook batching and update retry
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
        Created At 2023-07-12 13:12:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1366" class=".btn">#1366</a>
            </td>
            <td>
                <b>
                    docs: fix broken link to events reference document
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
        Created At 2023-07-10 20:45:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1365" class=".btn">#1365</a>
            </td>
            <td>
                <b>
                    v1.2: fix: multiple named tuple result from contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of https://github.com/hyperledger/firefly/pull/1333
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-10 14:11:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1364" class=".btn">#1364</a>
            </td>
            <td>
                <b>
                    Add unit test for LIKE filters with escaped characters
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Validates proper escaping of '%' and '_'.

Requires https://github.com/hyperledger/firefly-common/pull/87
Fixes #1084 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 16:25:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1363" class=".btn">#1363</a>
            </td>
            <td>
                <b>
                    Docs SEO Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @nguyer this pull request should address the items I've listed in issue #1362. It removes the output from the jekyll-seo-tag plugin and instead uses only the theme to add the page title and various meta tags. It includes custom page titles and meta descriptions for all of the docs pages so they'll be better crawled and displayed by search engines. And last, it hooks up Google Tag Manager so we'll be able to have Google Analytics for the site and see what kind of traffic it's getting. Let me know if you see anything you'd like me to adjust.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-06 13:54:50 +0000 UTC
    </div>
</div>

