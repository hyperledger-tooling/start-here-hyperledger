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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/556" class=".btn">#556</a>
            </td>
            <td>
                <b>
                    Audit logs cleanup
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
more audit log improvements
- added log for deleting users
- added log for mustgather actions
- fix search box on audit log page (under some circumstances it didn't work correctly)
- removed text "IBP" from a user login log
- added name of ordering service to log when deleting an ordering service

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-07 19:18:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/554" class=".btn">#554</a>
            </td>
            <td>
                <b>
                    Upgrade browserify-sign to 4.2.2 to address CVE.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

Upgrade npm browserify-sign in apollo to 4.2.2 to address https://nvd.nist.gov/vuln/detail/CVE-2023-46234
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 20:24:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/553" class=".btn">#553</a>
            </td>
            <td>
                <b>
                    changes as per pipeline execution
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change
- Test update

#### Description
- Removed package lock json
- Added new tag to run on existing console and regression
- Update in tests as per pipeline execution (Cypress launches test runner / browser with clean state after each feature file execution and that clears the local storage / identities)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 12:37:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/552" class=".btn">#552</a>
            </td>
            <td>
                <b>
                    tidy up audit log messages/events
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
many bug fixes/improvements on the audit log panel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-02 21:06:42 +0000 UTC
    </div>
</div>

