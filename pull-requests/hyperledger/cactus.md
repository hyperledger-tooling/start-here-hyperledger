---
layout: default
title: cactus
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cactus
---

# cactus <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cactus){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/870" class=".btn">#870</a>
            </td>
            <td>
                <b>
                    docs(meta): guidelnies for documentation authors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 22:46:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/867" class=".btn">#867</a>
            </td>
            <td>
                <b>
                    docs(vscode): added extensions.json file with recommended extensions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>

**Added**

- extensions.json file within the .vscode directory

**Updated**

- .gitignore file to allow extensions.json to be pushed to the repo

Resolve #863  
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 12:06:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/865" class=".btn">#865</a>
            </td>
            <td>
                <b>
                    feat(corda): prometheus exporter metrics integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
---	

feat(corda): prometheus exporter metrics integration
	
	Primary Change
	1. The corda ledger connector plugin now includes the prometheus metrics exporter integration
	2. OpenAPI spec now has api endpoint for getting the prometheus metrics

	Refactorings that were also necessary to incorporate 1) and 2)
	3. GetPrometheusMetricsV1 class is created to handle the corresponding api endpoint
	4. IPluginLedgerConnectorCordaOptions interface in PluginLedgerConnectorCorda class now has a prometheusExporter object optional field
	5. The PluginLedgerConnectorCorda class has relevant functions to incorporate prometheus exporter
	6. Updated Readme.md about the prometheus exporter
	7. Updated the test case located at packages/cactus-plugin-ledger-connector-corda/src/test/typescript/integration/deploy-cordapp-jars-to-nodes.test.ts
	8. Updated the OpenAPI spec file to have run-transaction endpoint which currently returns NOT_IMPLEMENTED with 501 code.

Resolve #535

Signed-off-by: Jagpreet Singh Sasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 09:37:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/864" class=".btn">#864</a>
            </td>
            <td>
                <b>
                    test(ci): fail ci.sh if git index is not empty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                the script uses npm ci, which should not cause
any updates to the lock files, therefor currently
the git index is checked only at the end of the
script

Resolves https://github.com/hyperledger/cactus/issues/809

Signed-off-by: Hristiyan Ivanov <hristiyan.d.ivanov@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 06:18:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/861" class=".btn">#861</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): enrollAdmin() and createCaClient()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                ## Dependencies

Depends on #841

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Date: Sat Apr 24 2021 20:55:46 GMT-0700 (Pacific Daylight Time) 

feat(connector-fabric): enrollAdmin() and createCaClient()

These are methods that come in handy while working with
Fabric networks.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-25 03:58:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/856" class=".btn">#856</a>
            </td>
            <td>
                <b>
                    docs(examples): add carbon-account-app #540
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">Xdai</span><span class="chip">dependent</span><span class="chip">documentation</span>
            </td>
            <td>
                ## Dependencies

Depends on https://github.com/hyperledger/cactus/pull/861
Depends on https://github.com/hyperledger/cactus/pull/855
Depends on https://github.com/hyperledger/cactus/pull/854
Depends on https://github.com/hyperledger/cactus/pull/841

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: Fri Apr 23 2021 15:00:07 GMT-0700 (Pacific Daylight Time)
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: Fri Apr 23 2021 21:02:19 GMT-0700 (Pacific Daylight Time) 

docs(examples): add carbon-account-app #540

Fixes #540

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-24 04:10:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/855" class=".btn">#855</a>
            </td>
            <td>
                <b>
                    feat(connector-xdai): add ledger connector plugin for xdai #852
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Xdai</span><span class="chip">dependent</span><span class="chip">enhancement</span>
            </td>
            <td>
                ## Dependencies

Depends on #854

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: 2021-04-23 14:47:01 -0700
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: 2021-04-23 14:53:42 -0700 

feat(connector-xdai): add ledger connector plugin for xdai #852

A 1 to 1 clone of the besu connector for now but I thought it best
to keep it separate regardless because a lot of Besu specific
changes are about to drop for the Besu connector as we add the
differentiating features of it to the connector as well and
once that happens the codebases will probably look quite
different at that point.

Fixes #852

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 21:55:08 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/854" class=".btn">#854</a>
            </td>
            <td>
                <b>
                    feat(test-tooling): add OpenEthereumTestLedger #851
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Xdai</span>
            </td>
            <td>
                We did not need to roll our own contanier image for this
so the only thing new here is the class in the test tooling
package that makes it convenient to write test cases against
OpenEthereum. The container image used by the class behind
the scenes is just the stock OpenEthereum image from DockerHub.

Fixes #851

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 21:48:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/849" class=".btn">#849</a>
            </td>
            <td>
                <b>
                    fix(ci): dependent issues bot workflow has no job id #848
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span>
            </td>
            <td>
                There's a mismatch in what you have set as the name of the required status check for the main branch (Dependabot Issues) and what the check is actually called when the workflow runs (check)

https://github.com/hyperledger/cactus/actions/runs/772009240/workflow

```yaml
jobs:
  check:
    runs-on: ubuntu-latest
---
```

You can rename the job in that workflow to Dependabot Issues to match the required status check name:

```yaml
jobs:
  check:
    runs-on: ubuntu-latest
    name: Dependabot Issues
----
```
https://docs.github.com/en/actions/reference/workflow-syntax-for-github-actions#jobsjob_idname

The check will then be displayed as Dependabot Issues - if this was the intended name - and will satisfy the protected branches rule.

Fixes #848

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 16:48:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/846" class=".btn">#846</a>
            </td>
            <td>
                <b>
                    docs(readthedocsio): add packages readme files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                Resolve #340 
