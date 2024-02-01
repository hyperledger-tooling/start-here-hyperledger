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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/605" class=".btn">#605</a>
            </td>
            <td>
                <b>
                    update releaes notes
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
update release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 21:31:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/604" class=".btn">#604</a>
            </td>
            <td>
                <b>
                    change the prefixes found on exported files to FOC instead of IBP
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
zip files and json files that were downloaded used a legacy prefix of `IBP`, changing that to `FOC`. 
- example filename with this PR: `FOC.1-26-2024-42454.zip`



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 21:26:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/603" class=".btn">#603</a>
            </td>
            <td>
                <b>
                    Fix create component modals - default choice
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

  - in the import/deploy component modal for CAs, peers, and OS's, it was defaulting to the deploy flow, even if that choice was not available
  - the app was hiding the deploy option if it was not available, but it will now show as a disabled choice


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 20:51:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/602" class=".btn">#602</a>
            </td>
            <td>
                <b>
                    Upgrade deployer to latest Docker Golang client.
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

As per CVE-2023-28842 and many others.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 19:20:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/601" class=".btn">#601</a>
            </td>
            <td>
                <b>
                    Address CVE-2022-1996. emicklei/go-restful.
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
CVE-2022-1996: https://nvd.nist.gov/vuln/detail/CVE-2022-1996

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-26 19:04:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/600" class=".btn">#600</a>
            </td>
            <td>
                <b>
                    reduce cache expiration from 2 minutes to 1.5 minutes
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
Lowers the cache expiration of component status APIs from 120 seconds to 90 seconds.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 14:36:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/599" class=".btn">#599</a>
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
Update release notes


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-25 14:15:14 +0000 UTC
    </div>
</div>

