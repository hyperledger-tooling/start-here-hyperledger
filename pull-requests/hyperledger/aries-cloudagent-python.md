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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2344" class=".btn">#2344</a>
            </td>
            <td>
                <b>
                    0.9.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 20:03:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2343" class=".btn">#2343</a>
            </td>
            <td>
                <b>
                    Add more context to the ACA-Py Revocation handling documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 18:12:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2341" class=".btn">#2341</a>
            </td>
            <td>
                <b>
                    fix: ensure request matches offer, if sent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This change implements checking that ld proof credential requests match their corresponding offer, if an offer was sent.

If using the `--auto-*` flags for issuance, it was possible for the receiver of the credential offer to change values in the request and ACA-Py would accept this and issue based off of the request values. The `--auto-*` flags are debug flags and should not be used in production which would mean that a controller should have been able to catch this discrepancy. However, it is still expedient for ACA-Py to check that the offer and request match to avoid this slipping past the controller as well.

There is a side affect of this check. We were permitting late binding of the credential subject ID to the holder in the request. Meaning, on request, the holder will automatically (when using auto flags) insert a DID key as the credential subject ID to ensure the holder can actually present proof of possession later. These changes modify this behavior such that it only applies iff the credential subject id is not set already (e.g. in the credential offer). This enables the issuer to bind the credential to a DID other than the holder's pairwise DID if an alternate is known to the issuer. If the issuer wants to permit late binding by the holder still, the credential subject ID should be omitted in the offer.

So, to summarize, the two modifications implemented here:
- Ensure the request doesn't change the credential unless the offer explicitly omits a credential subject ID
- Only override with holder did if the credential subject ID is omitted
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-24 14:32:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2340" class=".btn">#2340</a>
            </td>
            <td>
                <b>
                    Document the Indy SDK to Askar Migration process
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 23:08:02 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2339" class=".btn">#2339</a>
            </td>
            <td>
                <b>
                    Feat: Support Selectable Write Ledger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - WIP [under testing and debugging]
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 15:57:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2338" class=".btn">#2338</a>
            </td>
            <td>
                <b>
                    0.9.0-rc0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Stephen Curran <swcurran@gmail.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 13:53:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2336" class=".btn">#2336</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `requests` to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `requests` dependency for ACA-py is currently using version `2.25.1` (Dec 2020), and has seen numerous improvements since then ito vulnerability fixes, speed optimizations, and support for python 3.10+

See changelogs here: https://github.com/psf/requests/releases
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 09:08:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2335" class=".btn">#2335</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `pyjwt` to latest; introduce leeway to `jwt.decode`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Latest release (2.8) introduces support for python 3.10+

Release notes: https://github.com/jpadilla/pyjwt/releases

Note: `jwt.decode` can fail spuriously due to breaking changes introduced in https://github.com/jpadilla/pyjwt/pull/797, where an exception is raised if the 'issued at' time of the JWT is in the future when decoding, with default 0 leeway. This means that a miniscule mismatch in clock synchronization, between generation and decoding of JWT, can now cause a failure when decoding. This arose in the integration tests, and is resolved with a leeway of 1 second.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 09:02:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2334" class=".btn">#2334</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `packaging` to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The `packaging` dependency is pinned to version 20. This is incompatible with the latest release of the `black` formatter:
```
black 23.7.0 requires packaging>=22.0, but you have packaging 20.9 which is incompatible.
```

There doesn't seem to be any breaking changes in the new packaging release, so this PR bumps the dependency to latest
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-21 08:32:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2333" class=".btn">#2333</a>
            </td>
            <td>
                <b>
                    Add revocation registry rotate to faber demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add new revocation registry endpoint to `faber` demo.

Update the readme with new actions:

```
    (7) Rotate Revocation Registry
    (8) List Revocation Registries
```

**Important** includes a fix for the decommission and init new registry logic. Running the demo revealed that 2 active registries were not always created, so simplified the logic and enforced create/init when `active` is `decommissioned`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 19:41:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2332" class=".btn">#2332</a>
            </td>
            <td>
                <b>
                    chore: add indy deprecation warnings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds deprecation warnings when using the Indy wallet type. The newly added warnings will look like this on startup, assuming wallet type indy is used and log level is set to at least `WARNING`:

