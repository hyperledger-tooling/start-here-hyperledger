---
layout: default
title: aries-mobile-agent-react-native
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-mobile-agent-react-native
---

# aries-mobile-agent-react-native <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-mobile-agent-react-native){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/196" class=".btn">#196</a>
            </td>
            <td>
                <b>
                    Expire cache
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Expire caches to see if that fixes the iOS build issue.

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-29 00:02:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    Activate get started button in on-boarding carousel
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

- Enable the on-boaridng "Get Started" button to complete the tutorial screens;
- Add tests for Button component;
- Remove dead props for Button component (cleanup);
- Debug and fix warning (__Animated: `useNativeDriver` is not supported__) with test run. 
- Cleaned up ambiguity with `create` in some tests

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 21:59:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    Credentials list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

* Updates credentials list user interface with refreshed look
* Refactors common logic into helper functions
* Refactors credential offer and proof request screens with new helper functions

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 18:54:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/193" class=".btn">#193</a>
            </td>
            <td>
                <b>
                    Bump nanoid from 3.1.25 to 3.2.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [nanoid](https://github.com/ai/nanoid) from 3.1.25 to 3.2.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/ai/nanoid/blob/main/CHANGELOG.md">nanoid's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>This project adheres to <a href="http://semver.org/">Semantic Versioning</a>.</p>
<h2>3.2</h2>
<ul>
<li>Added <code>--size</code> and <code>--alphabet</code> arguments to binary (by Vitaly Baev).</li>
</ul>
<h2>3.1.32</h2>
<ul>
<li>Reduced <code>async</code> exports size (by Artyom Arutyunyan).</li>
<li>Moved from Jest to uvu (by Vitaly Baev).</li>
</ul>
<h2>3.1.31</h2>
<ul>
<li>Fixed collision vulnerability on object in <code>size</code> (by Artyom Arutyunyan).</li>
</ul>
<h2>3.1.30</h2>
<ul>
<li>Reduced size for project with <code>brotli</code> compression (by Anton Khlynovskiy).</li>
</ul>
<h2>3.1.29</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.28</h2>
<ul>
<li>Reduced npm package size.</li>
</ul>
<h2>3.1.27</h2>
<ul>
<li>Cleaned <code>dependencies</code> from development tools.</li>
</ul>
<h2>3.1.26</h2>
<ul>
<li>Improved performance (by Eitan Har-Shoshanim).</li>
<li>Reduced npm package size.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/ai/nanoid/commit/23b136929a6d58f32e31b269534a3ce3f680a086"><code>23b1369</code></a> Release 3.2 version</li>
<li><a href="https://github.com/ai/nanoid/commit/967788efce880960512f969a56f8f22f3fc20bae"><code>967788e</code></a> Remove TS test tools</li>
<li><a href="https://github.com/ai/nanoid/commit/27eaa90cd207a7782bbcf17343092ae87dd62164"><code>27eaa90</code></a> Simplify new binary tool</li>
<li><a href="https://github.com/ai/nanoid/commit/a9d91239931dc77506381874826d297aee71d6ef"><code>a9d9123</code></a> Update dependencies</li>
<li><a href="https://github.com/ai/nanoid/commit/32b9bdaab1fbc28576b17de8516164ce0360f292"><code>32b9bda</code></a> Allows passing size or custom alphabet via cli as args (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/334">#334</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/246d5f87b6b34e23b5e401bdf3da1f80c810ac4c"><code>246d5f8</code></a> Update vite</li>
<li><a href="https://github.com/ai/nanoid/commit/afdf9c92b41427f35476fbe14b5af5d73dd7fbdb"><code>afdf9c9</code></a> doc: Fixed Typo (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/335">#335</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/90a446fef3ecaac78e5af2ea01025c4f40182e2b"><code>90a446f</code></a> Update benchmark results</li>
<li><a href="https://github.com/ai/nanoid/commit/8ba2319b579895cc1f9060b9946a44852f97c509"><code>8ba2319</code></a> bench: add <code>@​napi-rs/uuid</code> v4 (<a href="https://github-redirect.dependabot.com/ai/nanoid/issues/333">#333</a>)</li>
<li><a href="https://github.com/ai/nanoid/commit/f4257780ece488734a65c176e80c2fd8ab6aab8e"><code>f425778</code></a> Release 3.1.32 version</li>
<li>Additional commits viewable in <a href="https://github.com/ai/nanoid/compare/3.1.25...3.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nanoid&package-manager=npm_and_yarn&previous-version=3.1.25&new-version=3.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 16:39:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    Bump follow-redirects from 1.14.4 to 1.14.7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [follow-redirects](https://github.com/follow-redirects/follow-redirects) from 1.14.4 to 1.14.7.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ede36d7c60d3acdcd324dcd99a9dbd52e4fb3a6"><code>2ede36d</code></a> Release version 1.14.7 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/8b347cbcef7c7b72a6e9be20f5710c17d6163c22"><code>8b347cb</code></a> Drop Cookie header across domains.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/6f5029ae1a0fdab4dc25f6379a5ee303c2319070"><code>6f5029a</code></a> Release version 1.14.6 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/af706bee57de954414c0bde0a9f33e62beea3e52"><code>af706be</code></a> Ignore null headers.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/d01ab7a5c5df3617c7a40a03de7af6427fdfac55"><code>d01ab7a</code></a> Release version 1.14.5 of the npm package.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/40052ea8aa13559becee5795715c1d45b1f0eb76"><code>40052ea</code></a> Make compatible with Node 17.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/86f7572f9365dadc39f85916259b58973819617f"><code>86f7572</code></a> Fix: clear internal timer on request abort to avoid leakage</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2e1eaf0218c5315a2ab27f53964d0535d4dafb51"><code>2e1eaf0</code></a> Keep Authorization header on subdomain redirects.</li>
<li><a href="https://github.com/follow-redirects/follow-redirects/commit/2ad9e82b6277ae2104f7770e9ff1186cc6da29d4"><code>2ad9e82</code></a> Carry over Host header on relative redirects (<a href="https://github-redirect.dependabot.com/follow-redirects/follow-redirects/issues/172">#172</a>)</li>
<li>See full diff in <a href="https://github.com/follow-redirects/follow-redirects/compare/v1.14.4...v1.14.7">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=follow-redirects&package-manager=npm_and_yarn&previous-version=1.14.4&new-version=1.14.7)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 16:39:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/191" class=".btn">#191</a>
            </td>
            <td>
                <b>
                    Bump validator from 13.6.0 to 13.7.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [validator](https://github.com/validatorjs/validator.js) from 13.6.0 to 13.7.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/validatorjs/validator.js/releases">validator's releases</a>.</em></p>
<blockquote>
<h2>13.7.0</h2>
<h1><code>13.7.0</code></h1>
<h2>New Features</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1706">#1706</a> <code>isISO4217</code>, currency code validator <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
</ul>
<h2>Fixes and Enhancements</h2>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1647">#1647</a> <code>isFQDN</code>: add <code>allow_wildcard</code> option <a href="https://github.com/fasenderos"><code>@​fasenderos</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1654">#1654</a> <code>isRFC3339</code>: Disallow prepended and appended strings to RFC 3339 date-time <a href="https://github.com/jmacmahon"><code>@​jmacmahon</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1658">#1658</a> maintenance: increase code coverage <a href="https://github.com/tux-tn"><code>@​tux-tn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1669">#1669</a> <code>IBAN</code> export list of country codes that implement IBAN <a href="https://github.com/dror-heller"><code>@​dror-heller</code></a> <a href="https://github.com/fedeci"><code>@​fedeci</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1676">#1676</a> <code>isBoolean</code>: add <code>loose</code> option <a href="https://github.com/brybrophy"><code>@​brybrophy</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1697">#1697</a> maintenance: fix npm installation error <a href="https://github.com/rubiin"><code>@​rubiin</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1708">#1708</a> <code>isISO31661Alpha3</code>: perf <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1711">#1711</a> <code>isDate</code>: allow users to strictly validate dates with <code>.</code> as delimiter <a href="https://github.com/flymans"><code>@​flymans</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1715">#1715</a> <code>isCreditCard</code>: fix for Union Pay cards <a href="https://github.com/shreyassai123"><code>@​shreyassai123</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1718">#1718</a> <code>isEmail</code>: replace all dots in GMail length validation <a href="https://github.com/DasDingGehtNicht"><code>@​DasDingGehtNicht</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1721">#1721</a> <code>isURL</code>: add <code>allow_fragments</code> and <code>allow_query_components</code> <a href="https://github.com/cowboy-bebug"><code>@​cowboy-bebug</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1724">#1724</a> <code>isISO31661Alpha2</code>: perf <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1730">#1730</a> <code>isMagnetURI</code> <a href="https://github.com/tux-tn"><code>@​tux-tn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1738">#1738</a> <code>trim</code>: remove regex to prevent ReDOS attack <a href="https://github.com/tux-tn"><code>@​tux-tn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1747">#1747</a> maintenance: run scripts in parallel for build and clean <a href="https://github.com/sachinraja"><code>@​sachinraja</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1748">#1748</a> <code>isURL</code>: higher priority to <code>whitelist</code> <a href="https://github.com/deepanshu2506"><code>@​deepanshu2506</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1751">#1751</a> <code>isURL</code>: allow url with colon and no port <a href="https://github.com/MatteoPierro"><code>@​MatteoPierro</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1777">#1777</a> <code>isUUID</code>: fix for <code>null</code> version argument <a href="https://github.com/theteladras"><code>@​theteladras</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1799">#1799</a> <code>isFQDN</code>: check more special chars <a href="https://github.com/MatteoPierro"><code>@​MatteoPierro</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1833">#1833</a> <code>isURL</code>: allow URL with an empty user <a href="https://github.com/MiguelSavignano"><code>@​MiguelSavignano</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1835">#1835</a> <code>unescape</code>: fixed bug where intermediate string contains escaped <a href="https://github.com/Marcholio"><code>@​Marcholio</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1836">#1836</a> <code>contains</code>: can check that string contains seed multiple times <a href="https://github.com/Marcholio"><code>@​Marcholio</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1844">#1844</a> docs: add CDN instructions <a href="https://github.com/luiscobits"><code>@​luiscobits</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1848">#1848</a> <code>isUUID</code>: add support for validation of <code>v1</code> and <code>v2</code> <a href="https://github.com/theteladras"><code>@​theteladras</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1641">#1941</a> <code>isEmail</code>: add <code>host_blacklist</code> option <a href="https://github.com/fedeci"><code>@​fedeci</code></a></li>
</ul>
<h2>New and Improved Locales</h2>
<ul>
<li>
<p><code>isAlpha</code>, <code>isAlphanumeric</code>:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1716">#1716</a> <code>hi-IN</code> <a href="https://github.com/MiKr13"><code>@​MiKr13</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1837">#1837</a> <code>fi-FI</code> <a href="https://github.com/Marcholio"><code>@​Marcholio</code></a></li>
</ul>
</li>
<li>
<p><code>isPassportNumber</code>:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1656">#1656</a> <code>ID</code> <a href="https://github.com/rubiin"><code>@​rubiin</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1714">#1714</a> <code>CN</code> <a href="https://github.com/anirudhgiri"><code>@​anirudhgiri</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1809">#1809</a> <code>PL</code> <a href="https://github.com/Ronqn"><code>@​Ronqn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1810">#1810</a> <code>RU</code> <a href="https://github.com/Theta-Dev"><code>@​Theta-Dev</code></a></li>
</ul>
</li>
<li>
<p><code>isPostalCode</code>:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1788">#1788</a> <code>LK</code> <a href="https://github.com/nimanthadilz"><code>@​nimanthadilz</code></a></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/validatorjs/validator.js/blob/master/CHANGELOG.md">validator's changelog</a>.</em></p>
<blockquote>
<h2>13.7.0</h2>
<h3>New Features</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1706">#1706</a> <code>isISO4217</code>, currency code validator <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
</ul>
<h3>New Features</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1706">#1706</a> <code>isISO4217</code>, currency code validator <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
</ul>
<h3>Fixes and Enhancements</h3>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1647">#1647</a> <code>isFQDN</code>: add <code>allow_wildcard</code> option <a href="https://github.com/fasenderos"><code>@​fasenderos</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1654">#1654</a> <code>isRFC3339</code>: Disallow prepended and appended strings to RFC 3339 date-time <a href="https://github.com/jmacmahon"><code>@​jmacmahon</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1658">#1658</a> maintenance: increase code coverage <a href="https://github.com/tux-tn"><code>@​tux-tn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1669">#1669</a> <code>IBAN</code> export list of country codes that implement IBAN <a href="https://github.com/dror-heller"><code>@​dror-heller</code></a> <a href="https://github.com/fedeci"><code>@​fedeci</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1676">#1676</a> <code>isBoolean</code>: add <code>loose</code> option <a href="https://github.com/brybrophy"><code>@​brybrophy</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1697">#1697</a> maintenance: fix npm installation error <a href="https://github.com/rubiin"><code>@​rubiin</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1708">#1708</a> <code>isISO31661Alpha3</code>: perf <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1711">#1711</a> <code>isDate</code>: allow users to strictly validate dates with <code>.</code> as delimiter <a href="https://github.com/flymans"><code>@​flymans</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1715">#1715</a> <code>isCreditCard</code>: fix for Union Pay cards <a href="https://github.com/shreyassai123"><code>@​shreyassai123</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1718">#1718</a> <code>isEmail</code>: replace all dots in GMail length validation <a href="https://github.com/DasDingGehtNicht"><code>@​DasDingGehtNicht</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1721">#1721</a> <code>isURL</code>: add <code>allow_fragments</code> and <code>allow_query_components</code> <a href="https://github.com/cowboy-bebug"><code>@​cowboy-bebug</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1724">#1724</a> <code>isISO31661Alpha2</code>: perf <a href="https://github.com/jpaya17"><code>@​jpaya17</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1730">#1730</a> <code>isMagnetURI</code> <a href="https://github.com/tux-tn"><code>@​tux-tn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1738">#1738</a> <code>rtrim</code>: remove regex to prevent ReDOS attack <a href="https://github.com/tux-tn"><code>@​tux-tn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1747">#1747</a> maintenance: run scripts in parallel for build and clean <a href="https://github.com/sachinraja"><code>@​sachinraja</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1748">#1748</a> <code>isURL</code>: higher priority to <code>whitelist</code> <a href="https://github.com/deepanshu2506"><code>@​deepanshu2506</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1751">#1751</a> <code>isURL</code>: allow url with colon and no port <a href="https://github.com/MatteoPierro"><code>@​MatteoPierro</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1777">#1777</a> <code>isUUID</code>: fix for <code>null</code> version argument <a href="https://github.com/theteladras"><code>@​theteladras</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1799">#1799</a> <code>isFQDN</code>: check more special chars <a href="https://github.com/MatteoPierro"><code>@​MatteoPierro</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1833">#1833</a> <code>isURL</code>: allow URL with an empty user <a href="https://github.com/MiguelSavignano"><code>@​MiguelSavignano</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1835">#1835</a> <code>unescape</code>: fixed bug where intermediate string contains escaped <a href="https://github.com/Marcholio"><code>@​Marcholio</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1836">#1836</a> <code>contains</code>: can check that string contains seed multiple times <a href="https://github.com/Marcholio"><code>@​Marcholio</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1844">#1844</a> docs: add CDN instructions <a href="https://github.com/luiscobits"><code>@​luiscobits</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1848">#1848</a> <code>isUUID</code>: add support for validation of <code>v1</code> and <code>v2</code> <a href="https://github.com/theteladras"><code>@​theteladras</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1641">#1941</a> <code>isEmail</code>: add <code>host_blacklist</code> option <a href="https://github.com/fedeci"><code>@​fedeci</code></a></li>
</ul>
<h3>New and Improved Locales</h3>
<ul>
<li>
<p><code>isAlpha</code>, <code>isAlphanumeric</code>:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1716">#1716</a> <code>hi-IN</code> <a href="https://github.com/MiKr13"><code>@​MiKr13</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1837">#1837</a> <code>fi-FI</code> <a href="https://github.com/Marcholio"><code>@​Marcholio</code></a></li>
</ul>
</li>
<li>
<p><code>isPassportNumber</code>:</p>
<ul>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1656">#1656</a> <code>ID</code> <a href="https://github.com/rubiin"><code>@​rubiin</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1714">#1714</a> <code>CN</code> <a href="https://github.com/anirudhgiri"><code>@​anirudhgiri</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1809">#1809</a> <code>PL</code> <a href="https://github.com/Ronqn"><code>@​Ronqn</code></a></li>
<li><a href="https://github-redirect.dependabot.com/validatorjs/validator.js/pull/1810">#1810</a> <code>RU</code> <a href="https://github.com/Theta-Dev"><code>@​Theta-Dev</code></a></li>
</ul>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/validatorjs/validator.js/commit/47ee5ad64cf5c684c841b59110af4e221b74945c"><code>47ee5ad</code></a> 13.7.0</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/496fc8b2a7f5997acaaec33cc44d0b8dba5fb5e1"><code>496fc8b</code></a> fix(rtrim): remove regex to prevent ReDOS attack (<a href="https://github-redirect.dependabot.com/validatorjs/validator.js/issues/1738">#1738</a>)</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/45901ec4f1276d192da6d0eb10a60b64722356c1"><code>45901ec</code></a> Merge pull request <a href="https://github-redirect.dependabot.com/validatorjs/validator.js/issues/1851">#1851</a> from validatorjs/chore/fix-merge-conflicts</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/83cb7f8cca9e62c26852bc28ba600680751a36f1"><code>83cb7f8</code></a> chore: merge conflict clean-up</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/f17e220b1d8788549d5f9cb80662d001bad7fdbf"><code>f17e220</code></a> feat(isMobilePhone): add El Salvador es-SV locale</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/5b067037996768f032facd5f2aeb89bb20188aa3"><code>5b06703</code></a> feat(isMobilePhone): add Palestine ar-PS locale</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/a3faa8392783aed01d709e4e786ad35e32f743ef"><code>a3faa83</code></a> feat(isMobilePhone): add Botswana en-BW locale</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/26605f9881495a0b6774dcd51833f566c0d6b794"><code>26605f9</code></a> feat(isMobilePhone): add Turkmenistan tk-TM</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/0e5d5d4216885a4aa03a88c3c462e8a96110c378"><code>0e5d5d4</code></a> feat(isMobilePhone): add Guyana en-GY locale</li>
<li><a href="https://github.com/validatorjs/validator.js/commit/f7ff349b0c0429a2c41cc18bc86fc85e9224ab4d"><code>f7ff349</code></a> feat(isMobilePhone): add Frech Polynesia fr-PF locale</li>
<li>Additional commits viewable in <a href="https://github.com/validatorjs/validator.js/compare/13.6.0...13.7.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=validator&package-manager=npm_and_yarn&previous-version=13.6.0&new-version=13.7.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-mobile-agent-react-native/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-28 16:39:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/190" class=".btn">#190</a>
            </td>
            <td>
                <b>
                    Credentials list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

* Adds tests for credentials list scenarios
* Fixes up styling/theming for proof request screen
* Fixes navigation issues when navigating between home and credentials list screens during a credential offer workflow

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 23:22:24 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/189" class=".btn">#189</a>
            </td>
            <td>
                <b>
                    Change status bar style
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Change the status bar style to light content so the text has better contrast.

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 17:54:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/188" class=".btn">#188</a>
            </td>
            <td>
                <b>
                    Settings screen theming
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Pulls theming through the settings and language screens (i.e. styling is applied from a set of global theme settings)

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-27 01:38:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/187" class=".btn">#187</a>
            </td>
            <td>
                <b>
                    Fix theme color
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Fix base theme color.

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 23:02:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/186" class=".btn">#186</a>
            </td>
            <td>
                <b>
                    Style home screen et al
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Pull the color theme through the following screens just enough so they look decent when other color pallets are applied:

- Home
- Credential offer
- Credenza offer accept / reject (ModularView).

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 21:27:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/184" class=".btn">#184</a>
            </td>
            <td>
                <b>
                    Pull theming through scan screen and scanner components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

Pulls theming through the scan screen and scanner components (i.e. styling is applied from a set of global theme settings)

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 18:33:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    Pull theming through contact list and contact list items
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Akiff Manji <akiff.manji@gmail.com>

# Summary of Changes

Pulls theming through the contacts list and contacts list items (i.e. styling is applied from a set of global theme settings)

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-26 18:04:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/181" class=".btn">#181</a>
            </td>
            <td>
                <b>
                    Add alternative dark grey
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Add alternative dark grey, used for text in some cases.

# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 23:53:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/180" class=".btn">#180</a>
            </td>
            <td>
                <b>
                    Fix husky
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Husky, the tool that runs our hooks stopped working for me. I think this should fix it.

# Related Issues

Please reference here any issue #'s that are relevant to this PR, or simply enter "N/A" if this PR does not relate to any existing issues.

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 22:52:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/179" class=".btn">#179</a>
            </td>
            <td>
                <b>
                    Credentials list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

* Applies theme variables through credentials list
* Fixes issue with displaying credential info
  - Updates schema parser helper to capitalize first letters of parsed schema names
  - Adds time issued to credential
* Fixes crash error when tapping to credential details screen

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 01:18:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/178" class=".btn">#178</a>
            </td>
            <td>
                <b>
                    Fix PIN create and enter contrast
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

Because of the original two color pallet it was hard to change the theme and not run into contrast issues with the PIN entry screens. This change just better uses the updated pallet for a more uniform look and allows for more options when changing the color pallet.

I didn't change too much in the way of theme because these screens will be redone as Ontario comes up with a new and better way to use biometrics with a PIN override if not available.

![IMG_5780](https://user-images.githubusercontent.com/390891/151063931-382b3d8c-69cf-4a5b-a681-4171f12dd132.PNG)



# Related Issues

n/a

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [x] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [x] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [x] Run prettier: `npm run style-format`
- [x] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 19:56:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-mobile-agent-react-native/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    Display credential offer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                # Summary of Changes

* Add full notification screen modals and navigation changes for credential offer workflow
  - Modals include a pending, credential received and credential arrived
  - Modal component is generic and reusable
* Refactors some navigation params into exported module
* Adds unit tests for credential offer workflow

# Related Issues

N/A

# Pull Request Checklist

This is just a reminder about the most common mistakes. Please make sure that you tick all _appropriate_ boxes. But please read our [contribution guide](../CONTRIBUTING.md) at least once; it will save you a few review cycles!

If an item doesn't apply to your pull request, **check it anyway** to make it apparent that there's nothing to do.

- [ ] All commits contain a DCO `Signed-off-by` line (we use the [DCO GitHub app](https://github.com/apps/dco) to enforce this).
- [ ] Updated LICENSE-3RD-PARTY.md for any added dependencies or vendored components.
- [ ] Run prettier: `npm run style-format`
- [ ] Updated **documentation** for changed code and new or modified features.

If you have _any_ questions to _any_ of the points above, just **submit and ask**! This checklist is here to _help_ you, not to deter you from contributing!

_PR template adapted from the Python attrs project._

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-24 17:29:53 +0000 UTC
    </div>
</div>

