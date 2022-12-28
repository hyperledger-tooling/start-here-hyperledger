---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    chore(release): v0.3.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">ci-test</span>
            </td>
            <td>
                Release version 0.3.1
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-27 23:34:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1185" class=".btn">#1185</a>
            </td>
            <td>
                <b>
                    chore(migrations): add generated test 0.2 connection records for migration tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR is a follow up to #1177 and includes generated test connection records from [this script](https://github.com/petridishdev/aries-framework-javascript-test-data-generator/blob/main/index.ts) along with migration tests and snapshots for AFJ update from 0.2 to 0.3.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-26 21:28:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1184" class=".btn">#1184</a>
            </td>
            <td>
                <b>
                    fix: missing migration script and exports
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Unfortunately, `migrateDidRecordToV0_3` was not added to `updateV0_2ToV0_3` script, meaning that DID records were not upgraded, making DIDs non-resolvable.

This PR fixes that and also exposes a few classes that are mentioned in [the documentation](https://aries.js.org/guides/updating/update-assistant) but were no exported directly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-26 17:57:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1182" class=".btn">#1182</a>
            </td>
            <td>
                <b>
                    feat: adding trust ping events and trust ping command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Kim Ebert <kim@indicio.tech>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-22 21:17:54 +0000 UTC
    </div>
</div>