```
2023-07-20 19:34:16,917 aries_cloudagent.resolver WARNING Ledger is not configured, not loading IndyDIDResolver
2023-07-20 19:34:17,043 aries_cloudagent.indy.sdk.profile WARNING Indy wallet type is deprecated, use Askar instead; see: https://github.com/hyperledger/aries-cloudagent-python/issues/2330
2023-07-20 19:34:17,052 indy.libindy WARNING _indy_loop_callback: Function returned error
2023-07-20 19:34:18,298 indy.libindy WARNING _indy_loop_callback: Function returned error
2023-07-20 19:34:18,300 aries_cloudagent.core.conductor WARNING No ledger configured

::::::::::::::::::::::::::::::::::::::::::::::
:: Aries Cloud Agent                        ::
::                                          ::
::                                          ::
:: Inbound Transports:                      ::
::                                          ::
::   - http://0.0.0.0:3000                  ::
::                                          ::
:: Outbound Transports:                     ::
::                                          ::
::   - http                                 ::
::   - https                                ::
::                                          ::
:: Administration API:                      ::
::                                          ::
::   - http://0.0.0.0:3001                  ::
::                                          ::
::                               ver: 0.8.2 ::
::::::::::::::::::::::::::::::::::::::::::::::

Listening...

DEPRECATTION NOTICE:
        The Indy wallet type is deprecated, use Askar instead; see: https://github.com/hyperledger/aries-cloudagent-python/issues/2330

2023-07-20 19:34:18,473 aries_cloudagent.core.conductor WARNING Wallet version storage record not found.
2023-07-20 19:34:18,473 aries_cloudagent.core.conductor WARNING No upgrade from version was found from wallet or via --from-version startup argument. Defaulting to v0.7.5.
2023-07-20 19:34:18,480 indy.libindy WARNING _indy_loop_callback: Function returned error
```

The `DEPRECATION NOTICE: The indy wallet type...` lines will always be printed regardless of log level to `stderr` (but still only when using the indy wallet type).

The lines added to the profile will ensure warnings are logged whenever a new sub-wallet is created in addition to the main wallet when operating without multi-tenancy. The `warnings.warn` lines show up in different circumstances from the `logging.warning` depending on how you're using ACA-Py. I really wanted something attention grabbing though so I added the `print_notices` to be printed immediately following the banner.

Open to suggestions on what should be included in the warning or if we should point people to somewhere other than #2330.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 19:39:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2331" class=".btn">#2331</a>
            </td>
            <td>
                <b>
                    Fix: Track endorser and author roles in per-tenant settings
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Bug fixes #2233 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 17:16:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2329" class=".btn">#2329</a>
            </td>
            <td>
                <b>
                    chore: update PyYAML
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The older version seems to be causing errors in builds downstream for plugins and deployments after the recent 6.0.1 release.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 16:00:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2328" class=".btn">#2328</a>
            </td>
            <td>
                <b>
                    Added base wallet provisioning details to Multitenancy.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves #2317 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 16:00:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2325" class=".btn">#2325</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump aiohttp from 3.8.4 to 3.8.5 in /demo/playground/scripts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [aiohttp](https://github.com/aio-libs/aiohttp) from 3.8.4 to 3.8.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/releases">aiohttp's releases</a>.</em></p>
