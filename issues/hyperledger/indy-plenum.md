---
layout: default
title: indy-plenum
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/indy-plenum
---

# indy-plenum <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-plenum){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/indy-plenum/issues/1554" class=".btn">1554</a>
            </td>
            <td>
                <b>
                    GitHub Action CI/CD Enhancements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span><span class="chip">help wanted</span><span class="chip">Ubuntu 20.04</span>
            </td>
            <td>
                The following is a list of what the existing Jenkins Pipelines do that the GitHub Actions Workflows don't (yet).

We'll be focusing on the features and functionality of the `Jenkinsfile.cd` Pipeline, since the GitHub Actions Workflows have incorporated all of the features and functionality of the `Jenkinsfile.ci` Pipeline.

The flow of the pipeline is setup in `Jenkinsfile.cd` but the execution is controlled by the `testAndPublish` script in the `private`[sovrin-foundation/jenkins-shared](https://github.com/sovrin-foundation/jenkins-shared) repository therefore anyone working on these enhancements will need to be granted read-only access to that repository in order to follow the code.  The scripts automate the release process described here; [Indy-Node Release Workflow](https://github.com/hyperledger/indy-node/blob/master/docs/source/ci-cd.md#release-workflow).  The same scripts are used for both `indy-node` and `indy-plenum`.

- [ ] Configure auto-merge on PRs containing changes to `setup.py` and no other files.
- [ ] Update the release version on release candidate (`isRC`) PRs.
- [ ] Conditionally build (for release candidates) or repack (for releases) artifacts.
- [ ] Promote/copy artifacts (deb packages) to different locations in the repository.
- [ ] Optionally run system tests (this feature is used for `indy-node`, but not `indy-plenum`).
- [ ] Create a release PR for (off) RC PRs.
- [ ] Notify a mailing list that a new RC release is waiting for approval, and then wait for the release to be approved.
- [ ] Merge approved release candidate PRs into the release branch.
- [ ] Notify a mailing list that a new release is available.
- [ ] Rollback release commits on PRs when the release is not approved.

When developing the enhancements a separate issue should be created to track the work and be linked back to this issue.  Feature enhancements should be limited to the smallest set of related features in order to limit the scope of the work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 21:33:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/indy-plenum/issues/1553" class=".btn">1553</a>
            </td>
            <td>
                <b>
                    Remove Jenkinsfile.ci Pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">Ubuntu 20.04</span>
            </td>
            <td>
                GitHub Actions based workflows have been developed, on both the main branch and the ubuntu-20.04-upgrade branch, to replace all of the functionality of the Jenkinsfile.ci pipeline.

Jenkinsfile.ci can safely be removed from the ubuntu-20.04-upgrade branch so when the branch is eventually merged into the main branch the file will be removed there as well.

This should be done after https://github.com/hyperledger/indy-plenum/pull/1545 is merged.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 15:49:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/indy-plenum/issues/1552" class=".btn">1552</a>
            </td>
            <td>
                <b>
                    Upgrade and unpin remaining dependencies 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span><span class="chip">good first issue</span><span class="chip">Ubuntu 20.04</span><span class="chip">upgrade</span>
            </td>
            <td>
                An overview of all installed, referenced, and required PyPI packages can be found here: [Hyperledger Indy-Plenum | Dependency management Ubuntu 20](https://docs.google.com/document/d/1445VZL3qHBmuVbzm-K9O7te_63zKKlyv6mrEwiJcL3Y/edit?usp=sharing)

As discussed here, Issue https://github.com/hyperledger/indy-plenum/issues/1544, there are still several dependencies that need to be upgraded following the initial Ubuntu 20.04 release.

Where possible the dependencies should be upgraded individually to reduce the scope of the work, and a separate issue linking back to this one should be created to track the work.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-07-27 15:15:47 +0000 UTC
    </div>
</div>

