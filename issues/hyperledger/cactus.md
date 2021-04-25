---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/717" class=".btn">717</a>
            </td>
            <td>
                <b>
                    feat(ci): support debugging on CI server through ssh
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">Nice-to-Have</span><span class="chip">documentation</span><span class="chip">enhancement</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span>
            </td>
            <td>
                ### Description
As a contributor I want to be able to debug the failing tests on the CI server directly so that I can figure out what is going wrong even if my tests are only failing on the CI server and not on my local machine (which is a very common scenario at present...)

Use this (?) => https://github.com/marketplace/actions/debugging-with-ssh

### Acceptance Criteria
1. Works out of the box with VSCode debugger (preferably, but other is acceptable too)
2. GIF tutorial in CONTRIBUTING.md showing exactly how it's done in 30 seconds or less.

cc: @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo @jagpreetsinghsasan
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-03-24 05:33:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/662" class=".btn">662</a>
            </td>
            <td>
                <b>
                    refactor: obtain output from TSC repo linter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Developer_Experience</span><span class="chip">Hacktoberfest</span><span class="chip">Nice-to-Have</span><span class="chip">Triage_Needed</span><span class="chip">enhancement</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span>
            </td>
            <td>
                ### Description

We need to get going with adopting the TSC repo structure recommendations where applicable and/or send PRs to the default config file (rule set parameter) where that's more suiting. 

### Acceptance Criteria
1. Run the tool against the `main` branch of the repository
2. Post the output here, whatever it may be
3. Initiated discussion on which errors/warnings can we fix and which ones we'd like to squash by updating the repo linter rule set instead.
4. Created follow-up tasks for addressing each item as discussed during `3)`

### For Context the original email

> Hi all,
> 
> The TSC decided to recommend that all Hyperledger projects adopt a common repository structure to provide some consistency across projects and make it easier for people to find their way around and quickly locate important information. In order to help implement it the TSC then decided to leverage the TODO group repolinter tool.
> 
> A customized configuration file has been developed for Hyperledger and I'd like to invite all the projects to try and use it.
> 
> Contrary to what was first thought, we do not want every project to copy that file into their own repos. This is bound to create a maintenance nightmare. So, instead, we'd like to try and use the same common config file.
> 
> After installing repolinter you can check your repository with the following command from the root directory of your repo:
> 
> repolinter --rulesetUrl https://github.com/hyperledger-labs/hyperledger-community-management-tools/raw/main/repo_structure/repolint.json
> 
> It is understood that the config file may not work well for all projects. We welcome contribution on how to improve it. All PRs welcome. :-) Just keep in mind that the goal is to make the file work for everyone so don't simply remove stuff that's not relevant to your repo. Some errors can simply be ignored.
> 
> Finally, whether this should be integrated in your CI is up to you. As a first step it may be enough to give it a run every now and then.
> 
> Please, let us know how your experiment goes. We're interested in both good and bad stories!

cc: @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo @lehors 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-03-12 18:50:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/647" class=".btn">647</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): plugin import - asn1 illegal padding
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">bug</span><span class="chip">dependencies</span><span class="chip">help wanted</span>
            </td>
            <td>
                **Describe the bug**

A quite strange flake. 3 out of the 4 CI runs succeeded for my PR but this one failed with the error mentioned in the subject while executing the test at `./packages/cactus-cmd-api-server/src/test/typescript/integration/runtime-plugin-imports.test.ts`

**To Reproduce**

Not sure, could be some race condition internal to NodeJS itself. I doubt we'll be able to reproduce it to be honest.

**Expected behavior**

Test does not fail.

**Logs/Stack traces**

https://github.com/petermetz/cactus/runs/2071676202?check_suite_focus=true#step:10:179

