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
                PR <a href="https://github.com/hyperledger/fabric/pull/4634" class=".btn">#4634</a>
            </td>
            <td>
                <b>
                    Re-add the RSA definitions to BCCSP - RSA implementation additional c…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BCCSP supported RSA in version 1.4. The Fabric CA is currently using the Fabric 1.4 dependency. It is necessary to move Fabric CA off of Fabric 1.4 dependencies since they are no longer maintained. Fabric 2.X does not support RSA, however the CA still needs to support RSA for any older but not expired certificates that may be in use by older netwo

Github:
https://github.com/hyperledger/fabric/issues/4625


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 23:27:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4632" class=".btn">#4632</a>
            </td>
            <td>
                <b>
                    Fix docs that link to .md files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Docs should link to the .html file rather than the .md file in order to get resolved.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 22:38:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4631" class=".btn">#4631</a>
            </td>
            <td>
                <b>
                    Add TLS passthrough and SANs info to TLS doc (backport #4568)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4568 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 16:13:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4630" class=".btn">#4630</a>
            </td>
            <td>
                <b>
                    refactor gateway bft test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The test is really short on time. 
But I decided not to increase the time, 
but to break the test into separate time intervals.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 14:21:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4629" class=".btn">#4629</a>
            </td>
            <td>
                <b>
                    Update documents to remove remaining descriptions on JIRA (backport #4628)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4628 done by [Mergify](https://mergify.com).


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

Additionally, on Mergify [dashboard](https://dashboard.mergify.com) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-22 14:10:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4628" class=".btn">#4628</a>
            </td>
            <td>
                <b>
                    Update documents to remove remaining descriptions on JIRA
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This patch removes remaining descriptions regarding JIRA in the repository. Also, it includes minor improvements of docs.

#### Type of change

- Documentation update

#### Description
It seems the Hyperledger JIRA instance was sunset at the end of last year.
On the other hands, there are some remaining descriptions regarding JIRA in the repository.
So, this patch removes the remaining descriptions. Also, it includes some minor improvements of docs.

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
        Created At 2024-01-22 06:26:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4627" class=".btn">#4627</a>
            </td>
            <td>
                <b>
                    Re-add the RSA definitions to BCCSP - RSA implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    BCCSP supported RSA in version 1.4. The Fabric CA is currently using the Fabric 1.4 dependency.
    It is necessary to move Fabric CA off of Fabric 1.4 dependencies since they are no longer maintained.
    Fabric 2.X does not support RSA, however the CA still needs to support RSA for any older but not expired certificates that may be in use by older netwo

    Github:
    https://github.com/hyperledger/fabric/issues/4625
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-20 16:19:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4626" class=".btn">#4626</a>
            </td>
            <td>
                <b>
                    Re-add the RSA definitions to BCCSP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BCCSP supported RSA in version 1.4. The Fabric CA is currently using the Fabric 1.4 dependency. It is necessary to move Fabric CA off of Fabric 1.4 dependencies since they are no longer maintained. Fabric 2.X does not support RSA, however the CA still needs to support RSA for any older but not expired certificates that may be in use by older netwo

Github:
https://github.com/hyperledger/fabric/issues/4625

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-19 19:14:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4623" class=".btn">#4623</a>
            </td>
            <td>
                <b>
                    Fix the jQuery issue in the docs on release-2.5 branch 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **This PR is for the release-2.5 branch**

#### Type of change

- Documentation update

#### Description

jQuery was not loading the readthedocs menu to allow for viewing different doc versions. This commit fixes that.

#### Additional details

Found the fix here: https://github.com/readthedocs/readthedocs.org/issues/10159

#### Related issues

https://github.com/hyperledger/fabric/issues/4620.

#### Release Note
No impact on Fabric Functionality.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 15:06:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4622" class=".btn">#4622</a>
            </td>
            <td>
                <b>
                    Fix the jQuery issue in the docs on release-2.2 branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **This PR is for the release-2.2 branch**

#### Type of change

- Documentation update

#### Description

jQuery was not loading the readthedocs menu to allow for viewing different doc versions. This commit fixes that.

#### Additional details

Found the fix here: https://github.com/readthedocs/readthedocs.org/issues/10159

#### Related issues

https://github.com/hyperledger/fabric/issues/4620.

#### Release Note
No impact on Fabric Functionality.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 14:58:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4621" class=".btn">#4621</a>
            </td>
            <td>
                <b>
                    Fix the jQuery issue in the docs on main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **This PR is for the main branch**

#### Type of change

- Documentation update

#### Description

jQuery was not loading the readthedocs menu to allow for viewing different doc versions. This commit fixes that.

#### Additional details

Found the fix here: https://github.com/readthedocs/readthedocs.org/issues/10159

#### Related issues

https://github.com/hyperledger/fabric/issues/4620.

#### Release Note
No impact on Fabric Functionality.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 14:39:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4619" class=".btn">#4619</a>
            </td>
            <td>
                <b>
                    Fix inter-page links with MyST options in docs.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

**This is for the release-2.5 branch**

- Documentation update

#### Description

The new parser (MyST) for Markdown files was interpreting relative links (e.g. `../../file.html`) as anchors (e.g. `#../../file.html`) which doesn't help.  This changes the docs configuration to stop doing that.

#### Additional details

Sphinx moved to MyST for parsing Markdown files. This is the config page: https://myst-parser.readthedocs.io/en/latest/configuration.html#global-configuration

#### Related issues

N/A

#### Release Note
This will have no effect on Fabric functionality, but will change how the docs link to each other.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 21:08:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4618" class=".btn">#4618</a>
            </td>
            <td>
                <b>
                    Fix inter-page links with MyST options in docs.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

**This is for the main branch**

- Documentation update

#### Description

The new parser (MyST) for Markdown files was interpreting relative links (e.g. `../../file.html`) as anchors (e.g. `#../../file.html`) which doesn't help.  This changes the docs configuration to stop doing that.

#### Additional details

Sphinx moved to MyST for parsing Markdown files. This is the config page: https://myst-parser.readthedocs.io/en/latest/configuration.html#global-configuration

#### Related issues

N/A

#### Release Note
This will have no effect on Fabric functionality, but will change how the docs link to each other.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 21:04:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4616" class=".btn">#4616</a>
            </td>
            <td>
                <b>
                    Upgrade Jinja2 to v3.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **This is for the release-2.2 branch**.

The version of Sphinx we were using is simply not compatible with Jinja2 > v3.0.3, so given that we had to upset the delicate balance of requirements anyway, the goal of this PR is now to bring all docs infrastructure for CI/CD as well as dependencies and indeed the docs themselves to the latest version.

#### Type of change

- Documentation update

#### Description

Motivation is https://nvd.nist.gov/vuln/detail/CVE-2024-22195, quite simply. But the version of Sphinx that we were using was many years old and does not support a version of Jinja higher than v3.0.3.  So we need to update the entire set of dependencies for the documentation.

#### Additional details

I will make whatever changes are needed to the docs and/or to the CI/CD pipeline to make this compatible with Sphinx v7.2.6, which is the latest.  Please let me know if something isn't right or needs fixing, because this is the time to do it.

#### Related issues

* https://github.com/hyperledger/fabric/issues/4607.

#### Release Note

This change does **NOT** impact users of Fabric, nor shall it impact the functionality of **any** release, past, future, present.   We are also unlikely to merge it until the docs look correct on RTD.  But be advised that they may indeed change.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 19:57:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4615" class=".btn">#4615</a>
            </td>
            <td>
                <b>
                    Upgrade Jinja2 to v3.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **This is for the release-2.5 branch**.

The version of Sphinx we were using is simply not compatible with Jinja2 > v3.0.3, so given that we had to upset the delicate balance of requirements anyway, the goal of this PR is now to bring all docs infrastructure for CI/CD as well as dependencies and indeed the docs themselves to the latest version.

#### Type of change

- Documentation update

#### Description

Motivation is https://nvd.nist.gov/vuln/detail/CVE-2024-22195, quite simply. But the version of Sphinx that we were using was many years old and does not support a version of Jinja higher than v3.0.3.  So we need to update the entire set of dependencies for the documentation.

#### Additional details

I will make whatever changes are needed to the docs and/or to the CI/CD pipeline to make this compatible with Sphinx v7.2.6, which is the latest.  Please let me know if something isn't right or needs fixing, because this is the time to do it.

#### Related issues

* https://github.com/hyperledger/fabric/issues/4607.

#### Release Note

This change does **NOT** impact users of Fabric, nor shall it impact the functionality of **any** release, past, future, present.   We are also unlikely to merge it until the docs look correct on RTD.  But be advised that they may indeed change.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 19:43:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4613" class=".btn">#4613</a>
            </td>
            <td>
                <b>
                    Upgrade Jinja2 to v3.1.3 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **This is for the main branch**.

The version of Sphinx we were using is simply not compatible with Jinja2 > v3.0.3, so given that we had to upset the delicate balance of requirements anyway, the goal of this PR is now to bring all docs infrastructure for CI/CD as well as dependencies and indeed the docs themselves to the latest version.

#### Type of change

- Documentation update

#### Description

Motivation is https://nvd.nist.gov/vuln/detail/CVE-2024-22195, quite simply. But the version of Sphinx that we were using was many years old and does not support a version of Jinja higher than v3.0.3.  So we need to update the entire set of dependencies for the documentation.

#### Additional details

I will make whatever changes are needed to the docs and/or to the CI/CD pipeline to make this compatible with Sphinx v7.2.6, which is the latest.  Please let me know if something isn't right or needs fixing, because this is the time to do it.

#### Related issues

* https://github.com/hyperledger/fabric/issues/4607.

#### Release Note

This change does **NOT** impact users of Fabric, nor shall it impact the functionality of **any** release, past, future, present.   We are also unlikely to merge it until the docs look correct on RTD.  But be advised that they may indeed change.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 18:38:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4612" class=".btn">#4612</a>
            </td>
            <td>
                <b>
                    Malicious Block Deliverer Test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Test update: Add a test that will checkout how the block deliverer acts with a malicious orderer in the network.

- Description: The test creates a network, creates blocks on the chain, replaces the orderers with mocks and communicates with the peer.

<arkadi.piven@ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 11:02:53 +0000 UTC
    </div>
</div>

