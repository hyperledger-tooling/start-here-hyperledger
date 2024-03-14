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
                PR <a href="https://github.com/hyperledger/cacti/pull/3073" class=".btn">#3073</a>
            </td>
            <td>
                <b>
                    feat(connector-besu): add continuous benchmarking with JMeter
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Primary Changes
---------------

1. Added continuous benchmarking using JMeter that reports performance in cactus-plugin-ledger-connector-besu using one of its endpoint.

fixes: #2672

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 08:15:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3072" class=".btn">#3072</a>
            </td>
            <td>
                <b>
                    build(rust-compiler): retire the container image and the test cases
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This started off with me trying to fix the CVEs in the rust-compiler image.
2. I was able to get rid of most of them by changing the base image to ubuntu-24.04
3. The remaining high and critical ones were due to wasm-pack so went to see
if we could upgrade that but we are already on the latest which is 8 months old.
The vulnerabilities were reported on the wasm-pack repo 6 months ago along with
a pull request that fixes them, neither the issue nor the pull request fixing it
received any attention from the wasm-pack maintainers which lead me to believe
that it is a liability to depend on it right now and we should instead look into
a different tooling where the maintenance happens to have a little more resources
dedicated to it. Java/Kotlin might be the way to go.
1. I've also looked into possible alternatives to wasm-pack but the only
other tool I found that does the same thing is cargo-web which hasn't had
a new release for 4 years and counting and has even more CVEs plaguing it
than wasm-pack.
1. The official web assembly site links to wasm-pack when it comes to
compiling to it from Rust so there's probably not a better maintained tool
out there, but if someone finds something I'd love to start using it.
In the meantime I'll just archive/retire/delete the rust compiler image
and the tests associated with it because it's a maintenance burden that
we don't need to carry.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-08 00:12:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3071" class=".btn">#3071</a>
            </td>
            <td>
                <b>
                    build: eslint, tslint, prettier consolidation, purge from non-root pkgs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. We had dozens of different versions of ESLint, TSLint, Prettier
declard in package.json files. Most versions were so old that they had
ben EOL for several years too.
2. The presence of these and their scripts/config files/etc were making
it impossible to run the linter on the sub-folders where these were
being used.
3. As part of the big push to consolidate linting and code formatting on
the entire project, this is phase 1 where I purged the mentioned dependencies
from the project and now only the root package.json file declares them
which is currently using the latest and greatest versions.
4. I know that the diff is huge in this pull request but there are no
code changes that would cause bugs or logic modification at all. It's all
just applying automated formatting and linting on sub-directories where
previously this was impossible. E.g., this entire change should not cause
any sort of bugs (but of course we'll see what the CI execution has to
say about that).
5. The follow-up phases will consist of slowly applying more brazen
refactoring in a much more targeted and surgical manner with small
pull requests that are easy and quick to review.
6. The smaller pull requests will target sub-directories that we still
cannot include in the linting (see the .eslintignore file for a list) and
then culminate in us finally enabling the linter for everything.
7. The root folder's ESLint ignore file was refactored in a way that the
files that we plan on fixing later are now ignored on a one by one basis
instead of using patterns. This makes the ignore file a collection of
to-dos where one can delete a single line from the ignore file (pertaining
to a single file that is being ignored) and then proceed to fix the linter
issues and send a small, easy to review pull request that does not overwhelm
the maintainers when they are trying to review a huge diff with a large
batch of linter fixes. Phase two of this project is then to one by one
drain the ignore entries of these mentioned files from the ESLint ignore
file.

So, the bottom line is that this might look like a hugely disruptive
change, but I've done my best to keep it as simple as possible so that
we don't have to worry about reviewing it line by line and instead just
focus on the big picture and the principle idea(s) behind it (code quality).