```sh
  
ok 4 - packages/cactus-cmd-api-server/src/test/typescript/integration/remote-plugin-imports.test.ts # time=27952.046ms

# Subtest: packages/cactus-cmd-api-server/src/test/typescript/integration/runtime-plugin-imports.test.ts
    # can import plugins at runtime (CLI)
    Warning: configuration param 'type' not declared in the schema
    [2021-03-10T02:03:56.784Z] INFO (config-service): Configuration validation OK.
    not ok 1 Error: error:0D0E20DD:asn1 encoding routines:c2i_ibuf:illegal padding
      ---
        operator: error
        at: bound (/home/runner/work/cactus/cactus/node_modules/onetime/index.js:30:12)
        stack: |-
          Error: error:0D0E20DD:asn1 encoding routines:c2i_ibuf:illegal padding
              at Object.createSecureContext (_tls_common.js:129:17)
              at Server.setSecureContext (_tls_wrap.js:1323:27)
              at Server (_tls_wrap.js:1181:8)
              at new Server (https.js:66:14)
              at Object.createServer (https.js:91:10)
              at new ApiServer (/home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/main/typescript/api-server.ts:1:25253)
              at /home/runner/work/cactus/cactus/packages/cactus-cmd-api-server/src/test/typescript/integration/runtime-plugin-imports.test.ts:34:21
              at Test.<anonymous> (/home/runner/work/cactus/cactus/node_modules/tape-promise/index.compiled.js:86:19)
              at Test.bound [as _cb] (/home/runner/work/cactus/cactus/node_modules/tape/lib/test.js:84:32)
              at Test.run (/home/runner/work/cactus/cactus/node_modules/tape/lib/test.js:101:31)
      ...
    
    Bail out! Error: error:0D0E20DD:asn1 encoding routines:c2i_ibuf:illegal padding
Bail out! Error: error:0D0E20DD:asn1 encoding routines:c2i_ibuf:illegal padding
----------------------------------------------------------------------------------------|----------|----------|----------|----------|-------------------|
File                                                                                    |  % Stmts | % Branch |  % Funcs |  % Lines | Uncovered Line #s |
----------------------------------------------------------------------------------------|----------|----------|----------|----------|-------------------|
All files                                                                               |    38.28 |    21.51 |    25.44 |    37.96 |                   |
 cactus-api-client/src/main/typescript                                                  |    44.26 |    33.33 |    45.45 |    42.37 |                   |
  api-client.ts                                                                         |       20 |        0 |        0 |       20 |... 29,131,133,137 |
  default-consortium-provider.ts                                                        |    61.54 |       60 |       75 |    61.54 |... 47,50,52,59,65 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  public-api.ts                                                                         |      100 |      100 |      100 |      100 |                   |
 cactus-cmd-api-server/src/main/typescript                                              |    81.22 |    46.15 |    65.52 |    81.77 |                   |
  api-server.ts                                                                         |    80.32 |    46.15 |       68 |    81.08 |... 72,373,375,377 |
  public-api.ts                                                                         |      100 |      100 |       50 |      100 |                   |
 cactus-cmd-api-server/src/main/typescript/cmd                                          |    29.17 |       25 |        0 |    29.17 |                   |
  cactus-api.ts                                                                         |    29.17 |       25 |        0 |    29.17 |... 32,33,35,36,41 |
 cactus-cmd-api-server/src/main/typescript/config                                       |    83.48 |    39.39 |    81.25 |    83.48 |                   |
  config-service.ts                                                                     |    85.33 |    47.83 |    83.33 |    85.33 |... 54,512,513,543 |
  convict-plugin-array-format.ts                                                        |       70 |    16.67 |       50 |       70 |           5,16,17 |
  self-signed-pki-generator.ts                                                          |    83.33 |       25 |      100 |    83.33 |    38,39,41,43,44 |
 cactus-cmd-api-server/src/main/typescript/generated/openapi/typescript-axios           |    25.45 |        0 |        0 |    26.92 |                   |
  api.ts                                                                                |    18.18 |        0 |        0 |    19.35 |... 46,157,165,185 |
  base.ts                                                                               |    38.46 |        0 |        0 |    41.67 |... 54,55,67,68,69 |
  configuration.ts                                                                      |    14.29 |        0 |        0 |    14.29 | 69,70,71,72,73,74 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
 cactus-common/src/main/typescript                                                      |     34.9 |    15.58 |    31.25 |    31.43 |                   |
  bools.ts                                                                              |       50 |        0 |        0 |       50 |                13 |
  checks.ts                                                                             |       50 |       60 |      100 |       50 |       17,18,36,37 |
  coded-error.ts                                                                        |       20 |        0 |        0 |       25 |            7,8,12 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  js-object-signer.ts                                                                   |    16.13 |        0 |        0 |    16.13 |... 99,100,101,102 |
  key-converter.ts                                                                      |    12.24 |     7.69 |    14.29 |     12.5 |... 18,121,124,125 |
  objects.ts                                                                            |     6.25 |        0 |        0 |     6.67 |... 57,58,59,60,63 |
  public-api.ts                                                                         |      100 |      100 |    27.27 |      100 |                   |
  secp256k1-keys.ts                                                                     |    42.86 |      100 |        0 |    42.86 |       17,18,22,24 |
  servers.ts                                                                            |    44.19 |    33.33 |    58.33 |       45 |... 70,92,93,96,98 |
  strings.ts                                                                            |    42.86 |        0 |    33.33 |    42.86 |       13,17,18,19 |
 cactus-common/src/main/typescript/logging                                              |    87.88 |    63.64 |    71.43 |    87.88 |                   |
  logger-provider.ts                                                                    |      100 |    71.43 |      100 |      100 |             10,27 |
  logger.ts                                                                             |    78.95 |       50 |    63.64 |    78.95 |       46,54,60,63 |
 cactus-core-api/src/main/typescript                                                    |      100 |      100 |       75 |      100 |                   |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  public-api.ts                                                                         |      100 |      100 |       75 |      100 |                   |
 cactus-core-api/src/main/typescript/generated/openapi/typescript-axios                 |    63.16 |    46.15 |       50 |    64.86 |                   |
  api.ts                                                                                |      100 |      100 |      100 |      100 |                   |
  base.ts                                                                               |    38.46 |        0 |        0 |    41.67 |... 54,55,67,68,69 |
  configuration.ts                                                                      |    14.29 |        0 |        0 |    14.29 | 69,70,71,72,73,74 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
 cactus-core-api/src/main/typescript/plugin                                             |      100 |    83.33 |      100 |      100 |                   |
  i-cactus-plugin.ts                                                                    |      100 |       75 |      100 |      100 |                85 |
  plugin-aspect.ts                                                                      |      100 |      100 |      100 |      100 |                   |
  plugin-factory.ts                                                                     |      100 |      100 |      100 |      100 |                   |
 cactus-core-api/src/main/typescript/plugin/web-service                                 |      100 |      100 |      100 |      100 |                   |
  i-plugin-web-service.ts                                                               |      100 |      100 |      100 |      100 |                   |
 cactus-core/src/main/typescript                                                        |    38.96 |    38.46 |    19.35 |    38.89 |                   |
  consortium-repository.ts                                                              |    15.79 |        0 |        0 |    16.67 |... 44,48,59,60,62 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  plugin-registry.ts                                                                    |    39.22 |    41.67 |    22.73 |    40.82 |... 22,127,132,136 |
  public-api.ts                                                                         |      100 |      100 |    33.33 |      100 |                   |
 cactus-core/src/main/typescript/web-services                                           |    11.11 |      100 |        0 |    11.11 |                   |
  register-web-service-endpoint.ts                                                      |    11.11 |      100 |        0 |    11.11 |... 18,20,21,22,24 |
 cactus-plugin-consortium-manual/src/main/typescript                                    |    30.86 |        0 |        0 |       30 |                   |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  plugin-consortium-manual.ts                                                           |    15.63 |        0 |        0 |    15.63 |... 37,141,145,149 |
  plugin-factory-consortium-manual.ts                                                   |       75 |      100 |        0 |       75 |                18 |
  public-api.ts                                                                         |    91.67 |      100 |        0 |    90.91 |                27 |
 cactus-plugin-consortium-manual/src/main/typescript/consortium                         |    13.19 |        0 |        0 |    13.33 |                   |
  get-consortium-jws-endpoint-v1.ts                                                     |    10.42 |        0 |        0 |    10.64 |... 13,114,115,116 |
  get-node-jws-endpoint-v1.ts                                                           |    16.28 |        0 |        0 |    16.28 |... 00,101,107,109 |
 cactus-plugin-consortium-manual/src/main/typescript/generated/openapi/typescript-axios |     51.9 |       36 |       40 |     52.7 |                   |
  api.ts                                                                                |    49.12 |    27.78 |    41.18 |    50.94 |... 14,222,231,262 |
  base.ts                                                                               |    76.92 |    66.67 |       50 |       75 |          67,68,69 |
  configuration.ts                                                                      |    14.29 |        0 |        0 |    14.29 | 69,70,71,72,73,74 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
 cactus-plugin-keychain-vault/src/main/typescript                                       |    50.86 |    22.22 |    20.59 |    50.43 |                   |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  plugin-factory-keychain.ts                                                            |    89.47 |    33.33 |      100 |    89.47 |             33,45 |
  plugin-keychain-vault-remote-adapter.ts                                               |     64.1 |       50 |    33.33 |     64.1 |... 27,134,138,146 |
  plugin-keychain-vault.ts                                                              |    16.33 |        0 |        0 |    16.33 |... 48,149,153,157 |
  public-api.ts                                                                         |      100 |      100 |    33.33 |      100 |                   |
 cactus-plugin-keychain-vault/src/main/typescript/generated/openapi/typescript-axios    |    77.53 |    48.98 |       65 |    78.57 |                   |
  api.ts                                                                                |    83.58 |    47.62 |    70.59 |    85.71 |... 70,228,237,247 |
  base.ts                                                                               |    76.92 |    66.67 |       50 |       75 |          67,68,69 |
  configuration.ts                                                                      |    14.29 |        0 |        0 |    14.29 | 69,70,71,72,73,74 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
 cactus-plugin-keychain-vault/src/main/typescript/web-services                          |    27.78 |        0 |        0 |    27.78 |                   |
  get-keychain-entry-endpoint-v1.ts                                                     |    27.78 |        0 |        0 |    27.78 |... 46,47,51,55,59 |
  set-keychain-entry-endpoint-v1.ts                                                     |    27.78 |        0 |        0 |    27.78 |... 46,47,51,55,59 |
 cactus-test-tooling/src/main/typescript                                                |    97.87 |        0 |    15.63 |    97.73 |                   |
  i-key-pair.ts                                                                         |       50 |        0 |        0 |       50 |                 9 |
  index.ts                                                                              |      100 |      100 |      100 |      100 |                   |
  public-api.ts                                                                         |      100 |      100 |    16.13 |      100 |                   |
 cactus-test-tooling/src/main/typescript/besu                                           |      6.8 |        0 |        0 |     6.94 |                   |
  besu-test-ledger.ts                                                                   |      6.8 |        0 |        0 |     6.94 |... 48,358,368,369 |
 cactus-test-tooling/src/main/typescript/cactus-keychain-vault-server                   |    85.11 |    68.75 |      100 |    85.11 |                   |
  cactus-keychain-vault-server.ts                                                       |    85.11 |    68.75 |      100 |    85.11 |... 06,121,122,135 |
 cactus-test-tooling/src/main/typescript/common                                         |    28.13 |    23.08 |    29.17 |    27.13 |                   |
  containers.ts                                                                         |    32.12 |    27.91 |    36.84 |    31.06 |... 92,394,395,397 |
  streams.ts                                                                            |      3.7 |        0 |        0 |      3.7 |... 65,66,68,74,75 |
 cactus-test-tooling/src/main/typescript/corda                                          |     9.15 |        0 |        0 |     9.27 |                   |
  corda-test-ledger.ts                                                                  |     8.55 |        0 |        0 |     8.67 |... 82,383,395,396 |
  sample-cordapp-enum.ts                                                                |      100 |      100 |      100 |      100 |                   |
 cactus-test-tooling/src/main/typescript/corda-connector                                |     12.5 |        0 |        0 |    12.66 |                   |
  corda-connector-container.ts                                                          |     12.5 |        0 |        0 |    12.66 |... 13,214,223,224 |
 cactus-test-tooling/src/main/typescript/fabric                                         |     7.07 |        0 |        0 |     7.14 |                   |
  fabric-test-ledger-v1.ts                                                              |     7.07 |        0 |        0 |     7.14 |... 04,505,515,516 |
 cactus-test-tooling/src/main/typescript/http-echo                                      |        8 |        0 |        0 |     8.25 |                   |
  http-echo-container.ts                                                                |        8 |        0 |        0 |     8.25 |... 23,233,242,243 |
 cactus-test-tooling/src/main/typescript/quorum                                         |     6.99 |        0 |        0 |     7.14 |                   |
  quorum-test-ledger.ts                                                                 |     6.99 |        0 |        0 |     7.14 |... 53,363,372,373 |
 cactus-test-tooling/src/main/typescript/vault-test-server                              |    82.69 |       75 |    91.67 |    82.69 |                   |
  vault-test-server.ts                                                                  |    82.69 |       75 |    91.67 |    82.69 |... 28,143,144,154 |
----------------------------------------------------------------------------------------|----------|----------|----------|----------|-------------------|
npm ERR! code ELIFECYCLE
npm ERR! errno 1
npm ERR! @hyperledger/cactus@ test:integration: `tap --node-arg=--max-old-space-size=4096 --jobs=1 --timeout=600 "packages/cactus-*/src/test/typescript/integration/" "--bail"`
npm ERR! Exit status 1
npm ERR! 
npm ERR! Failed at the @hyperledger/cactus@ test:integration script.
npm ERR! This is probably not a problem with npm. There is likely additional logging output above.

npm ERR! A complete log of this run can be found in:
npm ERR!     /home/runner/.npm/_logs/2021-03-10T02_03_57_146Z-debug.log
```

