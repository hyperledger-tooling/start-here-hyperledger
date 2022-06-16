---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1813" class=".btn">#1813</a>
            </td>
            <td>
                <b>
                    Refactoring of revocation registry creation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the revocation registry initialization process.

Previously, an event was fired using `profile.notify`, which led to an `IssuerRevRegRecord` being created and the associated revocation registry being generated. Now, the `IssuerRevRegRecord` is created first, and then the event is fired, which leads to the registry generation. This allows the detection of a registry in progress and helps to avoid multiple revocation registries being created in parallel for the same credential definition.

Also, the tails file is now uploaded after the registry definition is posted and before the first entry is posted, instead of after the first entry is posted. This ensures that the registry doesn't enter the ACTIVE state until after the tails file is publicly available.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 03:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1812" class=".btn">#1812</a>
            </td>
            <td>
                <b>
                    Fix external Outbound Transport loading code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                As the code currently stands, only internal outbound transports are able to be loaded. With these changes, it should be possible to load a new outbound transport via a plugin.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-16 02:13:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1811" class=".btn">#1811</a>
            </td>
            <td>
                <b>
                    Fix: present-proof v1 send-proposal flow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                - resolve #1809 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 17:41:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1808" class=".btn">#1808</a>
            </td>
            <td>
                <b>
                    Fix put_file when the server returns a redirect
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                I believe this fix only applies to tails file uploads at the moment. Previously, aiohttp would encounter an error because it closed the tails file after the first attempt.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-15 00:40:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1804" class=".btn">#1804</a>
            </td>
            <td>
                <b>
                    Adjust revocation registry update procedure to shorten transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-13 21:52:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1802" class=".btn">#1802</a>
            </td>
            <td>
                <b>
                    Fix: Inbound Transport is_external attribute
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: shaangill025 [gill.shaanjots@gmail.com](mailto:gill.shaanjots@gmail.com)

- resolve #1790 
- resolve #1791

Closed original PR #1792 due to merge issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 18:06:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1800" class=".btn">#1800</a>
            </td>
            <td>
                <b>
                    Fix: Duplicated schema and cred_def - Askar and Postgres
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">0.7.4</span>
            </td>
            <td>
                Signed-off-by: shaangill025 <gill.shaanjots@gmail.com>

- resolve #1786 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-06-10 14:45:26 +0000 UTC
    </div>
</div>

