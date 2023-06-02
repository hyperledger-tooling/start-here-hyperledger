---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2253" class=".btn">#2253</a>
            </td>
            <td>
                <b>
                    1.0.0-rc2 Updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                @WadeBarnes -- advice needed.

With this PR, we update the "version.py" and "openapi" versions to "1.0.0-rc2", which I don't we want to leave in place.

Here are some things we can do:

- After this PR is merged, add another that changes the "main" branch version to what it usually is -- "0.8.1" (the last released version).  That's the state we are usually in between releases.
   - Side Issue: Should we change this practice and after a release, change the version references in the code to what we expect the next release to be -- e.g. "0.8.2-latest" or something like that.
- Merge this PR into a new branch "1.0.0" and we use that for future "1.0.0-rcX" tags.  As part of making subsequent 1.0.0-rcX tags, we merge main into the 1.0.0 branch.  That means that 1.0.0 is a clone of main for tags, updated with the types of changes that are in this PR.

I kind of lean towards the "1.0.0" branch, but you know this stuff way better than I.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-06-01 23:16:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2247" class=".btn">#2247</a>
            </td>
            <td>
                <b>
                    chore!: drop python 3.6 support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update setup.py minimum python version requirement.
Update workflows to use Python 3.9 by default.
Update container image docs.

@swcurran @WadeBarnes I believe these are the relevant changes in workflows and setup files in order to officially drop Python 3.6. I think once we've made the transition, there are a number of dependencies that ought to be updated. I think those updates are best suited to a follow up PR.

closes: #2244 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 20:01:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2246" class=".btn">#2246</a>
            </td>
            <td>
                <b>
                    Upgrade codegen tools in `scripts/generate-open-api-spec` and publish Swagger 2.0 and OpenAPI 3.0 specs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Now is as good a time as any to upgrade the codegen tools in `scripts/generate-open-api-spec` to use the latest `swaggerapi/swagger-codegen-cli` release (it was ~3 years out of date). 

Additionally, I added the latest `openapitools/openapi-generator-cli`, so that the spec generation now provides both a Swagger 2.0 spec, and an OpenApi 3.0 spec. This way users don't need to manually upgrade the spec themselves.

Previously the Swagger 2.0 spec was simply called `openapi.json`. This is now renamed `swagger.json`, with the 3.0 compatible spec in its place. 

Worth noting that the spec validation still only throws warnings that can be ignored:
- the `swagger` spec validation only complains about some missing operationId's (and 'host' not defined);
- and the `open-api` spec validation only complains about `example` fields being unexpected, and a single case of `attribute tags.tagsexternalDocs.url is missing`.

Also, I updated the `UsingOpenAPI.md` file to reflect these changes, with some minor neatening up included.

Review can be validated by running `scripts/generate-open-api-spec`.

Discussion re further edits is welcome.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-27 12:01:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2245" class=".btn">#2245</a>
            </td>
            <td>
                <b>
                    ./run_demo performance -c 1 --mediation --timing --trace-log
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bug with prompt_toolkit and trace logging. Could only bump up the prompt_toolkit library so much since demos run on Python 3.6. However, I did attempt on 3.9 with the latest version of prompt_toolkit and setting an env var (see https://github.com/prompt-toolkit/python-prompt-toolkit/pull/898). This still did not correct the issue, so reverted to existing code and just handled the exception(s). The output of the trace log is being written to the console, my limited understanding of this would be that the trace log works, but also triggers the prompt_toolkit to do the same work and gets into conflict.

Fixes #2205 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 17:21:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2243" class=".btn">#2243</a>
            </td>
            <td>
                <b>
                    fix: route multitenant connectionless oob invitation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This addresses an issue where the keys used in connectionless oob invitations were not correctly set-up for routing through the base wallet when multi-tenancy is enabled, which resulted in those invitation not being usable.

cc @lohanspies @ff137


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-05-26 12:49:04 +0000 UTC
    </div>
</div>