**Screenshots**

If applicable, add screenshots to help explain your problem.

**Cloud provider or hardware configuration:**
Are you running the software on a dev machine or somewhere in the cloud?

**Operating system name, version, build:**

Ubuntu 20.04 LTS

**Hyperledger Cactus release version or commit (git rev-parse --short HEAD):**

`main`

**Hyperledger Cactus Plugins/Connectors Used**

 `N/A`

**Additional context**

This came out during the development of the Fabric contract deployment endpoint, but this fact is suspected to be a coincidence and that the issue itself has nothing to do with the Fabric connector or its tests.

cc: @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-03-10 04:51:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/597" class=".btn">597</a>
            </td>
            <td>
                <b>
                    feat: rosetta API compatibility
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Core_API</span><span class="chip">Developer_Experience</span><span class="chip">Epic</span><span class="chip">SPIKE</span><span class="chip">enhancement</span><span class="chip">help wanted</span>
            </td>
            <td>
                ### Description

We could have our ledger plugins implement the rosetta spec either by themselves or by way of adding new plugins dedicated to rosetta (unclear as of the time of this writing which one is more suitable).

Should be very easy to get started since Rosetta also uses OpenAPI 3 to describe the APIs. 

https://www.rosetta-api.org/
https://github.com/coinbase/rosetta-specifications

