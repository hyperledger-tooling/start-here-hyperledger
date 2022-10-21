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
                PR <a href="https://github.com/hyperledger/fabric/pull/3708" class=".btn">#3708</a>
            </td>
            <td>
                <b>
                    Changed Linux to Linux(Ubuntu/Debian based distro)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Signed-off-by: Ayush Choudhury <41822282+sunflowermarmalade@users.noreply.github.com>

#### Type of change

- Documentation update

#### Description
The readme provided will only work for Ubuntu or Debian-based distributions and not on any kind of Linux environment


#### Additional details
I can add documentation regarding more linux distributions which will have somewhat different commands if required.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-21 03:30:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3706" class=".btn">#3706</a>
            </td>
            <td>
                <b>
                    Release Workflow
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- New feature
- Improvement (improvement to code, performance, etc)

#### Description

<!--- Describe your changes in detail, including motivation. -->

- Release workflow automates new release creation process similar the current Azure Pipelines release job
- Generates binaries for linux, darwin, and windows targets, pushes Docker images to Hyperledger DockerHub, and creates a new tag and release with artifacts for given version number based off of main branch latest commit
- Workflow must be manually triggered from Actions tab and requires input for the version number and two digit version number similar to Azure Pipelines
- GitHub secrets for DOCKERHUB_PASSWORD and DOCKERHUB_USERNAME must be added to repository matching Hyperledger DockerHub credentials before workflow can be run successfully


<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->


<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
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
        Created At 2022-10-20 18:20:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3705" class=".btn">#3705</a>
            </td>
            <td>
                <b>
                    Commit path changes for private data purge
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables processing of purge operation in a transaction during block commit

Signed-off-by: manish <manish.sethi@gmail.com>

#### Type of change
- New feature
#### Related issues
Closes #3026
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-19 23:49:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3701" class=".btn">#3701</a>
            </td>
            <td>
                <b>
                    Move inactive maintainers to emeritus status
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The TOC approved a requirement that maintainers
that have not been active in over three to six
months be move to emeritus status.

These maintainers have not been active in over
one year.

hyperledger/toc#32

Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-18 18:43:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3699" class=".btn">#3699</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos (backport #3698)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3698 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 17:22:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3698" class=".btn">#3698</a>
            </td>
            <td>
                <b>
                    Use safe accessors for RWset protos
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the Getter functions rather than direct access to fields in the proto structures.

Backport of https://github.com/hyperledger/fabric/pull/3686 with modified unit test for different proto behaviour.

Signed-off-by: andrew-coleman <andrew_coleman@uk.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-17 15:34:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3697" class=".btn">#3697</a>
            </td>
            <td>
                <b>
                    Use env variables to initialize the PKCS11 BCCSP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The environment variables to configure the PKCS11 BCCSP are ignored for the peer node, such as CORE_PEER_BCCSP_PKCS11_LIBRARY. This change allows specifying the BCCSP Default and to configure all of the PKCS11 BCCSP settings using environment variables.

This is an alternative solution to the problem proposed in https://github.com/hyperledger/fabric/pull/3681

Signed-off-by: Fred Partanskiy <pfi79@mail.ru>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 15:06:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3696" class=".btn">#3696</a>
            </td>
            <td>
                <b>
                    Add delivery client logging (backport #3692 release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add logging for delivery client connections to ordering service, as well as disconnections.
This will help with troubleshooting when connections between peer and orderer are in doubt.

Also improve related log messages and config descriptions.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 15:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3694" class=".btn">#3694</a>
            </td>
            <td>
                <b>
                    Add delivery client logging (backport #3692 release-2.4)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3692 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 14:05:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3693" class=".btn">#3693</a>
            </td>
            <td>
                <b>
                    Add delivery client logging (backport #3692 release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #3692 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 14:05:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/3692" class=".btn">#3692</a>
            </td>
            <td>
                <b>
                    Add delivery client logging
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add logging for delivery client connections to ordering service, as well as disconnections.
This will help with troubleshooting when connections between peer and orderer are in doubt.

Also improve related log messages and config descriptions.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-10-15 05:19:54 +0000 UTC
    </div>
</div>

