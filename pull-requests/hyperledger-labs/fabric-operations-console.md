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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/433" class=".btn">#433</a>
            </td>
            <td>
                <b>
                    tidy up console restart apis
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
- console restart apis will now log the process id that is restarting
- added restart api that will kill the process (which kills the pod) `ak/api/v[123]/restart/force/hard`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:11:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/432" class=".btn">#432</a>
            </td>
            <td>
                <b>
                    add debug log for couch db connection errors
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
- during startup the console will now wait up to 90 seconds (was 60) for the database
- adds connection error to log if the console cannot connect to couchdb during startup
- also conforms the log messages


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:08:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/431" class=".btn">#431</a>
            </td>
            <td>
                <b>
                    disable keep alive on incoming connections
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
Security recommendation, disable keep alives.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 19:00:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/430" class=".btn">#430</a>
            </td>
            <td>
                <b>
                    compress console database backups and use fs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement

#### Description

- console database backups will be temporary stored to the filesystem to avoid cloudant size limits
- console database backups will be compressed to minimize transfer sizes during migration

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-03 18:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/429" class=".btn">#429</a>
            </td>
            <td>
                <b>
                    fix resource vaildation
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
Fix the resource input validation for CPU, memory and storage.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 20:14:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/428" class=".btn">#428</a>
            </td>
            <td>
                <b>
                    Fix safelist port
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
Fixes the unsafe url error from the new safe-url validation when creating a peer or os. the port and hostname are in separate fields in this api and had to be combined to pass validation .


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 17:13:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/427" class=".btn">#427</a>
            </td>
            <td>
                <b>
                    Pen test Input Validation update
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
<!--- Describe your changes in detail, including motivation. -->
Pen test Input Validation update

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-30 12:06:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/426" class=".btn">#426</a>
            </td>
            <td>
                <b>
                    update activity tracker doc
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
Update the doc on activity tracker and allow it to be turned on* via the setting.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-29 20:22:23 +0000 UTC
    </div>
</div>