### Acceptance Criteria
1. At least one of our ledger plugins understands Rosetta formatted requests.

cc: @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo @mwklein
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-02-23 18:22:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/546" class=".btn">546</a>
            </td>
            <td>
                <b>
                    feat: design authz/authn
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">API_Server</span><span class="chip">Core_API</span><span class="chip">SPIKE</span><span class="chip">Security</span><span class="chip">Significant_Change</span><span class="chip">help wanted</span>
            </td>
            <td>
                ### Description

We already have an issue and a corresponding branch for OpenID connect which is the right start, but there has to be some more detailed plans made about how the authentication and authorization will look like especially in deployments where each plugin is running in it's own container.

There's a lot of angles to consider, some are more exotic that do not come up during "traditional" system design such as how does the authnz play with the consortium members? Do we want node-local storage? (most likely yes)


### Acceptance Criteria
1. An actionable design document dedicated to authnz
2. Output of 1) must be actionable for actual implementation
3. Horizontal scalability is not hindered by the authzn design once implemented

cc: @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-02-05 02:39:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/544" class=".btn">544</a>
            </td>
            <td>
                <b>
                    chore: security audit for 1.0 release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Security</span><span class="chip">help wanted</span>
            </td>
            <td>
                ### Description
As a maintainer, I want to make sure that someone other than the current set of maintainers/core contributors have taken a detailed look into the code and concluded that it contains no obvious security holes/vulnerabilities.
The idea is to have someone perform a security audit to act as a sort of peer review. This is to reduce the risk of us releasing a 1.0 GA with severe vulnerabilities baked into it (still very possible, but this issue is about going the extra mile, not about eliminating the possibility entirely, which is anyway impossible).

