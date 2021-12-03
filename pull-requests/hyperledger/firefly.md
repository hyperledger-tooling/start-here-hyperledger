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
                PR <a href="https://github.com/hyperledger/firefly/pull/350" class=".btn">#350</a>
            </td>
            <td>
                <b>
                    Replace UpsertOperation with InsertOperation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                No code path ever passes allowExisting=true, and we already have a separate
UpdateOperation method for updates. Therefore, rename this method to
InsertOperation and remove the unneeded branches.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-03 17:22:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/347" class=".btn">#347</a>
            </td>
            <td>
                <b>
                    Address coverage drop from #337
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Coverage for JSONInputMask was inadvertently lost.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 19:28:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/346" class=".btn">#346</a>
            </td>
            <td>
                <b>
                    Return an empty slice (rather than nil) for zero token accounts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #345
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-02 18:47:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/344" class=".btn">#344</a>
            </td>
            <td>
                <b>
                    Reduce overhead of gocritic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For consideration - this seems to reduce the overhead significantly.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 21:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/342" class=".btn">#342</a>
            </td>
            <td>
                <b>
                    Update dependencies for v0.11.1 release
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
        Created At 2021-12-01 16:12:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/341" class=".btn">#341</a>
            </td>
            <td>
                <b>
                    Metrics endpoint to support charting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In order to support histograms, pie charts, and other charting in [Firefly-UI](https://github.com/hyperledger/firefly-ui), an endpoint is needed to fetch an array of row counts in a table, where each index (bucket) of the array is the count for the corresponding time interval between the start and end time.

time interval = `startTime - endTime` / `buckets`

GET `/api/v1/namespaces/default/metrics` with the following params:
`startTime`: unix time stamp to specify the start time of the data you want to fetch (ex. 1638279785)
`endTime`: unix time stamp to specify the end time of the data you want to fetch (ex. 1638366185)
`buckets`: number of buckets to divide the data into between the start and end time
`type`: the table name of the data you want to fetch data for

Typical response times for this endpoint are `50-100ms`. The `buckets` param is hard capped at 100 buckets to prevent expensive queries to the DB
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-12-01 13:52:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/340" class=".btn">#340</a>
            </td>
            <td>
                <b>
                    Fix Hyperledger Image Refs and Migration Job's Postgres URL in Helm Chart
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Noticed these when trying to deploy FireFly in live environments via the Helm chart

## Fixes

* `psql_url` needs to be a key in the `firefly-config` `Secret` when using the migration job
* uses for `ghcr.io/hyperledger/` for Docker repos
* no longer uses `latest` image tag, and instead uses `v0.9.2` for DX and `.Chart.AppVersion` for FF (which is set to `v0.11.1`)
* error message for when `organization.key` is not set is misleading since it reference the deprecated `organization.identity`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-30 04:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/339" class=".btn">#339</a>
            </td>
            <td>
                <b>
                    bump ui to version 0.4.2
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
        Created At 2021-11-29 14:15:30 +0000 UTC
    </div>
</div>

