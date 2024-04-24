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
                PR <a href="https://github.com/hyperledger/fabric/pull/4825" class=".btn">#4825</a>
            </td>
            <td>
                <b>
                    adding external chaincode binaries to the base peer image WIP
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Simplify the use of external chaincodes

#### Type of change

- New feature
- Improvement (improvement to code, performance, etc)

Might be a new feature or an improvement.

#### Description

Using external chaincode as a service needs to change the peer image providing three binaries (detect/build/release). To simplify the setup for use cases where docker (podman, kubernetes, openshift to name a few) is not available you are forced to use external chaincodes.

#### Additional details

As its basically my first PR for fabric, feedback regarding tools/guidelines would be appreciated.
Maybe, the functionality could be moved into the existing tools in ccaasbuilder, but I wont risk a bug there.

#### Related issues

#### Release Note

The change wont impact existing installations

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
        Created At 2024-04-24 09:50:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4824" class=".btn">#4824</a>
            </td>
            <td>
                <b>
                    chore: use errors.New to replace fmt.Errorf with no parameters will much better.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                use errors.New to replace fmt.Errorf with no parameters.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-22 01:49:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4823" class=".btn">#4823</a>
            </td>
            <td>
                <b>
                    chore: fix some typos in comments
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

fix some typos in comments
<!--- Describe your changes in detail, including motivation. -->

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

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
        Created At 2024-04-19 11:45:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4822" class=".btn">#4822</a>
            </td>
            <td>
                <b>
                    chore: Optimize many comments including structure names and typos
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

- Bug fix
- New feature
- Improvement (improvement to code, performance, etc)
- Test update
- Documentation update

#### Description

Optimize many comments including structure names and typos

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

No

#### Related issues

No

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

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
        Created At 2024-04-18 03:54:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4821" class=".btn">#4821</a>
            </td>
            <td>
                <b>
                    smartbft sync is called after restart test
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

smartbft sync is called after restart

#### Related issues

Issue #4732
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 16:09:46 +0000 UTC
    </div>
</div>

