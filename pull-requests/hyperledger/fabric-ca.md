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
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/319" class=".btn">#319</a>
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
        Created At 2022-10-18 21:48:35 +0000 UTC
    </div>
</div>

