---
layout: default
title: anoncreds-rs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/anoncreds-rs
---

# anoncreds-rs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/anoncreds-rs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/96" class=".btn">#96</a>
            </td>
            <td>
                <b>
                    build: use dynamic libraries for iOS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 11:56:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/95" class=".btn">#95</a>
            </td>
            <td>
                <b>
                    build: build xc frameworks with dylibs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Build the xcframework with dynamic instead of static libraries
- used in the CI now

### Notes

- Dynamic libraries and frameworks pushing to the App Store can fail if it is not setup correctly I think.
  - Since I am not an iOS developer I "botched" together some of the resources about constructing a `.framework` online, but we have to push an app to the app store to see whether it is done properly. if anyone knows anyone with experience like this, help would be awesome!
- This is by no means a perfect shell script. It can be refactored later, but it does the job for now.

Signed-off-by: blu3beri <blu3beri@proton.me>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 11:27:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/94" class=".btn">#94</a>
            </td>
            <td>
                <b>
                    build(deps): bump http-cache-semantics from 4.1.0 to 4.1.1 in /wrappers/javascript
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [http-cache-semantics](https://github.com/kornelski/http-cache-semantics) from 4.1.0 to 4.1.1.
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/kornelski/http-cache-semantics/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=http-cache-semantics&package-manager=npm_and_yarn&previous-version=4.1.0&new-version=4.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/anoncreds-rs/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-02 09:56:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/93" class=".btn">#93</a>
            </td>
            <td>
                <b>
                    build: updated version in the test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 19:02:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/92" class=".btn">#92</a>
            </td>
            <td>
                <b>
                    chore: update versions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: blu3beri <blu3beri@proton.me>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 15:55:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/91" class=".btn">#91</a>
            </td>
            <td>
                <b>
                    fix react native
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Native side of the wrapper should be good but for some reason the native module does not register. I will see if I can fix this somehow, but it might be that it works when its installed via NPM.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-01 12:26:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/89" class=".btn">#89</a>
            </td>
            <td>
                <b>
                    fix(js): proverDid optional in Credential Request
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Since #57, prover_did in Credential Request is optional and some parts of the wrappers have been updated accordingly. But there were some missing changes in interfaces for both Node.JS and React Native wrappers that are updated here.

Signed-off-by: Ariel Gentile <gentilester@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-30 23:13:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/anoncreds-rs/pull/87" class=".btn">#87</a>
            </td>
            <td>
                <b>
                    fix(js): missing export and return type
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Some minor fixes in JavaScript wrapper:

- Remove the need of passing a `Presentation` instance in `verify`, as it is an instance method and can get the handle by itself
- Expose `RevocationStatusList`
- Fix `RevocationRegistryDefinition.load` method
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-28 23:46:22 +0000 UTC
    </div>
</div>

