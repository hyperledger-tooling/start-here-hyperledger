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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1914" class=".btn">#1914</a>
            </td>
            <td>
                <b>
                    feat: include connection ids in keylist update webhook
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the connection IDs of the mediated connections. This should make it easier to trigger the next step in a flow (i.e. accept a connection request for one of the connections, if it's in the right state).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 14:55:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1913" class=".btn">#1913</a>
            </td>
            <td>
                <b>
                    Remove aca-py check for unrevealed revealed attrs on proof validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ian Costanzo <ian@anon-solutions.ca>

Addresses issue #1893
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-24 13:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1912" class=".btn">#1912</a>
            </td>
            <td>
                <b>
                    fix: incorrect response schema for discover features
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Small change that won't really affect anything but OpenAPI json and client generators.

The query features endpoint returns the discovery record directly rather than nesting it in a `results` attribute.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 19:13:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1911" class=".btn">#1911</a>
            </td>
            <td>
                <b>
                    [#1895] Stopping the aca-py shell process keeps python process running
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Thomas Diesler <tdiesler@redhat.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 17:51:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1910" class=".btn">#1910</a>
            </td>
            <td>
                <b>
                    Create sonarcloud.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 16:17:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1908" class=".btn">#1908</a>
            </td>
            <td>
                <b>
                    Add offers_attach to V10 credential schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We found out that the `offers_attach` attribute is not present in the credential offer schema. It is possible to send it to the api but its not present in the openapi spec. This is a problem is you generate yourself a client with the openapi spec because offers_attach is not defined.

This pr adds the attribute to the credential offer schemas.
It seems that there were also some other changes that are not reflected in the openapi.json. Therefore the changes in the openapi spec are bigger than the real changes in this pr.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-23 09:55:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1906" class=".btn">#1906</a>
            </td>
            <td>
                <b>
                    Send webhooks upon record/credential deletion
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is a ToDo note talking about sending webhooks when records are deleted. There are also no webhooks that get sent when a credential is deleted. This PR aims to fix the ToDo, as well as provide webhooks for when a credential has been deleted.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-22 15:23:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1904" class=".btn">#1904</a>
            </td>
            <td>
                <b>
                    Update for the v1.0.0-rc0 release. Changelog comment added for v0.7.4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update for the v1.0.0-rc0 release. Changelog comment added for v0.7.4
- Added this PR to changelog

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-18 19:41:58 +0000 UTC
    </div>
</div>

