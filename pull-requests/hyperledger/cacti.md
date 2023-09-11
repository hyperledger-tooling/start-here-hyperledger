---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2681" class=".btn">#2681</a>
            </td>
            <td>
                <b>
                    build(codegen): fix URL of OpenAPI generator jar v6.6.0 not 6.3.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [skip ci]

Fixes #2680

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 18:14:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2673" class=".btn">#2673</a>
            </td>
            <td>
                <b>
                    test(cmd-api-server): fix CVE-2023-37903 - vm2 Sandbox Escape vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                There is no fix for the vm2 package's vulnerability and it is also no longer
maintained so a fix is not coming either.
Based on this and the fact that artillery's newer updates also did not
move away from using vm2 (as a transitive dependency) it is best to
just delete the artillery based benchmark for now. The longer term
and more robust solution is probably to have JMeter tests defined.
The downside of this is that it is harder to maintain them because
it's not NodeJS/Typescript technology stack but we already suffer
from this due to needing the JVM for Corda development tasks
therefore it is not as big of an overhead as it seems.

https://github.com/hyperledger/cacti/issues/2672

Fixes #2671

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 05:21:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2670" class=".btn">#2670</a>
            </td>
            <td>
                <b>
                    docs(examples): fix Mongoose Prototype Pollution vulnerability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Both mongoose and the mongodb NodeJS driver dependency appeared to be
completely unused so instead of upgrading I just removed them.

Fixes #2669

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 04:55:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2668" class=".btn">#2668</a>
            </td>
            <td>
                <b>
                    docs(example-cbdc-bridging-backend): fix CVE-2020-36632
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Upgraded hardhat to newer versions which don't depend on flat at all.

Fixes #2667

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 04:24:53 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2666" class=".btn">#2666</a>
            </td>
            <td>
                <b>
                    docs(examples): fix CVE-2022-37601 - upgrade to Angular v16
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The new versions allow for loader-utils to be upgraded to non-vulnerable
versions so these are now fixed:

CVE ID: CVE-2022-37601
GHSA ID: GHSA-76p3-8jx3-jpfq

https://github.com/hyperledger/cacti/security/dependabot/257
https://github.com/advisories/GHSA-76p3-8jx3-jpfq

Fixes #2665

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 03:58:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2664" class=".btn">#2664</a>
            </td>
            <td>
                <b>
                    chore(deps): upgrade @lerna-lite/* to v2.5.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In addition to the @lerna-lite upgrade:
1. Also upgraded @commitlint/* to the current latest
2. Deleted some npm scripts that were not used anymore.
3. The canary publish script no longer run the CI (it was a huge overhead)

Fixes #2663

[skip ci]

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-10 03:06:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2660" class=".btn">#2660</a>
            </td>
            <td>
                <b>
                    build(weaver-go): Update code and dependencies in Go packages for Fabric
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Updated Fabric Go SDK code in `weaver/sdks/fabric/go-sdk` to work with the latest protos and release a new version of the library.
- Updated dependencies in `go.mod` for Fabric Interop Chaincode, Fabric Go CLI, and sample chaincodes.
- Updated dependencies in relay `Cargo.lock`.
- Updated Fabric testnet launch script to use the right Fabric Interop Chaincode package.
- Set correct release versions for Fabric driver and IIN Agent local builds.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 13:18:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2659" class=".btn">#2659</a>
            </td>
            <td>
                <b>
                    build(corda-all-in-one-obligation): fix build unable to select packages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Fixed the OpenSSH related problems by wiping the default installation
of it that ships with the distro (Alpine Linux images)
2. Updated the kotlin samples repository's code manually so that it
specifies the platform version as 11 instead of 12 for the basic contracts
which is what we need for Corda v4.8 and v4.9 as well (I'm guessing that
platform  version 12 will stand for v5 when it becomes GA but not sure)
The manual update is done via sed-ing at image build time right after
the kotlin samples repository has been cloned.

Fixes #2621

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-07 06:00:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2658" class=".btn">#2658</a>
            </td>
            <td>
                <b>
                    build(deps): bump webpki from 0.22.0 to 0.22.1 in /weaver/core/relay
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [webpki](https://github.com/briansmith/webpki) from 0.22.0 to 0.22.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/briansmith/webpki/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpki&package-manager=cargo&previous-version=0.22.0&new-version=0.22.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 17:39:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2657" class=".btn">#2657</a>
            </td>
            <td>
                <b>
                    build(deps): bump webpki from 0.22.0 to 0.22.1 in /weaver/common/protos-rs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [webpki](https://github.com/briansmith/webpki) from 0.22.0 to 0.22.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/briansmith/webpki/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=webpki&package-manager=cargo&previous-version=0.22.0&new-version=0.22.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

Dependabot will resolve any conflicts with this PR as long as you don't alter it yourself. You can also trigger a rebase manually by commenting `@dependabot rebase`.

[//]: # (dependabot-automerge-start)
[//]: # (dependabot-automerge-end)

---

<details>
<summary>Dependabot commands and options</summary>
<br />

You can trigger Dependabot actions by commenting on this PR:
- `@dependabot rebase` will rebase this PR
- `@dependabot recreate` will recreate this PR, overwriting any edits that have been made to it
- `@dependabot merge` will merge this PR after your CI passes on it
- `@dependabot squash and merge` will squash and merge this PR after your CI passes on it
- `@dependabot cancel merge` will cancel a previously requested merge and block automerging
- `@dependabot reopen` will reopen this PR if it is closed
- `@dependabot close` will close this PR and stop Dependabot recreating it. You can achieve the same result by closing it manually
- `@dependabot show <dependency name> ignore conditions` will show all of the ignore conditions of the specified dependency
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cacti/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 17:39:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2654" class=".btn">#2654</a>
            </td>
            <td>
                <b>
                    chore(tools): add script to strip out non-production sources
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                To run the script you can execute this on a shell:
    yarn tools:create-production-only-archive

The above will create a temporary clone of the project sources, then
delete a lot of the files that are documentation/test code (e.g. things
that do not go into production). Finally it zips the remaining files
together into something that includes a date & timestamp and the git
hash that the archive was generated from.

There were plans to make the generated zip file also encrypted, but this
is not supported by the library that we are using for compression. The
other library was not necessarily purely Javascript implemented and so
there was some reluctance to use it because of the huge overhead on the
the dependency installation process that we already have from packages
that use native code to satisfy their stated purpose.
So, with all that said, encrypting the .zip file is left as a to-do for
later. The issues tracking this feature are here:
1. https://github.com/cthackers/adm-zip/issues/259
2. https://github.com/cthackers/adm-zip/issues/398

Fixes #2652

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-06 01:29:01 +0000 UTC
    </div>
</div>

