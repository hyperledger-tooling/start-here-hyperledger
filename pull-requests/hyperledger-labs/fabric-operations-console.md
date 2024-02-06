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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/619" class=".btn">#619</a>
            </td>
            <td>
                <b>
                    add channel name validation on channel creation
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
- Add validation on channel name on channel creation.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 17:07:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/618" class=".btn">#618</a>
            </td>
            <td>
                <b>
                    add object-src to the csp header in all api responses
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Improvement (security)

#### Description
- adding `object-src 'none'` to our CSP response header, this will be on all non-cached responses (cached responses already have it)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 15:09:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/617" class=".btn">#617</a>
            </td>
            <td>
                <b>
                    remove "saas" and replace "v2" text from  api paths
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Clean up

#### Description
- Removing `/saas/` from api routes (legacy text), this only effects internal routes the webapp uses
- some internal routes still used `/v2/`, changed to use `/v3/`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 14:05:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    sanitise payload of db backup api
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
- Code Improvement

#### Description
<!--- Describe your changes in detail, including motivation. -->

- Sanitise input payload of db backup api
- Improve code by duplicate conditions
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-06 08:31:21 +0000 UTC
    </div>
</div>

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