<blockquote>
<h2>3.8.5</h2>
<h2>Security bugfixes</h2>
<ul>
<li>
<p>Upgraded the vendored copy of llhttp_ to v8.1.1 -- by :user:<code>webknjaz</code>
and :user:<code>Dreamsorcerer</code>.</p>
<p>Thanks to :user:<code>sethmlarson</code> for reporting this and providing us with
comprehensive reproducer, workarounds and fixing details! For more
information, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w</a>.</p>
<p>.. _llhttp: <a href="https://llhttp.org">https://llhttp.org</a></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7346">#7346</a>)</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p>Added information to C parser exceptions to show which character caused the error. -- by :user:<code>Dreamsorcerer</code></p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7366">#7366</a>)</p>
</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>
<p>Fixed a transport is :data:<code>None</code> error -- by :user:<code>Dreamsorcerer</code>.</p>
<p>(<a href="https://redirect.github.com/aio-libs/aiohttp/issues/3355">#3355</a>)</p>
</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/aio-libs/aiohttp/blob/v3.8.5/CHANGES.rst">aiohttp's changelog</a>.</em></p>
<blockquote>
<h1>3.8.5 (2023-07-19)</h1>
<h2>Security bugfixes</h2>
<ul>
<li>
<p>Upgraded the vendored copy of llhttp_ to v8.1.1 -- by :user:<code>webknjaz</code>
and :user:<code>Dreamsorcerer</code>.</p>
<p>Thanks to :user:<code>sethmlarson</code> for reporting this and providing us with
comprehensive reproducer, workarounds and fixing details! For more
information, see
<a href="https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w">https://github.com/aio-libs/aiohttp/security/advisories/GHSA-45c4-8wx5-qw6w</a>.</p>
<p>.. _llhttp: <a href="https://llhttp.org">https://llhttp.org</a></p>
<p><code>[#7346](https://github.com/aio-libs/aiohttp/issues/7346) &lt;https://github.com/aio-libs/aiohttp/issues/7346&gt;</code>_</p>
</li>
</ul>
<h2>Features</h2>
<ul>
<li>
<p>Added information to C parser exceptions to show which character caused the error. -- by :user:<code>Dreamsorcerer</code></p>
<p><code>[#7366](https://github.com/aio-libs/aiohttp/issues/7366) &lt;https://github.com/aio-libs/aiohttp/issues/7366&gt;</code>_</p>
</li>
</ul>
<h2>Bugfixes</h2>
<ul>
<li>
<p>Fixed a transport is :data:<code>None</code> error -- by :user:<code>Dreamsorcerer</code>.</p>
<p><code>[#3355](https://github.com/aio-libs/aiohttp/issues/3355) &lt;https://github.com/aio-libs/aiohttp/issues/3355&gt;</code>_</p>
</li>
</ul>
<hr />
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9c13a52c21c23dfdb49ed89418d28a5b116d0681"><code>9c13a52</code></a> Bump aiohttp to v3.8.5 a security release</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/7c02129567bc4ec59be467b70fc937c82920948c"><code>7c02129</code></a>  Bump pypa/cibuildwheel to v2.14.1</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/135a45e9d655d56e4ebad78abe84f1cb7b5c62dc"><code>135a45e</code></a> Improve error messages from C parser (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7366">#7366</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7380">#7380</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/9337fb3f2ab2b5f38d7e98a194bde6f7e3d16c40"><code>9337fb3</code></a> Fix bump llhttp to v8.1.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7367">#7367</a>) (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7377">#7377</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/f07e9b44b5cb909054a697c8dd447b30dbf8073e"><code>f07e9b4</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7373">#7373</a>/66e261a5 backport][3.8] Drop azure mention (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7374">#7374</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/01d9b70e5477cd746561b52225992d8a2ebde953"><code>01d9b70</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7370">#7370</a>/22c264ce backport][3.8] fix: Spelling error fixed (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7371">#7371</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/3577b1e3719d4648fa973dbdec927f78f9df34dd"><code>3577b1e</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7359">#7359</a>/7911f1e9 backport][3.8]  Set up secretless publishing to PyPI (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7360">#7360</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/8d45f9c99511cd80140d6658bd9c11002c697f1c"><code>8d45f9c</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7333">#7333</a>/3a54d378 backport][3.8] Fix TLS transport is <code>None</code> error (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7357">#7357</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/dd8e24e77351df9c0f029be49d3c6d7862706e79"><code>dd8e24e</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7343">#7343</a>/18057581 backport][3.8] Mention encoding in <code>yarl.URL</code> (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7355">#7355</a>)</li>
<li><a href="https://github.com/aio-libs/aiohttp/commit/40874103ebfaa1007d47c25ecc4288af873a07cf"><code>4087410</code></a> [PR <a href="https://redirect.github.com/aio-libs/aiohttp/issues/7346">#7346</a>/346fd202 backport][3.8]  Bump vendored llhttp to v8.1.1 (<a href="https://redirect.github.com/aio-libs/aiohttp/issues/7352">#7352</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/aio-libs/aiohttp/compare/v3.8.4...v3.8.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=aiohttp&package-manager=pip&previous-version=3.8.4&new-version=3.8.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 15:07:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2322" class=".btn">#2322</a>
            </td>
            <td>
                <b>
                    ⬆️ upgrade `marshmallow` to latest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `marshmallow` dependency is currently pinned to `3.5.1`. There are no breaking changes in marshmallow's minor releases, so this PR unpins the dependency and upgrades to latest `3.19.0`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-20 10:41:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2313" class=".btn">#2313</a>
            </td>
            <td>
                <b>
                    Add workaround for ARM based macs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - ARM based macs caused dependency issues with indy-vdr and ursa-bbs-signatures
- Solution checks for architecture and updates DOCKER_DEFAULT_PLATFORM
- Closes #2311 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-19 14:53:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2309" class=".btn">#2309</a>
            </td>
            <td>
                <b>
                    API endpoint to decommission revocation registry
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes issue #2304 

There are two active registries at a given time, this API endpoint - given a `cred_def_id` - will find and decommission the active revocation registries and will kick off the procedure to create new active registries (same as when a registry is full).

Note that the `pytest` doesn't have a handler to transition the `init` state registries to `active`, so we simulate that before testing the decommission code. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-07-18 02:12:20 +0000 UTC
    </div>
</div>

