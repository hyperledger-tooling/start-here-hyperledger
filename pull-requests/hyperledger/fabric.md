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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4611" class=".btn">#4611</a>
            </td>
            <td>
                <b>
                    Use the named var for build dir
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Use the variable instead of build path string.

Change-Id: I0c8663cdfe9c7c546694a3edfb7a09d10ba2af69

#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

The file already has the build variable, hence should use it.


#### Additional details

N/A

#### Related issues

N/A

#### Release Note

N/A
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 22:18:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4610" class=".btn">#4610</a>
            </td>
            <td>
                <b>
                    Configured orderer's backoff for the gateway tests.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Сonfigured backoff in orderers for gateway tests, so that after restart other orderers will find the newly started one.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 17:58:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4609" class=".btn">#4609</a>
            </td>
            <td>
                <b>
                    Add doc for CA cert renewal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add doc for CA cert renewal.

Resolves #4573.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 17:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4605" class=".btn">#4605</a>
            </td>
            <td>
                <b>
                    Update docs on queryapproved to query all approved definitions
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

- Documentation update

#### Description

This patch updates documents on `queryapproved` to query all approved definitions.

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Jira issue or approved rfc. -->
Resolve https://github.com/hyperledger/fabric/issues/4564

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
        Created At 2024-01-13 02:46:15 +0000 UTC
    </div>
</div>

