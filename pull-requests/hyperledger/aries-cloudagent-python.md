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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3103" class=".btn">#3103</a>
            </td>
            <td>
                <b>
                    Library update 15/07/24 / Fix unit test typing
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes some type checking syntax in unit tests. I'm not really sure why these didn't get flagged before or why the command line doesn't seem to pick up these specific errors. They are easy to fix though so I just changed them.

Upgrades ruff, pytest-ruff, portalocer and mkdocs-material
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-15 16:24:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3097" class=".btn">#3097</a>
            </td>
            <td>
                <b>
                    Update the docs for latest release and improve the publish flow and documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Addresses issue: #3096 

Cleans up a couple of documents, moves a "feature" document to be in the "deploying" section, updates the mkdocs.yml.

Also updates the PUBLISHING.md to remind publishers that the docs need to be checked on every release, and slight improvements in the script to test the mkdocs generation testing.  Also fixes a mistake in the script to convert MD to published site links.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-10 20:12:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/3095" class=".btn">#3095</a>
            </td>
            <td>
                <b>
                    Check connection is ready in all connection required handlers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is for https://github.com/hyperledger/aries-cloudagent-python/security/advisories/GHSA-cxwq-rwgr-qp5m.

I'm pretty sure this fixes the main issues reported with basic_messages and handshake_reuse protocols. I also applied the connection ready check to all other protocols that were missing and that I think need an established connection.

I didn't apply it to any problem report protocols because I don't think a connection is required in the cases. I'm not entirely sure if the problem report protocols could still be exploited in this way. Maybe an nefarious actor could send problem reports before the connection was established and cause issues?

The details of all these protocols isn't a strong point for me. I did my best to remediate the problem but I good review by someone more knowledgeable would be appreciated. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-10 17:58:35 +0000 UTC
    </div>
</div>