### Acceptance Criteria
1. The person or organization who performed the audit is willing to put it in writing that according to their findings there are no known security vulnerabilities (if they do find anything obviously we'll fix that prior to 1.0 GA)

cc: @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-02-05 01:52:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/cactus/issues/540" class=".btn">540</a>
            </td>
            <td>
                <b>
                    docs(examples): add carbon-account-app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">Fabric</span><span class="chip">GFI_Climate_Action_SIG</span><span class="chip">Hacktoberfest</span><span class="chip">documentation</span><span class="chip">good-first-issue</span><span class="chip">help wanted</span>
            </td>
            <td>
                ### Description

It would be great for us to help out the Climate Action SIG with the important work that they are doing and at the same time expose ourselves (our designs) to real-world problems/use cases that developers will use Cactus to solve.
The idea here is to have a full-fledged example application doing the same thing that's being done in the pre-existing codebase that Si Chen demoed to us during the maintainer's call on the 19th of January in the year 2021 [1] and based on the additional information provided later via emails: [2], [3]

https://docs.google.com/document/d/1jiPaEoa-lBwn5_w4HVj1_ItdUV-DkFU93guSTMqtOu8/edit?ts=601c8205

[1] 2021-01-19 Meeting Notes: https://wiki.hyperledger.org/display/cactus/2021-01-19+Meeting+Notes


[2] [Hyperledger Cactus] Using Cactus to connect Fabric and Besu: https://lists.hyperledger.org/g/cactus/message/204?p=,,,100,0,0,0::relevance,,si+chen,100,2,0,78464157

[3] testing the Climate SIG Fabric-Ethereum connection: https://lists.hyperledger.org/g/cactus/message/217?p=,,,100,0,0,0::Created,,,100,2,0,80392158

[4] https://wiki.hyperledger.org/display/CASIG/Emissions+Tokens+Network

[5] http://emissionstokens.opentaps.org/

### Acceptance Criteria

1. Example is end to end and containerized so that we discover issues that a developer would face who actually has to deliver a working application not just some partial demo/PoC
2. Changes that were necessary (if any, likely many) to Cactus while developing the example are broken into separate commits and submitted as independent pull requests prior to submitting the final PR containing the example itself. This will provide us with a chance to review changes in the core and review those independently from the examples itself (of which the review should be much simpler/straightforward since it's just an example not something that changes actual Cactus packages)
3. Solution should be approved by the CA SIG as something that appears to be usable by them (doesn't need to actually replace their existing implementation but that would be the absolute best of course)
4. A set of good first issues are defined that are all specific to the CA SIG work of ours 

cc: @opentaps @takeutak @sfuji822 @hartm @jonathan-m-hamilton @AzaharaC @jordigiam @kikoncuo
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-02-04 22:33:51 +0000 UTC
    </div>
</div>