If it does end up introducing a bug or CI breakage, I'll volunteer to fix
those because I'm very confident that even if this does happen, it will
be very minor and quick fixes necessary only so I don't mind being on the
hook for it.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 22:03:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3070" class=".btn">#3070</a>
            </td>
            <td>
                <b>
                    tools: fix scripts - use run-time-error instead of run-time-error-cjs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The `-cjs` version of the package was put into place because in the
production packages we needed it to be able to import the dependency
despite us not using ESM just yet.
2. We did a blanket search and replace at the time which seemed like a
good idea but turns out it wasn't because there are some tooling scripts
(the ones in this diff) that are already using ESM and for those the
-cjs flavored package started breaking the code.
3. So this change is just a partial/selective/surgical revert of the
earlier project-wide migratin from run-time-error to run-time-error-cjs.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 19:44:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3068" class=".btn">#3068</a>
            </td>
            <td>
                <b>
                    build(deps): bump jose from 4.9.2 to 4.15.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [jose](https://github.com/panva/jose) from 4.9.2 to 4.15.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/releases">jose's releases</a>.</em></p>
<blockquote>
<h2>v4.15.5</h2>
<h3>Fixes</h3>
<ul>
<li>add a maxOutputLength option to zlib inflate (<a href="https://github.com/panva/jose/commit/1b91d88d2f8233f3477a5f4579aa5f8057b2ee8b">1b91d88</a>), fixes <a href="https://github.com/panva/jose/security/advisories/GHSA-hhhv-q57g-882q">CVE-2024-28176</a></li>
</ul>
<h2>v4.15.4</h2>
<h3>Fixes</h3>
<ul>
<li><strong>types:</strong> export GetKeyFunction (<a href="https://redirect.github.com/panva/jose/issues/592">#592</a>) (<a href="https://github.com/panva/jose/commit/936c9dff2bc124dc5f64906a96f665a28e57392c">936c9df</a>), closes <a href="https://redirect.github.com/panva/jose/issues/591">#591</a></li>
</ul>
<h2>v4.15.3</h2>
<p>This release contains only Node.js CITGM related test updates.</p>
<p>Fixes <a href="https://redirect.github.com/nodejs/citgm/issues/1011">nodejs/citgm#1011</a></p>
<h2>v4.15.2</h2>
<h3>Fixes</h3>
<ul>
<li><strong>build:</strong> add a node target for jose-browser-runtime releases (<a href="https://github.com/panva/jose/commit/abb63d0e8e7a55326dc343eec5f5eee9addc1dcf">abb63d0</a>)</li>
</ul>
<h2>v4.15.1</h2>
<h3>Fixes</h3>
<ul>
<li>resolve missing types for the cryptoRuntime const (<a href="https://github.com/panva/jose/commit/16279652a67133fba0db7c9879767f000a8f1662">1627965</a>)</li>
</ul>
<h2>v4.15.0</h2>
<h3>Features</h3>
<ul>
<li>export the used crypto runtime as a constant (<a href="https://github.com/panva/jose/commit/0681dda1592a82c22a18981002b3763c502d0fc4">0681dda</a>)</li>
</ul>
<h2>v4.14.6</h2>
<h3>Fixes</h3>
<ul>
<li><strong>build:</strong> publish bundle and umd files with jose-browser-runtime module (<a href="https://github.com/panva/jose/commit/62fcbcc2170db00f5bbfc817839523dbf970239f">62fcbcc</a>), closes <a href="https://redirect.github.com/panva/jose/issues/571">#571</a></li>
</ul>
<h2>v4.14.5</h2>
<h3>Refactor</h3>
<ul>
<li>catch type error when decoding base64url signature (<a href="https://redirect.github.com/panva/jose/issues/569">#569</a>) (<a href="https://github.com/panva/jose/commit/935e920d29d242e0446d365b1e4f0449d144c23c">935e920</a>)</li>
<li>catch type errors when decoding various base64url strings (<a href="https://github.com/panva/jose/commit/9024e870ece4ef121205dadc733c36d7978b97ab">9024e87</a>)</li>
</ul>
<h2>v4.14.4</h2>
<h3>Refactor</h3>
<ul>
<li>cleanup NODE-ED25519 workerd workarounds (<a href="https://github.com/panva/jose/commit/072e83de5bf3a15775b0bf25ef8afa8851b8862d">072e83d</a>)</li>
</ul>
<h2>v4.14.3</h2>
<h3>Reverts</h3>
<ul>
<li>Revert &quot;fix(types): headers and payloads may only be JSON values and primitives&quot; (<a href="https://github.com/panva/jose/commit/06d8101a5827a69bb25c2847b1a10d03f015db03">06d8101</a>), closes <a href="https://redirect.github.com/panva/jose/issues/534">#534</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/panva/jose/blob/v4.15.5/CHANGELOG.md">jose's changelog</a>.</em></p>
<blockquote>
<h2><a href="https://github.com/panva/jose/compare/v4.15.4...v4.15.5">4.15.5</a> (2024-03-07)</h2>
<h3>Fixes</h3>
<ul>
<li>add a maxOutputLength option to zlib inflate (<a href="https://github.com/panva/jose/commit/1b91d88d2f8233f3477a5f4579aa5f8057b2ee8b">1b91d88</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.15.3...v4.15.4">4.15.4</a> (2023-10-14)</h2>
<h3>Fixes</h3>
<ul>
<li><strong>types:</strong> export GetKeyFunction (<a href="https://redirect.github.com/panva/jose/issues/592">#592</a>) (<a href="https://github.com/panva/jose/commit/936c9dff2bc124dc5f64906a96f665a28e57392c">936c9df</a>), closes <a href="https://redirect.github.com/panva/jose/issues/591">#591</a></li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.15.2...v4.15.3">4.15.3</a> (2023-10-11)</h2>
<h2><a href="https://github.com/panva/jose/compare/v4.15.1...v4.15.2">4.15.2</a> (2023-10-04)</h2>
<h3>Fixes</h3>
<ul>
<li><strong>build:</strong> add a node target for jose-browser-runtime releases (<a href="https://github.com/panva/jose/commit/abb63d0e8e7a55326dc343eec5f5eee9addc1dcf">abb63d0</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.15.0...v4.15.1">4.15.1</a> (2023-10-02)</h2>
<h3>Fixes</h3>
<ul>
<li>resolve missing types for the cryptoRuntime const (<a href="https://github.com/panva/jose/commit/16279652a67133fba0db7c9879767f000a8f1662">1627965</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.14.6...v4.15.0">4.15.0</a> (2023-10-02)</h2>
<h3>Features</h3>
<ul>
<li>export the used crypto runtime as a constant (<a href="https://github.com/panva/jose/commit/0681dda1592a82c22a18981002b3763c502d0fc4">0681dda</a>)</li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.14.5...v4.14.6">4.14.6</a> (2023-09-04)</h2>
<h3>Fixes</h3>
<ul>
<li><strong>build:</strong> publish bundle and umd files with jose-browser-runtime module (<a href="https://github.com/panva/jose/commit/62fcbcc2170db00f5bbfc817839523dbf970239f">62fcbcc</a>), closes <a href="https://redirect.github.com/panva/jose/issues/571">#571</a></li>
</ul>
<h2><a href="https://github.com/panva/jose/compare/v4.14.4...v4.14.5">4.14.5</a> (2023-09-02)</h2>
<h3>Refactor</h3>
<ul>
<li>catch type error when decoding base64url signature (<a href="https://redirect.github.com/panva/jose/issues/569">#569</a>) (<a href="https://github.com/panva/jose/commit/935e920d29d242e0446d365b1e4f0449d144c23c">935e920</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/panva/jose/commit/765aafd226d30dbab14038bfadc8af1881dce158"><code>765aafd</code></a> chore(release): 4.15.5</li>
<li><a href="https://github.com/panva/jose/commit/b36e45e008b8af2af38d9d2a8305e03ba77da644"><code>b36e45e</code></a> test: add export check to x509 pem import tests</li>
<li><a href="https://github.com/panva/jose/commit/e839ecbd7975c4264de6f10fa2b1aa00ad4121fa"><code>e839ecb</code></a> test: stop testing JWE RSA1_5 Algorithm</li>
<li><a href="https://github.com/panva/jose/commit/1b91d88d2f8233f3477a5f4579aa5f8057b2ee8b"><code>1b91d88</code></a> fix: add a maxOutputLength option to zlib inflate</li>
<li><a href="https://github.com/panva/jose/commit/9ca2b2427d15c3a410d9fe9ddb86e85fdc55e9ac"><code>9ca2b24</code></a> build: remove release action</li>
<li><a href="https://github.com/panva/jose/commit/f3035d8897b25dc9cd8e094f943e57ec74eeccb1"><code>f3035d8</code></a> chore: cleanup after release</li>
<li><a href="https://github.com/panva/jose/commit/f0bb22018cd673833e58445c769f24db9b044332"><code>f0bb220</code></a> chore(release): 4.15.4</li>
<li><a href="https://github.com/panva/jose/commit/6f38554f722c7c7c0f0d61e8a5276fae52e2722f"><code>6f38554</code></a> chore: bump dev deps</li>
<li><a href="https://github.com/panva/jose/commit/936c9dff2bc124dc5f64906a96f665a28e57392c"><code>936c9df</code></a> fix(types): export GetKeyFunction (<a href="https://redirect.github.com/panva/jose/issues/592">#592</a>)</li>
<li><a href="https://github.com/panva/jose/commit/5ac6619b11db84f4e776b95f69f935e8a050b0a0"><code>5ac6619</code></a> chore: bump dev deps</li>
<li>Additional commits viewable in <a href="https://github.com/panva/jose/compare/v4.9.2...v4.15.5">compare view</a></li>
</ul>
</details>
<details>
<summary>Maintainer changes</summary>
<p>This version was pushed to npm by <a href="https://www.npmjs.com/~panva">panva</a>, a new releaser for jose since your current version.</p>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jose&package-manager=npm_and_yarn&previous-version=4.9.2&new-version=4.15.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-03-07 19:26:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3067" class=".btn">#3067</a>
            </td>
            <td>
                <b>
                    build: upgrade & consolidate @types/node at v18.11.9 - NodeJS typings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The default/suggested NodeJS version we use and recommend is v18 LTS
but there were a lot of places in the code that still declared v14 and
v16 both of which are now EOL.
2. This was/is working fine but eventually we'll hit some compiler issue
where the upgrade will be forced so it's most likely wiser to do this little
quality of life/housekeeping change now when it's not urgent.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 18:34:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3066" class=".btn">#3066</a>
            </td>
            <td>
                <b>
                    ci: upgrade and pin to ubuntu-22.04 project-wide for CI runner images
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This does not upgrade all the container images that we build and publish
as part of the project, it just upgrades the runner images that are being
used by the continuous integration environment.
2. I also deleted a .yaml file that I left in the diff of another pull request
by accident. Apologies for the littering.
3. Upgrade: as-in, I bumped the 20.04 versions to 22.04
4. Pin: as-in, replaced `ubuntu-latest` with `ubuntu-22.04` everywhere.
5. Reasoning: 24.04 is out now and so we have to keep up with the times
because soon there'll be a stop to security patches even on what used to
be LTS (20.04). It is better to find out now if we have a problem with
ubuntu 22.04 rather than later when it's become urgent to upgrade.
6. The risk of something breaking because of these upgrades is most likely
low since ubuntu is one of the most stable distributions out there.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-07 17:57:05 +0000 UTC
    </div>
</div>

