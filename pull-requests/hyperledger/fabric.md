---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2576" class=".btn">#2576</a>
            </td>
            <td>
                <b>
                    removing -a from docker ps command as it lists stopped containers also
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: System Administrator <root@Rahuls-MacBook-Air.local>

Removing -a from 'docker ps' commnand, since it lists stopped containers also

<!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-01 20:17:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2574" class=".btn">#2574</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wuqiaomin <wuqiaomin2@huawei.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 06:47:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2573" class=".btn">#2573</a>
            </td>
            <td>
                <b>
                    Feature/fix trouble with pkcs11
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Fix troubles with PKCS11

#### Type of change

- Bug fix

#### Description

Simple changes that fix these errors on 1.4 Path:
- When setting ORDERER_GENERAL_BCCSP_PKCS11_SECURITY orderer variable the orderer fails saying that the security value is a string and not an int.
- When running `GO_TAGS=pkcs11 make docker` the fabric-tools docker image doesn't include a PKCS11 provider.

#### Related issues

https://jira.hyperledger.org/browse/FAB-18457


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 20:36:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2572" class=".btn">#2572</a>
            </td>
            <td>
                <b>
                    Fix incorrect error message in Gateway submit
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As pointed out in previous PR review, the error message was incorrect when the gateway can’t connect to the BroadcastClient. (https://github.com/hyperledger/fabric/pull/2508#discussion_r601777021)

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-29 10:50:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2570" class=".btn">#2570</a>
            </td>
            <td>
                <b>
                    FABGW-19: Secure CommitStatus service
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 16:10:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2569" class=".btn">#2569</a>
            </td>
            <td>
                <b>
                    fix typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: wuqiaomin <wuqiaomin2@huawei.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 06:15:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/2568" class=".btn">#2568</a>
            </td>
            <td>
                <b>
                    Corrected function name in comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: sukill <ckdrms622@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-27 06:58:15 +0000 UTC
    </div>
</div>