Depends on #827 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 12:31:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/845" class=".btn">#845</a>
            </td>
            <td>
                <b>
                    feat: incorporating load testing into our CI pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Performance</span>
            </td>
            <td>
                This changes utilizes Artillery to load test our API endpoint. This is a first cut implementation.

BREAKING CHANGE: 🧨 Behaviors in a cloud environment is currently untested and could impact
CI pipeline.


Artillery works by sending HTTP requests at different intervals as defined in [benchmark-script.yaml](https://github.com/hyperledger/cactus/pull/845/files#diff-db633280d17272defd50724836cb82a91e5a6e23f040d8e261c5eb75a5d53382).

I've defined 3 phases, a warm up phase, a ramp up phase, and finally a phase imitating a sustained high load.

We can further define different scenarios, target endpoints, and user actions.

After running the test, Artillery produces a report in json format, which is read back in to pull out the metrics we need. We can then define a threshold, and write an assert to ensure we're meeting that requirement.

✅ Closes: #295

Signed-off-by: Travis Payne <travis.payne@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 09:10:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/844" class=".btn">#844</a>
            </td>
            <td>
                <b>
                    build(lerna): canary publish script dist-tag = current git branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Primary change:
=============

Fixes #850 

The npm dist-tag parameter will now be set to whatever is the
current git branch checked out.

This allows for developers to work on their own feature branches
and publish their own canary releases
for every single commit as they see fit without having to wait for the
an upcoming official release.

Miscellaneous change:

The script will now make sure to run the CI script prior to issuing the
canary release so that it is guaranteed
that the canary release does not go
out unless it was made from a revision
of the code that has the tests and build passing.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 03:07:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/843" class=".btn">#843</a>
            </td>
            <td>
                <b>
                    fix(connector-besu): network update only if present in keychain
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Besu</span><span class="chip">bug</span>
            </td>
            <td>
                Only attempt to set/update the networks object on the contract JSON if
it was present in the keychain, leave it alone
otherwise.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 03:04:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/842" class=".btn">#842</a>
            </td>
            <td>
                <b>
                    docs(examples): fix supply chain app process.env authorization protocol
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">bug</span><span class="chip">documentation</span>
            </td>
            <td>
                The AUTHORIZATION_PROTOCOL=NONE
configuration parameter had to be specified because without it the config-
service bails out.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 03:00:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/841" class=".btn">#841</a>
            </td>
            <td>
                <b>
                    feat(connector-fabric): contract deployment Fabric 2.x
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependencies</span>
            </td>
            <td>
                Primary change:
--------------

Add support for deploying contracts to Fabric 2.x ledgers
Languages supported (and covered by tests):
- golang
- javascript
- typescript

It is assumed that the server that is running the Fabric
ledger containers have the required dependencies to build
the contracts.
In the case of the tests this is provided by the Cactus
Fabric All-In-One container image which has NodeJS and Go
installed on it.

Secondary change(s):
-------------------

Breaking API change: renamed the contract deployment endpoint
that supports Fabric 1.4.x so that:
- the default implementation of it now assumes Fabric 2.x
- there is still a compatible version of the endpoint for 1.4.x

Fixes #654

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

cc: @RafaelAPB 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-23 02:30:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/838" class=".btn">#838</a>
            </td>
            <td>
                <b>
                    docs: adding devcontainer docker file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: TonyRowntree <33454202+TonyRowntree@users.noreply.github.com>

**Added:**

- Devcontainer docker file

Resolve #504 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-22 12:54:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/830" class=".btn">#830</a>
            </td>
            <td>
                <b>
                    docs(contributing): add Reload VSCode Window After Adding Dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                New section to explain that after lerna add, sometimes it might be
necessary to reload VSCode for it to pick up the Typescript definitions
of the newly added dependency.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 14:19:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/829" class=".btn">#829</a>
            </td>
            <td>
                <b>
                    feat(fabric): add sequence diagram of run transaction endpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Commit to be reviewed
----------------------------------
feat(fabric): add sequence diagram of run transaction endpoint	
	
	Primary Change
	--------------

	1. Added plantuml diagrams and corresponding pngs to describe the run transaction endpoint and are located under cactus-plugin-ledger-connector-fabric/docs/architecture
	2. Modified the Readme to incorporate the pngs created above.

Resolve #756

Signed-off-by: Jagpreet Singh Sasan <jagpreet.singh.sasan@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 10:07:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/828" class=".btn">#828</a>
            </td>
            <td>
                <b>
                    feat(tools): fabric all-in-one 2.x add nodejs to image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Fabric</span><span class="chip">dependencies</span>
            </td>
            <td>
                ## Dependencies

Depends on #826 

## Commit to review

Author: Peter Somogyvari <peter.somogyvari@accenture.com>
Author Date: Tue Apr 20 2021 23:20:06 GMT-0700 (Pacific Daylight Time)
Committer: Peter Somogyvari <peter.somogyvari@accenture.com>
Committer Date: Tue Apr 20 2021 23:24:44 GMT-0700 (Pacific Daylight Time) 

feat(tools): fabric all-in-one 2.x add nodejs to image

This is necessary so that the AIO image can compile Typescript
contracts down into Javascript for the NodeJS
chaincode runtime.

Tagged on DockerHub as
hyperledger/cactus-fabric2-all-in-one:2021-04-20-nodejs

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-21 06:29:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cactus/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    docs(readthedocs): readthedocs documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolve #221 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-20 10:00:54 +0000 UTC
    </div>
</div>

