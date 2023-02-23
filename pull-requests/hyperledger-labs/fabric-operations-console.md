---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/381" class=".btn">#381</a>
            </td>
            <td>
                <b>
                    fix errors when migrating a settings doc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes bugs when migrating the settings doc.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-23 00:40:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/380" class=".btn">#380</a>
            </td>
            <td>
                <b>
                    prevent doc conflicts during restore
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
During a restore, if a doc doesn't exist it will causes a conflict when writing the doc (paradoxically). this PR fixes that.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-22 22:23:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/379" class=".btn">#379</a>
            </td>
            <td>
                <b>
                    remove json vaildation files from backups
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
The json validation file shouldn't be in a backup, too big.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-22 20:43:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/378" class=".btn">#378</a>
            </td>
            <td>
                <b>
                    allow backup/restore from different consoles that use different db names
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Change format of backup docs to fix backup/restore flow in migration. Backup docs now include the database type, which indicates if its a session, system, or component database. Backup docs now omit the database name. The restore process will restore the database by its type against the current environment's db name.

This allows backing up and restoring from different console environments that use different names for their databases.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-22 19:22:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/377" class=".btn">#377</a>
            </td>
            <td>
                <b>
                    Content signoffs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
Updating content based on feedback.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-21 17:30:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/375" class=".btn">#375</a>
            </td>
            <td>
                <b>
                    tweak migration text, style & fix last error state
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes the error state handling in the copy-console-data & migrate-wallet steps. Also tweaks the styling of the delete instructions.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-20 17:39:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    pass error messages from new console to ui
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Error messages from the other console will now surface to the ui.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 22:22:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/373" class=".btn">#373</a>
            </td>
            <td>
                <b>
                    check steps before starting them
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (improvement to code, performance, etc)

#### Description
Check if migration steps have been completed prior to calling them. Skips them if so.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-17 19:47:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/372" class=".btn">#372</a>
            </td>
            <td>
                <b>
                    fix migration lock error handling
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
fix the lock error handling during migration. and pass jupiter errors to ui if possible.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 21:46:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    fix wording for openshift
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fix error state in migration panel

fix react warnings

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Content fix

#### Description
Improved wording on the migration panel when using openshift.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 18:09:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/370" class=".btn">#370</a>
            </td>
            <td>
                <b>
                    fix iam token crash and migration version panel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Fixes console crash when retrieving a valid iam token & tweaks the version error panel css.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 15:03:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/369" class=".btn">#369</a>
            </td>
            <td>
                <b>
                    update release notes
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
Update release notes.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 01:45:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    hook up migration apis to jupiter endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature

#### Description
More migration code. Includes calling the jupiter apis and creating the initial login credentials.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-16 01:39:24 +0000 UTC
    </div>
</div>

