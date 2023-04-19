---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1437" class=".btn">#1437</a>
            </td>
            <td>
                <b>
                    chore: export askar types
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 08:05:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1436" class=".btn">#1436</a>
            </td>
            <td>
                <b>
                    chore(ci): switch to dedicated Aries runners
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-19 00:31:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1435" class=".btn">#1435</a>
            </td>
            <td>
                <b>
                    feat: Add cheqd demo and localnet for tests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the required Readme files and integrates cheqd modules in the demo

Also included a setup-cheqd in ./.github/actions which starts a localnet for the tests to be run
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-17 12:33:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1434" class=".btn">#1434</a>
            </td>
            <td>
                <b>
                    fix(indy-vdr): do not force indy-vdr version
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'm not sure if @hyperledger/indy-vdr-shared and @hyperledger/indy-vdr-nodejs versions are fixed to a particular version on purpose, but tests seem to work fine on the latest 0.1.0-dev.14.

This is mainly to fix https://github.com/hyperledger/aries-agent-test-harness/issues/669. If the version should be fixed to dev.13, another possibility is to fix it in the AATH backchannel.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-16 14:56:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1433" class=".btn">#1433</a>
            </td>
            <td>
                <b>
                    fix(connections): store imageUrl when using DIDExchange
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                It was already fixed for Connection protocol in https://github.com/hyperledger/aries-framework-javascript/pull/896 but missing for DID Exchange.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-14 18:46:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1431" class=".btn">#1431</a>
            </td>
            <td>
                <b>
                    fix: issuance with unqualified identifiers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bigger PR than anticipated, but this fixes the issuance of credentials with unqualified identifiers. You can now issue with both unqulaiifed and did indy identifiers interchangeably, but only for the issuance side. the other sides don't work interchangeably yet. 

I hope this is one of the last big tasks before releasing 0.4.0?

Lot of code is moving around stuff and removing some of the duplicated code. We now have indy specific identifier code in the anoncreds package, but it's needed for the unqualified handling. As it's part of the spec, and it can provide the easiest migration path, that is okay by me. (it's not much, just some identifier parsing etc..)

Hope this doesn't clash too much with your Revocation pr @genaris 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 18:57:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1429" class=".btn">#1429</a>
            </td>
            <td>
                <b>
                    build: test large builders 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Try large runners
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 20:29:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1428" class=".btn">#1428</a>
            </td>
            <td>
                <b>
                    build: Update CI/CD workflows
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR doesn't change any code: it primarily focusses on improving the workflows used for CI/CD in this repository. A few elements can be quickly discussed and resolved, but until then it's NOT to be merged. (I'm not setting to "draft" as that disables workflow runs).

# Outstanding questions

- [ ] Should job runners be consistently set to `ubuntu-20.04` or `ubuntu-22.04`? ([`ubuntu-latest` now points to `ubuntu-22.04`](https://docs.github.com/en/actions/using-github-hosted-runners/about-github-hosted-runners#supported-runners-and-hardware-resources). There was a transition period when it could have pointed to either near end of 2022.)
- [ ] Base image for Dockerfile (same as above)
- [ ] Keep local copy of setup-node Action or ditch it? (Explained below)
- [ ] `actions/setup-libssl` seems to be adding a package designed for Ubuntu 18.04. Ideally, this should be changed to the package for Ubuntu 20.04 or Ubuntu 22.04 (depending on runner decision above).
- [ ] Use [semantic-release](https://semantic-release.gitbook.io/semantic-release/) to auto-calculate version numbers and whether to release? (See [releaserc.json definition in `@cheqd/sdk` for an example](https://github.com/cheqd/sdk/blob/main/.releaserc.json)). This uses a custom/default Convention Commit convention to auto-trigger releases.
- [ ] Proper multi-stage Docker builds

# Changelog

## Continuous Integration/Deployment workflows

- I see there's a local copy of [action/setup-node](https://github.com/actions/setup-node) which is used throughout the workflows. It's not _strictly_ necessary including the caching directives, as the default `cache` handling option itself automatically does this. Using the actual upstream `actions/setup-node@v3` ensures all upstream security updates are used in the workflow. I'm not too fussed whether a local copy is kept, but should ideally be bumped to v3 and can be simplified to use the built-in cache handling. (v2 required manual configuration.)
- Consistently made the runners ubuntu-20.04. Right now, deployment workflows use 22.04 and integration uses 20.04. This is not very relevant for NodeJS, but _can_ be relevant for libindy/ssl/pool setup 
- [`set-output` as a statement in Github Actions is deprecated, and is currently in the sunset/transition period](https://github.blog/changelog/2022-10-11-github-actions-deprecating-save-state-and-set-output-commands/). It will be fully removed on 31st May 2023. I've updated these statements to use the new recommended technique instead, otherwise, all CI/CD would start failing in May 2023.
- Added `--frozen-lockfile` to all `yarn install` statements. Otherwise, there's a non-zero chance the target dependency resolution is different than what's in `yarn.lock` and could cause divergence in the lint/build stage vs what's happening in release.
- Bumped Actions versions, where needed

## CodeQL

CodeQL requires a build to be executed to analyse security and quality issues correctly. I've added a build statement to the CodeQL workflow, and added query packs explicitly (the default is `security-extended`). I've also updated the workflow versions for security.

## Dependabot

Adds a Dependabot workflow for security and version bumps. I've [set the strategy to focus only on direct dependencies, rather than direct + devDependencies](https://docs.github.com/en/code-security/dependabot/dependabot-version-updates/configuration-options-for-the-dependabot.yml-file#allow), although this can be customised.

## New cache cleanup workflow

Github repositories have [a maximum storage of 10 GB allocated to them with 7 days worth of caching](https://docs.github.com/en/actions/using-workflows/caching-dependencies-to-speed-up-workflows#usage-limits-and-eviction-policy), beyond which entries get ejected. However, if within those 7 days the cache hits 10 GB, there's a chance that CI/CD workflows _could_ fail. I've added a workflow to evict entries from the cache every 3 days, which will make the whole repository less likely to hit the cache limit and have workflows fail. (This can also be an issue for forks.)

## Lint PR, Repo Linter

Bumped external Actions to latest versions

## Dockerfile

I'm not sure if this is used still (or perhaps for local development only), but I recommend some of the following optimisations since the built image size is approx 4.5 GB (which is pretty big):

- Combine `RUN` statements. Each RUN, COPY, ADD etc adds layers, and the Docker caching engine behaves better (i.e., will likely find more cache hits for combined statements)
- Right now, the Dockerfile isn't a true multi-stage build since the `base` target is just copied over as-is to the `final` target. This doesn't really optimise the final image size. For example, one method would be keeping `base` mostly as-is, and then using the `node:16-buster` or `node:16-buster-slim` as the base for final stage. Built artefacts from `base` can be copied over using `COPY --from=base...` syntax. This way, the larger base image with all its dependencies and fat Ubuntu image can be ditched to make a slimmer `final` image. However, I'm not exactly sure which bits need to be copied over so I couldn't execute this entirely. Can the `yarn build` be done independently, or does it require the pre-requisites?
- For the final stage image, if possible, I'd recommend using `node:16-alpine` instead. While there's more packages that need to be installed (e.g., bash is not installed of the box, it comes with`sh` only) the image sizes are dramatically lower (approx. 50-100 MB vs 4+ GB on other repos where I've implemented this).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-12 19:50:45 +0000 UTC
    </div>
</div>

