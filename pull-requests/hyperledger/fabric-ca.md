---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/402" class=".btn">#402</a>
            </td>
            <td>
                <b>
                    Bump mysql to mysql-apt-config_0.8.29-1_all.deb
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump mysql to mysql-apt-config_0.8.29-1_all.deb.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 19:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/401" class=".btn">#401</a>
            </td>
            <td>
                <b>
                    Remove the Fabric 1.4 dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change is necessary to remove Fabric 1.4 dependencies in the CA.  The older dependencies are no longer maintained and a source of ongoing security exposures.  This change is the first of several to remove the the older dependencies.  This change refactors the CA to use Fabric 2.5.X dependencies.

This is a partial answer to the following:
https://github.com/hyperledger/fabric-ca/issues/376

This a refactoring effort with no new functionality.  Existing tests are sufficient.

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
        Created At 2024-01-18 19:06:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/400" class=".btn">#400</a>
            </td>
            <td>
                <b>
                    Fix jQuery issues in docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Try to fix docs so that jQuery loads on readthedocs.

#### Additional details

https://github.com/readthedocs/readthedocs.org/issues/10159#issuecomment-1478717074 has a temp fix that I'm trying.

#### Related issues

* https://github.com/readthedocs/readthedocs.org/issues/10159

#### Release Note

No impact to Fabric CA functionality. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-18 14:28:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/399" class=".btn">#399</a>
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
        Created At 2024-01-17 21:11:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/398" class=".btn">#398</a>
            </td>
            <td>
                <b>
                    Remove the Fabric 1.4 idemix dependencies and replace with IBM/idemix
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change is necessary to remove Fabric 1.4 dependencies in the CA.  The older dependencies are no longer maintained and a source of ongoing security exposures.  This change is the first of several to remove the the older dependencies.  This change refactors the idemix depencies to use github.com/IBM/idemix.

This is a partial answer to the following:
https://github.com/hyperledger/fabric-ca/issues/376

This a refactoring effort with no new functionality.  Existing tests are sufficient.

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
        Created At 2024-01-17 20:56:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    Apply the CSS.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description


#### Additional details

We haven't been using the `custom.css` that we have in our `/docs` directory for this whole time. I figured out how to make it applicable again.  This is a proposed change to how the docs look and feel.

#### Related issues

None

#### Release Note

This will have **zero** impact on Fabric-CA functionality, and will only change how the docs are _styled_, not any doc content.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 18:34:55 +0000 UTC
    </div>
</div>

