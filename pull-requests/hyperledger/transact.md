---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/219" class=".btn">#219</a>
            </td>
            <td>
                <b>
                    Backport 0.3: Allow migrations to be run against a single connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Backport of #218 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 18:51:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/218" class=".btn">#218</a>
            </td>
            <td>
                <b>
                    Allow migrations to be run against a single connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change allows the user to run the migrations directly against a reference to a diesel connection.  It accomplishes this by re-exporting the database-specific migration functions directly from the migration module.

This allows migrations to be run in instances where the caller does not have access to a pool or the connection string, and therefore cannot use a `Backend` instance via the `MigrationManager`.
 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-13 16:29:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/217" class=".btn">#217</a>
            </td>
            <td>
                <b>
                    Remove Clone constraint from Write, Prune
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change removes the `Clone` constraint from the `Write` and `Prune` traits.  This constraint makes it so that these traits cannot be boxed as the traits are not object-safe.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-12 20:56:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/216" class=".btn">#216</a>
            </td>
            <td>
                <b>
                    Release notes for 0.3.11
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
        Created At 2021-10-12 15:01:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/215" class=".btn">#215</a>
            </td>
            <td>
                <b>
                    Backport 0-3: stabilize "state-merkle-sql"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change back-ports the following PRs:

* #189
* #191
* #192  
* #193 
* #209 
* #214
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 17:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/214" class=".btn">#214</a>
            </td>
            <td>
                <b>
                    stabilize "state-merkle-sql"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR also stabilizes "sqlite" and "postgres" features. 

It also includes a new test run to cover the postgres tests with the stable feature group enabled. This run is executed only in CI.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-11 15:50:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/213" class=".btn">#213</a>
            </td>
            <td>
                <b>
                    Update various dependencies
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
        Created At 2021-10-08 21:43:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/212" class=".btn">#212</a>
            </td>
            <td>
                <b>
                    Fix `time_to_wait` comments
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix out of date comments related to the `time_to_wait` arg.

Signed-off-by: Isabel Tomb <tomb@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-10-08 16:36:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/211" class=".btn">#211</a>
            </td>
            <td>
                <b>
                    Merge insert nodes and update changelog operations
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
        Created At 2021-10-08 14:38:12 +0000 UTC
    </div>
</div>

