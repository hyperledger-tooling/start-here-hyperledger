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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/686" class=".btn">#686</a>
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
<!--- Describe your changes in detail, including motivation. -->

- Update release notes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 13:59:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/685" class=".btn">#685</a>
            </td>
            <td>
                <b>
                    added condition for migrated component to return os style urls
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
<!--- Describe your changes in detail, including motivation. -->

the console currently uses the field migrated_from="ibm_saas" to decide if it should use the legacy (saas) set of urls to communicate to the component, or the opensource-operator styled urls. this change allows a new field called preferred_url to be set (per component) to "os", which would allow a migrated(saas) component to return with the open-source style of urls.

> "preferred_url" - The style/format of a url to return for a migrated component. Does not apply to non-migrated components. Set to "os" to return open-source operator urls for these field: api_url, operations_url and osnadmin_url. Otherwise migrated components will return the legacy ("saas") style urls.

- effects apis like:
    - get-component
    - get-all-components


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 13:41:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Renew MSP admin certificate
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
- Renew MSP admin certificate fix.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 08:44:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    os node add to existing channel fix
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

- Join existing channel by ordering service node without system channel, give warning if OS node msp does not part of channel

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 07:02:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Upgrade google.golang.org/protobuf for CVE-2024-24786.
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

[CVE-2024-24786](https://nvd.nist.gov/vuln/detail/CVE-2024-24786)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 19:10:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/681" class=".btn">#681</a>
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
<!--- Describe your changes in detail, including motivation. -->
- Update release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-03 06:00:30 +0000 UTC
    </div>
</div>

