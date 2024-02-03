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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Changes as per timeout error in pipeline
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
Changes as per timeout error in pipeline

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 10:28:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/614" class=".btn">#614</a>
            </td>
            <td>
                <b>
                    Improved Deployer Logs for Mustgather Endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### - Improvement (improvement to code, performance, etc)

#### Description
The endpoints for Mustgather which are called by console, needed more logging so that we can debug and trouble shoot in production incase of errors.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-02 06:17:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/613" class=".btn">#613</a>
            </td>
            <td>
                <b>
                    changed input validation b/c available client and server log levels a…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                …re different + remove redundant validation

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- removes redundant input validation on the logging settings api (from legacy)
- client and server log levels have different options, fixed


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 15:51:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/612" class=".btn">#612</a>
            </td>
            <td>
                <b>
                    fixes yaml parsing
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
YAML to JSON parsing was broken, `safeDump()` is not longer in the yaml library.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 15:34:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/611" class=".btn">#611</a>
            </td>
            <td>
                <b>
                    hide mustgather section for readers and writers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Improvement (improvement to code, performance, etc)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-01 09:01:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/610" class=".btn">#610</a>
            </td>
            <td>
                <b>
                    fixes mustgather download button w/axios
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
Fixes the mustgather download zip button, the previous route for this download was using a `request.get` and a `pipe` method which are not available in our axios-request wrapper.

this fix does require rebuilding the URL allow list, which will happen on startup automatically


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-31 15:38:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/609" class=".btn">#609</a>
            </td>
            <td>
                <b>
                    add vs code option to always add "sign off"
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Other

#### Description
adds VScode setting to always add git "sign off" line to commit message


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 19:00:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/608" class=".btn">#608</a>
            </td>
            <td>
                <b>
                    bump release notes
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
Updating release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 18:43:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/607" class=".btn">#607</a>
            </td>
            <td>
                <b>
                    fixes deploy ca flow, hides unselected steps
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
The last build was incorrectly showing steps during the deploy CA flow that were not selected. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 18:36:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/606" class=".btn">#606</a>
            </td>
            <td>
                <b>
                    Update audit log message while fail to adding peers to channel
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
<!--- Describe your changes in detail, including motivation. -->
- Update audit log message and status code while fail to add peers to channel.
- Add Audit log entry on Join Orderer peer to existing channel
- Add Audit log entry on disconnect orderer peer from channel


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-29 16:13:51 +0000 UTC
    </div>
</div>

