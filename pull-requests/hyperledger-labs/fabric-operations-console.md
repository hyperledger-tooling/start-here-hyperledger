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
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/687" class=".btn">#687</a>
            </td>
            <td>
                <b>
                    Upgrade underlying runtimes/os.
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

* Upgrade console image(s) to UBI-9 base image and build images.
* Upgrade grpcweb base image to Go v1.21.9.
* Upgrade to Python v3.12 in workflows.

My motivation is that many of these OSes and runtime versions have either gone End of Life or are approaching EOL, and many of them contain known security vulnerabilities.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-09 20:36:45 +0000 UTC
    </div>
</div>

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

