---
layout: default
title: aries-askar
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-askar
---

# aries-askar <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-askar){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Add method to ping store sessions; verify profile existence when opening a session
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #163 

For Postgres, this also ensures that a profile cannot be removed while there is an active transaction against it.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-08 22:42:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Postgres provisioning fixes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                For support of Postgres 15 where the CREATE permission isn't automatically granted on the 'public' schema.

Adds a new optional 'schema' parameter for postgres connection URLs (ie. `postgres://user:pw@host/db?schema=public`). When not set, the schema now defaults to the username when creating new tables.

For new stores,
- If the database is newly created, then the database owner is set explicitly
- A new schema is created in the database, with the same name as the user. This is consistent with the default search path: `('$user', public)`
- All tables are created in the specified schema

For existing stores,
- If the schema isn't specified, then all schemas in the search path are checked for the config table (not just 'public')
- When the schema is set explicitly in the connection URL, the search path is restricted just to that schema

Fixes #129 ?
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 02:48:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                depends on #170 

Updated lerna to newer version to remove dependabot security issues.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 19:30:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-askar/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Adjust permissions to support uniffi module outside the repo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Please take a look @andrewwhitehead 
I could make a uniffi module as a separate crate with these changes. I added some dummy documents in error.rs and store.rs to make them public.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-05 08:26:20 +0000 UTC
    </div>
</div>

