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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/1427" class=".btn">#1427</a>
            </td>
            <td>
                <b>
                    feat(anoncreds): issue revocable credentials
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR includes some initial work done for supporting the issuance of revocable AnonCreds credentials in AFJ. 

**Brief summary of the changes:**

- Update of `AnonCredsRegistry` and `AnonCredsIssuerService` interfaces to add registration of revocation registry definitions and revocation status lists 
- AnonCreds module, through its `AnonCredsApi`, now allows to register these objects and update revocation status lists
- `AnonCredsCredentialFormatService` has been updated to handle accept revocable credential requests, retrieving an active Revocation Registry Definition and assigning an index to the credential that is going to be issued (this logic is not completely done yet though)
- Credentials module allows to send revocation notification for both `indy-anoncreds` and a potentially new `anoncreds` revocation format. This is very basic right now and needs some more work to support future formats and get information directly from the credential record to be more aligned with other modules API.
- AnonCreds module now has some new configuration items for object creation. In particular it adds the new `TailsFileService`, which is an interface for downloading and uploading tails files. The default implementation works as right now (only allows to download files), while a custom one can be used to upload files to any chosen tails server. In `samples` directory there is an example of tails server and service interface (not sure if they belong there but for the moment didn't find a better place). For the tests there is a dummy implementation that allows us to run them without the need of having an actual HTTP server

**Flow:**

For the moment, as seen in the few tests added in anoncreds-rs package, all VDR objects are managed exclusively from AnonCreds API and created/registered separately in order to have a simpler state management. For instance, if we want to create a revocable credential definition, we'd need to call:
- registerSchema
- registerCredentialDefinition
- registerRevocationRegistryDefinition
- registerRevocationStatusList

The only step that does two actions atomically is `registerRevocationRegistryDefinition`, as it will attempt to successfully uploading the tails file before registering the object in the VDR (this is mandatory because we may not know upfront what's the publicly available tails location).

To revoke a credential (or a number of credentials), `AnonCredsApi.updateRevocationStatusList()` must be called using the revocation registry definition id and credential indexes as an input.  If we want to notify the holder/s about this revocation, we must use Credentials API afterwards.

**Some notes/missing pieces**

- In this PR there is only a generic implementation using `InMemoryAnonCredsRegistry`. There is not yet any implementation for Indy VDR or Indy SDK
- It could feel more 'natural ' if we add a method called `revokeCredentials` in `CredentialsApi` that does both the revocation state update and send notification. However, this integration would need us to deal with the different credential formats and, after all, I'm not sure if it will be really useful in real world scenarios, because I think that usually an issuer would prefer to revoke multiple credentials at once (to avoid creating lots of ledger updates)
- In terms of agent storage, there are no specific changes to mark credentials as revoked and to store more information about credential revocation identification from the issuer side. I think it could be useful to find a good place to do so within AFJ model
- For the moment it depends on some fixes in anoncreds-rs (https://github.com/hyperledger/anoncreds-rs/pull/186, https://github.com/hyperledger/anoncreds-rs/pull/188 and probably something else with the timestamps that I'll need to debug more).
- Sorry for the monster PR!


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-11 22:51:00 +0000 UTC
    </div>
</div>

