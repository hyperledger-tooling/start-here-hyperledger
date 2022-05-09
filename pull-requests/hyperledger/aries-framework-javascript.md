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
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/754" class=".btn">#754</a>
            </td>
            <td>
                <b>
                    chore!: update indy-sdk-react-native version to 0.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Amit <amit@northernblock.io>

Update indy-sdk-react-native version to 0.2.0 to support

- chore!: update indy SDK version to 1.16 for android
- chore(deps): bump plist from 3.0.4 to 3.0.5
- chore(deps): bump async from 2.6.3 to 2.6.4
- chore: update indy framework source link
- 

Issue - https://github.com/hyperledger/aries-framework-javascript/issues/752


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-09 10:46:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    fix: do not import from src dir
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some files had `src` in their path meaning the files couldn't actually be found when published to NPM. 

We should probably look to run the tests (at least the root `tests`) using the built files so we can make sure the npm version will work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-07 09:25:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/746" class=".btn">#746</a>
            </td>
            <td>
                <b>
                    fix: do not import test logger in src
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also updates the ci to add the build script (in addition to check types) so this doesn't happen again.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 15:36:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/745" class=".btn">#745</a>
            </td>
            <td>
                <b>
                    feat: add issue credential v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Mike Richardson <mike.richardson@northernblock.io>

BEGIN_COMMIT_OVERRIDE
feat: add issue credential v2

BREAKING CHANGE: the issue credential module has been extended to support both v1 and v2 of protocol. See [Migrating from AFJ 0.1.0 to 0.2.x](https://github.com/hyperledger/aries-framework-javascript/blob/main/docs/migration/0.1-to-0.2.md) for a detailed migration instructions.
END_COMMIT_OVERRIDE
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-06 13:02:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/736" class=".btn">#736</a>
            </td>
            <td>
                <b>
                    fix: mediation record checks for pickup v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds checks in the mediation recipient service for mediation record state and role. Also splits up the sending of the status request message to be more in line with separation of service/module in the rest of the framework. 

Finally, this updates the processing of the message to be using the event emitter. We also use this approach for pickup v1 and it was causing issues in the oob branch due to circular dependencies.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-05-02 22:03:08 +0000 UTC
    </div>
</div>

