---
layout: default
title: aries-vcx
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-vcx
---

# aries-vcx <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-vcx){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/732" class=".btn">#732</a>
            </td>
            <td>
                <b>
                    Import/vdr tools
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
        Created At 2023-01-11 12:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/731" class=".btn">#731</a>
            </td>
            <td>
                <b>
                    Sync up cargo lock file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 12:27:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/729" class=".btn">#729</a>
            </td>
            <td>
                <b>
                    Revert hiding mocking behind test_utils feature flag
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">hotfix</span><span class="chip">tests</span>
            </td>
            <td>
                Currently, our tests rely on `test_utils` feature flag indicating whether `MessageId` should be generated randomly or mock value `testid` should be used. Without other changes, setting `test_utils` feature flag without running in test mode causes `MessageId`s to have the same value, which is undesirable. For now, mocking should be exposed without feature flags and work should be done to exclude static mockdata from release builds.

Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-11 10:26:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/727" class=".btn">#727</a>
            </td>
            <td>
                <b>
                    Release 0.51.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Let's include 
- https://github.com/hyperledger/aries-vcx/pull/726

Possibly also
- https://github.com/hyperledger/aries-vcx/pull/723
if we manage to test it today

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 12:01:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/726" class=".btn">#726</a>
            </td>
            <td>
                <b>
                    Update chrono dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Update from `chrono: 0.4.20` (in lock file) to `chrono: 0.4.23`
- The `0.4.20` version of chrono contained regression where it would panic if `TZ` variable is not set https://github.com/chronotope/chrono/releases
- In practice, this could cause panics in mobile environments with rust logging enabled

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-10 11:10:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/725" class=".btn">#725</a>
            </td>
            <td>
                <b>
                    Release 0.51.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-09 14:51:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/723" class=".btn">#723</a>
            </td>
            <td>
                <b>
                    Remove usage of vdrtools's ffi_api feature
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-android</span>
            </td>
            <td>
                - Ios wrapper contains links to vdrtools FFI functions - this PR is removing functions which links to vdrtools symbols (which are included, if vdrtools feature `ffi_api` is enabled).
- Ios wrapper should only use API directly exposed by libvcx
- Consequently we no longer use `vdrtools` feature `ffi_api`

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-07 00:26:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/722" class=".btn">#722</a>
            </td>
            <td>
                <b>
                    Bump tokio from 1.20.2 to 1.20.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [tokio](https://github.com/tokio-rs/tokio) from 1.20.2 to 1.20.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tokio-rs/tokio/commit/ba81945ffc2695b71f2bbcadbfb5e46ec55aaef3"><code>ba81945</code></a> chore: prepare Tokio 1.20.3 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/763bdc967e3e128d1e6e000238f1d257a81bf59a"><code>763bdc9</code></a> ci: run WASI tasks using latest Rust</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9f98535877f8f706b436447952f40f153e2a52dc"><code>9f98535</code></a> Merge remote-tracking branch 'origin/tokio-1.18.x' into fix-named-pipes-1.20</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/9241c3eddf4a6a218681b088d71f7191513e2376"><code>9241c3e</code></a> chore: prepare Tokio v1.18.4 release</li>
<li><a href="https://github.com/tokio-rs/tokio/commit/699573d550fabf4bfb45d82505d6709faaae9037"><code>699573d</code></a> net: fix named pipes server configuration builder</li>
<li>See full diff in <a href="https://github.com/tokio-rs/tokio/compare/tokio-1.20.2...tokio-1.20.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=tokio&package-manager=cargo&previous-version=1.20.2&new-version=1.20.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-vcx/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 21:54:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/721" class=".btn">#721</a>
            </td>
            <td>
                <b>
                    Improve mappings from vdrtools, refactor tests in libvcx
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Changes
- Adjust `IndyErrorKind -> AriesVcxErrorKind` to more sensible mapping
- Add new `LedgerItemNotFound` err kind to ariesvcx, libvcx
- Add new `ObjectAccessError` err kind  to libvcx
- Fix wrong err handling - it wrong `key` is used to open wallet, throw `LibvcxErrorKind::WalletAccessFailed` err kind instead of "unmapped" libindy error `LibvcxErrorKind::LibndyError(207)`. Added test to libvcx to cover this case

### Refactoring
- Move tests from `api_c` layer to `api_vcx`
- Delete dead code

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-06 18:16:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/720" class=".btn">#720</a>
            </td>
            <td>
                <b>
                    CI: Do not use deprecated set-output, update artifact publishing action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">skip-ios</span><span class="chip">skip-android</span>
            </td>
            <td>
                - `set-output::` is deprecated in produces warnings in CI
- removed the usage from our CI code
- upgraded `actions/upload-artifact@v3` 
- `set-output::` warnings still coming out from `actions-rs/toolchain@v1` - keep eye on https://github.com/actions-rs/toolchain/issues/221

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 18:01:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/719" class=".btn">#719</a>
            </td>
            <td>
                <b>
                    Update readme.md files, update architecture diagram
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - The root `readme.md` is more general and also
  - it puts `aries-vcx` along with the smaller subcrates as main components
  - `libvcx` is nuanced as "one of the crates built on aries-vcx"   
- Add specific readme for `libvcx`
- Add specific readme for `aries-vcx`
- Updated maintainers file
- Update architecture diagrams - where originally we had 1 diagram which spanned from libcx wrappers all way down to aries-vcx modules, now there's 2 diagrams instead.
   - One diagram for `aries-vcx` crate architecture only
   - One diagram for `libvcx` and surrounding language wrappers, depicting `aries-vcx` simply as 1 component

Signed-off-by: Patrik Stas <patrik.stas@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-05 17:17:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/718" class=".btn">#718</a>
            </td>
            <td>
                <b>
                    Nonmediated connection handles API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Miroslav Kovar <miroslav.kovar@absa.africa>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-01-04 15:59:31 +0000 UTC
    </div>
</div>

