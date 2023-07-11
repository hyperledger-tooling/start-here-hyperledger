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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/1361" class=".btn">#1361</a>
            </td>
            <td>
                <b>
                    Do not set operation state to failed if we get a 409 - leave unchanged
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In PR chain with #1342 - where the build failed, and the logs showed we'd now successfully got a 409 after FFTM update in https://github.com/hyperledger/firefly-transaction-manager/pull/85, but then had gone on within the operation updater to set the operation to failed:

```
[36;1mfirefly_core_1_1  |[0m [2023-07-03T20:25:06.334Z]  INFO Executing token_transfer operation fc1bed3c-cf0a-49c6-93ca-53bc84b0816f via handler AssetManager httpreq=Lzru5k4n pid=1 req=UQydjKKy
[36;1mfirefly_core_1_1  |[0m [2023-07-03T20:25:06.334Z] DEBUG ==> POST http://tokens_1_0:3000/api/v1/transfer breq=l0uT1OYU pid=1 proto=fftokens
[36;1mfirefly_core_1_1  |[0m [2023-07-03T20:25:06.342Z] ERROR <== POST http://tokens_1_0:3000/api/v1/transfer [409] (7.97ms) breq=l0uT1OYU pid=1 proto=fftokens
[36;1mfirefly_core_1_1  |[0m [2023-07-03T20:25:06.342Z] DEBUG fftokens updating operation default:fc1bed3c-cf0a-49c6-93ca-53bc84b0816f status=Failed error=FF10457: Conflict from tokens service: Conflict: FF21065: ID 'default:fc1bed3c-cf0a-49c6-93ca-53bc84b0816f' is not unique ns=default pid=1
[36;1mfirefly_core_1_1  |[0m [2023-07-03T20:25:06.342Z] DEBUG Submitting operation update id=fc1bed3c-cf0a-49c6-93ca-53bc84b0816f status=Failed blockchainTX= worker=opu_003 ns=default pid=1
[36;1mfirefly_core_1_1  |[0m [2023-07-03T20:25:06.342Z]  INFO <-- POST /api/v1/namespaces/default/tokens/transfers [409] (14.28ms): FF10457: Conflict from tokens service: Conflict: FF21065: ID 'default:fc1bed3c-cf0a-49c6-93ca-53bc84b0816f' is not unique httpreq=Lzru5k4n pid=1 req=UQydjKKy
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-04 04:18:30 +0000 UTC
    </div>
</div>

