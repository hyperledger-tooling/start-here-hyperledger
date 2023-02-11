---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    0.8.0-rc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    0.8.0-rc0
                </span>
            </td>
            <td>
                # 0.8.0-rc0

## February 8, 2023

0.8.0 is a breaking change release that contains all updates since release 0.7.5. It extends the previously tagged `1.0.0-rc1` release because it is not clear when that release will be finalized. Many of the PRs in this release were previously included in the `1.0.0-rc1` release. The categorized list of PRs separates those that are new from those in the `1.0.0-rc1` release candidate. See the [Changelog for v0.8.0-rc0](https://github.com/hyperledger/aries-cloudagent-python/blob/0.8.0-rc0/CHANGELOG.md#100-rc0) for all changes since v0.7.5.

There are not a lot of new Aries Framework features in the release, as the focus has been on cleanup and optimization. The biggest addition is the inclusion with ACA-Py of a universal resolver interface, allowing an instance to have both local resolvers for some DID Methods and a call out to an external universal resolver for other DID Methods. Another significant new capability is full support for Hyperledger Indy transaction endorsement for Authors and Endorsers. A new repo [aries-endorser-service](https://github.com/hyperledger/aries-endorser-service) has been created that is a pre-configured instance of ACA-Py for use as an Endorser service.

### Container Publishing Updated

With this release, a new automated process publishes container images in the Hyperledger container image repository. New images for the release are automatically published by the GitHubAction Workflows: [publish.yml] and [publish-indy.yml]. The actions are triggered when a release is tagged, so no manual action is needed. The images are published in the [Hyperledger Package Repository under aries-cloudagent-python] and a link to the packages added to the repositories main page (under "Packages"). Additional information about the container image publication process can be found in the document [Container Images and Github Actions].

The ACA-Py container images are based on [Python 3.6 and 3.9 `slim-bullseye` images](https://hub.docker.com/_/python), and are built to support `linux/386 (x86)`, `linux/amd64 (x64)`, and `linux/arm64`. There are two flavors of image built for each Python version. One contains only the Indy/Aries Shared Libraries only ([Aries Askar](https://github.com/hyperledger/aries-askar), [Indy VDR](https://github.com/hyperledger/indy-vdr) and [Indy Shared RS](https://github.com/hyperledger/indy-shared-rs), supporting only the use of `--wallet-type askar`). The other (labelled `indy`) contains the Indy/Aries shared libraries and the Indy SDK (considered deprecated). For new deployments, we recommend using the Python 3.9 Shared Library images. For existing deployments, we recommend migrating to those images. For those migrating an Indy SDK deployment, a new secure storage database migration capability from Indy SDK to Aries Askar is available--contact the ACA-Py maintainers on Hyperledger Discord for details.

Those currently using the container images published by [BC Gov on Docker Hub](https://hub.docker.com/r/bcgovimages/aries-cloudagent) should change to use those published to the [Hyperledger Package Repository under aries-cloudagent-python].

[Hyperledger Package Repository under aries-cloudagent-python]: https://github.com/orgs/hyperledger/packages?repo_name=aries-cloudagent-python
[publish.yml]: https://github.com/hyperledger/aries-cloudagent-python/blob/main/.github/workflows/publish.yml
[publish-indy.yml]: https://github.com/hyperledger/aries-cloudagent-python/blob/main/.github/workflows/publish-indy.yml
[Container Images and Github Actions]: https://github.com/hyperledger/aries-cloudagent-python/blob/main/ContainerImagesAndGithubActions.md

**Full Changelog**: https://github.com/hyperledger/aries-cloudagent-python/compare/0.7.5...0.8.0-rc0
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/aries-cloudagent-python/releases/tag/0.8.0-rc0" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2023-02-10 23:21:21 +0000 UTC
    </span>
</div>

