---
layout: default
title: aries-acapy-plugins
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-plugins
---

# aries-acapy-plugins <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-plugins){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/206" class=".btn">#206</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump nest-asyncio from 1.5.8 to 1.5.9 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [nest-asyncio](https://github.com/erdewit/nest_asyncio) from 1.5.8 to 1.5.9.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/c4b8289fe4f4a3192fd1d501e74df08fd93ed348"><code>c4b8289</code></a> Fix patching an already running Proactor loop, fixes <a href="https://redirect.github.com/erdewit/nest_asyncio/issues/87">#87</a></li>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/d5a13b0d5f156ac9076fbc244f49fb9d48af9bbc"><code>d5a13b0</code></a> Update link to build icon</li>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/a48a68a47e182bd7e1f86c60dfc07d7b8509508b"><code>a48a68a</code></a> Merge pull request <a href="https://redirect.github.com/erdewit/nest_asyncio/issues/84">#84</a> from 5j9/patch-1</li>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/c20e77426bfb9be50d514a850bc4cabbbc69f114"><code>c20e774</code></a> Update README.rst</li>
<li><a href="https://github.com/erdewit/nest_asyncio/commit/f7ce59048cdaace5a1a82c78ef476c3bbb3b664a"><code>f7ce590</code></a> v1.5.8</li>
<li>See full diff in <a href="https://github.com/erdewit/nest_asyncio/compare/v1.5.8...v1.5.9">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=nest-asyncio&package-manager=pip&previous-version=1.5.8&new-version=1.5.9)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:53:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/205" class=".btn">#205</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump mock from 4.0.3 to 5.1.0 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mock](https://github.com/testing-cabal/mock) from 4.0.3 to 5.1.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/testing-cabal/mock/blob/master/CHANGELOG.rst">mock's changelog</a>.</em></p>
<blockquote>
<h2>5.1.0</h2>
<ul>
<li>
<p>bpo-44185: :func:<code>unittest.mock.mock_open</code> will call the :func:<code>close</code>
method of the file handle mock when it is exiting from the context
manager. Patch by Samet Yaslan.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/94924">gh-94924</a>: :func:<code>unittest.mock.create_autospec</code> now properly returns
coroutine functions compatible with :func:<code>inspect.iscoroutinefunction</code></p>
</li>
<li>
<p>bpo-17013: Add <code>ThreadingMock</code> to :mod:<code>unittest.mock</code> that can be used
to create Mock objects that can wait until they are called. Patch by
Karthikeyan Singaravelan and Mario Corchero.</p>
</li>
<li>
<p>bpo-41768: :mod:<code>unittest.mock</code> speccing no longer calls class properties.
Patch by Melanie Witt.</p>
</li>
</ul>
<h2>5.0.2</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/102978">gh-102978</a>: Fixes :func:<code>unittest.mock.patch</code> not enforcing function
signatures for methods decorated with <code>@classmethod</code> or
<code>@staticmethod</code> when patch is called with <code>autospec=True</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/103329">gh-103329</a>: Regression tests for the behaviour of
<code>unittest.mock.PropertyMock</code> were added.</p>
</li>
</ul>
<h2>5.0.1</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/100740">gh-100740</a>: Fix <code>unittest.mock.Mock</code> not respecting the spec for
attribute names prefixed with <code>assert</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/100690">gh-100690</a>: <code>Mock</code> objects which are not unsafe will now raise an
<code>AttributeError</code> when accessing an attribute that matches the name of an
assertion but without the prefix <code>assert_</code>, e.g. accessing
<code>called_once</code> instead of <code>assert_called_once</code>. This is in addition to
this already happening for accessing attributes with prefixes <code>assert</code>,
<code>assret</code>, <code>asert</code>, <code>aseert</code>, and <code>assrt</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/testing-cabal/mock/issues/96127">gh-96127</a>: <code>inspect.signature</code> was raising <code>TypeError</code> on call with
mock objects. Now it correctly returns <code>(*args, **kwargs)</code> as infered
signature.</p>
</li>
</ul>
<h2>5.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/testing-cabal/mock/issues/98624">gh-98624</a>: Add a mutex to unittest.mock.NonCallableMock to protect
concurrent access to mock attributes.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/testing-cabal/mock/commit/d344fa2794b3b1ae7e4a4dbf265fb040d6f41d1f"><code>d344fa2</code></a> Preparing for 5.1.0 release.</li>
<li><a href="https://github.com/testing-cabal/mock/commit/e53a01c315095bac1101fb3545c61382dc0d23fd"><code>e53a01c</code></a> latest sync point</li>
<li><a href="https://github.com/testing-cabal/mock/commit/73343195e09fd20b9a39187a71c138fa13e02f9d"><code>7334319</code></a> Remove unused branches from mock module (<a href="https://redirect.github.com/testing-cabal/mock/issues/106617">#106617</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/f0cc38503e2d91341ca4e263d5acf934b7c0d130"><code>f0cc385</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/61215">GH-61215</a>: threadingmock: Remove unused branch for <code>timeout</code> (<a href="https://redirect.github.com/testing-cabal/mock/issues/106591">#106591</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/acd5fc58e41cd866b4ceff262140bd3304fb127a"><code>acd5fc5</code></a> Python 3.6+ compat</li>
<li><a href="https://github.com/testing-cabal/mock/commit/8d36bf4cc5f86cb7cc0b60d7b9f2c9c5e53f7f37"><code>8d36bf4</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/106300">gh-106300</a>: Improve <code>assertRaises(Exception)</code> usages in tests (<a href="https://redirect.github.com/testing-cabal/mock/issues/106302">GH-106302</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/9cbc589905dbb0f415ab3a995eee48f4906c0418"><code>9cbc589</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/106458">gh-106458</a>: Mark <code>testthreadingmock.py</code> with <code>@requires_working_threading</code> (GH...</li>
<li><a href="https://github.com/testing-cabal/mock/commit/0dc15d43989f7563b442b82e2807819b50b9d726"><code>0dc15d4</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/61215">gh-61215</a>: Rename <code>wait_until_any_call</code> to <code>wait_until_any_call_with</code> (<a href="https://redirect.github.com/testing-cabal/mock/issues/106414">#106414</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/cb8b3c8c8a3f1661f93b989440853b9377a91303"><code>cb8b3c8</code></a> <a href="https://redirect.github.com/testing-cabal/mock/issues/61215">gh-61215</a>: New mock to wait for multi-threaded events to happen (<a href="https://redirect.github.com/testing-cabal/mock/issues/16094">#16094</a>)</li>
<li><a href="https://github.com/testing-cabal/mock/commit/0bd94e622397bb2245a951086adb450731ee5d63"><code>0bd94e6</code></a> bpo-44185: Added close() to mock_open <strong>exit</strong> (<a href="https://redirect.github.com/testing-cabal/mock/issues/26902">#26902</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/testing-cabal/mock/compare/4.0.3...5.1.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mock&package-manager=pip&previous-version=4.0.3&new-version=5.1.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:52:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/204" class=".btn">#204</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump indy-vdr from 0.3.4 to 0.4.1 in /kafka_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [indy-vdr](https://github.com/hyperledger/indy-vdr) from 0.3.4 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/indy-vdr/releases">indy-vdr's releases</a>.</em></p>
<blockquote>
<h2>v0.4.1</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(js): add missing parameters to rn wrapper by <a href="https://github.com/genaris"><code>@​genaris</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/218">hyperledger/indy-vdr#218</a></li>
<li>Update to indy-data-types 0.7; remove indy-utils by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/224">hyperledger/indy-vdr#224</a></li>
<li>fix a typo in logs by <a href="https://github.com/xiaolou86"><code>@​xiaolou86</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/231">hyperledger/indy-vdr#231</a></li>
<li>fix(js): use quotes instead of brackets for local dependencies by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/232">hyperledger/indy-vdr#232</a></li>
<li>fix(js): use universal architecture for darwin by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/233">hyperledger/indy-vdr#233</a></li>
<li>fix(rn): do not try to deserialize again if it is a stream by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/234">hyperledger/indy-vdr#234</a></li>
<li>Faster pool refresh by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/242">hyperledger/indy-vdr#242</a></li>
<li>Add genesis transactions caching by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/243">hyperledger/indy-vdr#243</a></li>
<li>genesis cache js by <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/244">hyperledger/indy-vdr#244</a></li>
<li>Update setup.py by <a href="https://github.com/tnkhanh"><code>@​tnkhanh</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/245">hyperledger/indy-vdr#245</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/xiaolou86"><code>@​xiaolou86</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/231">hyperledger/indy-vdr#231</a></li>
<li><a href="https://github.com/tnkhanh"><code>@​tnkhanh</code></a> made their first contribution in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/245">hyperledger/indy-vdr#245</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/indy-vdr/compare/v0.4.0...v0.4.1">https://github.com/hyperledger/indy-vdr/compare/v0.4.0...v0.4.1</a></p>
<h2>v0.4.0</h2>
<ul>
<li>Added support for <code>did:indy</code> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/166">hyperledger/indy-vdr#166</a>, thanks to <a href="https://github.com/domwoe"><code>@​domwoe</code></a>, <a href="https://github.com/c2bo"><code>@​c2bo</code></a></li>
<li>Added new nodejs and react-native wrappers, thanks to <a href="https://github.com/berendsliedrecht"><code>@​berendsliedrecht</code></a>, <a href="https://github.com/TimoGlastra"><code>@​TimoGlastra</code></a>, <a href="https://github.com/karimStekelenburg"><code>@​karimStekelenburg</code></a>, <a href="https://github.com/genaris"><code>@​genaris</code></a>, <a href="https://github.com/mrlunin"><code>@​mrlunin</code></a></li>
<li>Switched from Ursa (now archived) to <code>indy-blssignatures</code></li>
<li>Added builder for POOL_UPGRADE request into FFI and Python by <a href="https://github.com/Artemkaaas"><code>@​Artemkaaas</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/148">hyperledger/indy-vdr#148</a></li>
<li>Proxy client by <a href="https://github.com/mirgee"><code>@​mirgee</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/184">hyperledger/indy-vdr#184</a></li>
<li>Support HTTPS by <a href="https://github.com/mirgee"><code>@​mirgee</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/187">hyperledger/indy-vdr#187</a></li>
<li>Issue <a href="https://redirect.github.com/hyperledger/indy-vdr/issues/210">#210</a> InvalidClientTaaAcceptanceError time too precise error if container timezone is not UTC by <a href="https://github.com/Ennovate-com"><code>@​Ennovate-com</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/211">hyperledger/indy-vdr#211</a></li>
<li>Fix minor typos by <a href="https://github.com/omahs"><code>@​omahs</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/213">hyperledger/indy-vdr#213</a></li>
<li>Now publishing arm64 packages</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/indy-vdr/compare/v0.3.4...v0.4.0">https://github.com/hyperledger/indy-vdr/compare/v0.3.4...v0.4.0</a></p>
<h2>v0.4.0-dev.16</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(rn): android works with JSC and Hermes by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/194">hyperledger/indy-vdr#194</a></li>
<li>chore: update version by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/195">hyperledger/indy-vdr#195</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/indy-vdr/compare/v0.4.0-dev.15...v0.4.0-dev.16">https://github.com/hyperledger/indy-vdr/compare/v0.4.0-dev.15...v0.4.0-dev.16</a></p>
<h2>v0.4.0-dev.15</h2>
<h2>What's Changed</h2>
<ul>
<li>fix(nodejs): compatible with Windows builds by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/183">hyperledger/indy-vdr#183</a></li>
<li>feat: react native 0.71.x and Expo support by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/186">hyperledger/indy-vdr#186</a></li>
<li>build(android): use custom cross images by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/189">hyperledger/indy-vdr#189</a></li>
<li>chore: update version by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/190">hyperledger/indy-vdr#190</a></li>
<li>build(js): use local network by <a href="https://github.com/blu3beri"><code>@​blu3beri</code></a> in <a href="https://redirect.github.com/hyperledger/indy-vdr/pull/192">hyperledger/indy-vdr#192</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/indy-vdr/compare/v0.4.0-dev.14...v0.4.0-dev.15">https://github.com/hyperledger/indy-vdr/compare/v0.4.0-dev.14...v0.4.0-dev.15</a></p>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/c4b558c2e99a6e0751642056b66511046a5a35ef"><code>c4b558c</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-vdr/issues/247">#247</a> from andrewwhitehead/upd/ver-041</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/0d975070f1caf5274563b327718132dab85328bf"><code>0d97507</code></a> use lockfile when installing cross</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/162a1f34f294f099cd925ec3a6ec02a7074c51c1"><code>162a1f3</code></a> update proxy version to 0.1.5</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/a19834485f8c8bd72511d37f8969cf3278f6f164"><code>a198344</code></a> update python wrapper version to 0.4.1</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/83f3507068b8dcbc78e9cef9681d3f414066da9e"><code>83f3507</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-vdr/issues/245">#245</a> from tnkhanh/patch-1</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/fb2bbbedb68f6a29cbe6dbe04e3cf861054ae35d"><code>fb2bbbe</code></a> Merge branch 'main' into patch-1</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/f70a6d80ff1d2aa53e4cc3f29bfb0bd452dd3e09"><code>f70a6d8</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-vdr/issues/244">#244</a> from berendsliedrecht/genesis-cache-js</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/9695a179160be3178cc2cb6b39470faedd97f317"><code>9695a17</code></a> Merge branch 'main' into genesis-cache-js</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/a914ef401ed7258c14a89365deb1c5a32dc5d1d5"><code>a914ef4</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-vdr/issues/243">#243</a> from andrewwhitehead/feat/genesis-cache</li>
<li><a href="https://github.com/hyperledger/indy-vdr/commit/cc7e2bb4ddae1fe8f6a4bbcf17c4c20a8fedd362"><code>cc7e2bb</code></a> Update setup.py</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/indy-vdr/compare/v0.3.4...v0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=indy-vdr&package-manager=pip&previous-version=0.3.4&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:51:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/203" class=".btn">#203</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-asyncio from 0.14.0 to 0.23.5 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) from 0.14.0 to 0.23.5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.5</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.5a0</h2>
<h1>0.23.5 (UNRELEASED)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4</h2>
<h1>0.23.4 (2024-01-28)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
<li>Declares incompatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
</ul>
<h2>pytest-asyncio 0.23.4a2</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
<li>Addresses further issues that caused an internal pytest error during test collection</li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4a1</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.4a0</h2>
<h1>0.23.4 (UNRELEASED)</h1>
<ul>
<li>pytest-asyncio no longer imports additional, unrelated packages during test collection <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/729">#729</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
<h2>pytest-asyncio 0.23.3</h2>
<h1>0.23.3 (2024-01-01)</h1>
<ul>
<li>Fixes a bug that caused event loops to be closed prematurely when using async generator fixtures with class scope or wider in a function-scoped test <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3aef60532f2a1c634af5f4539eabdd4fbfffcabc"><code>3aef605</code></a> [build] Update actions/upload-artifact and actions/download-artifact to v4.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4b1908d9ed26895c194a4bb8d4c61cef2dfc5067"><code>4b1908d</code></a> [fix] Prevent DeprecationWarning from bubbling to user code.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/fc6d6cfeb2fd7db1572869b80517ec436ef95e7f"><code>fc6d6cf</code></a> Fix typing and update to mypy 1.8.0 (<a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6008cf16e2a5c6c365e249db975a8a1afec3c8bf"><code>6008cf1</code></a> Build(deps): Bump pluggy from 1.3.0 to 1.4.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/712c51bde9d385ecf69ee98e8c40fa6868b80a75"><code>712c51b</code></a> Build(deps): Bump coverage from 7.4.0 to 7.4.1 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/42fd3041c3e44e3428adee10afa7935757375ff9"><code>42fd304</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a40b4f662454e3b33d44fc552958439db167a294"><code>a40b4f6</code></a> Build(deps): Bump urllib3 from 2.1.0 to 2.2.0 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/9d90f8ec6e68e2564f5116cf2accfe0b202af390"><code>9d90f8e</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/fe5da0771dcc0b939ae9ee3d1b9a50cfc4860667"><code>fe5da07</code></a> Build(deps): Bump markupsafe from 2.1.4 to 2.1.5 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/42b140decf8de145e76dcd61894a7963b10e815b"><code>42b140d</code></a> fix compatibility with pytest ^8 (<a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/776">#776</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-asyncio&package-manager=pip&previous-version=0.14.0&new-version=0.23.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:51:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/202" class=".btn">#202</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update pytest requirement from ~7.4.0 to ~8.1.0 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest](https://github.com/pytest-dev/pytest) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.1.0</h2>
<h1>pytest 8.1.0 (2024-03-03)</h1>
<h2>Features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11475">#11475</a>: Added the new <code>consider_namespace_packages</code>{.interpreted-text role=&quot;confval&quot;} configuration option, defaulting to <code>False</code>.</p>
<p>If set to <code>True</code>, pytest will attempt to identify modules that are part of <a href="https://packaging.python.org/en/latest/guides/packaging-namespace-packages">namespace packages</a> when importing modules.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11653">#11653</a>: Added the new <code>verbosity_test_cases</code>{.interpreted-text role=&quot;confval&quot;} configuration option for fine-grained control of test execution verbosity.
See <code>Fine-grained verbosity &lt;pytest.fine_grained_verbosity&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more details.</p>
</li>
</ul>
<h2>Improvements</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/10865">#10865</a>: <code>pytest.warns</code>{.interpreted-text role=&quot;func&quot;} now validates that <code>warnings.warn</code>{.interpreted-text role=&quot;func&quot;} was called with a [str]{.title-ref} or a [Warning]{.title-ref}.
Currently in Python it is possible to use other types, however this causes an exception when <code>warnings.filterwarnings</code>{.interpreted-text role=&quot;func&quot;} is used to filter those warnings (see [CPython <a href="https://redirect.github.com/pytest-dev/pytest/issues/103577">#103577</a>](<a href="https://redirect.github.com/python/cpython/issues/103577">python/cpython#103577</a>) for a discussion).
While this can be considered a bug in CPython, we decided to put guards in pytest as the error message produced without this check in place is confusing.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11311">#11311</a>: When using <code>--override-ini</code> for paths in invocations without a configuration file defined, the current working directory is used
as the relative directory.</p>
<p>Previoulsy this would raise an <code>AssertionError</code>{.interpreted-text role=&quot;class&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11475">#11475</a>: <code>--import-mode=importlib &lt;import-mode-importlib&gt;</code>{.interpreted-text role=&quot;ref&quot;} now tries to import modules using the standard import mechanism (but still without changing :py<code>sys.path</code>{.interpreted-text role=&quot;data&quot;}), falling back to importing modules directly only if that fails.</p>
<p>This means that installed packages will be imported under their canonical name if possible first, for example <code>app.core.models</code>, instead of having the module name always be derived from their path (for example <code>.env310.lib.site_packages.app.core.models</code>).</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11801">#11801</a>: Added the <code>iter_parents() &lt;_pytest.nodes.Node.iter_parents&gt;</code>{.interpreted-text role=&quot;func&quot;} helper method on nodes.
It is similar to <code>listchain &lt;_pytest.nodes.Node.listchain&gt;</code>{.interpreted-text role=&quot;func&quot;}, but goes from bottom to top, and returns an iterator, not a list.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11850">#11850</a>: Added support for <code>sys.last_exc</code>{.interpreted-text role=&quot;data&quot;} for post-mortem debugging on Python&gt;=3.12.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11962">#11962</a>: In case no other suitable candidates for configuration file are found, a <code>pyproject.toml</code> (even without a <code>[tool.pytest.ini_options]</code> table) will be considered as the configuration file and define the <code>rootdir</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11978">#11978</a>: Add <code>--log-file-mode</code> option to the logging plugin, enabling appending to log-files. This option accepts either <code>&quot;w&quot;</code> or <code>&quot;a&quot;</code> and defaults to <code>&quot;w&quot;</code>.</p>
<p>Previously, the mode was hard-coded to be <code>&quot;w&quot;</code> which truncates the file before logging.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/12047">#12047</a>: When multiple finalizers of a fixture raise an exception, now all exceptions are reported as an exception group.
Previously, only the first exception was reported.</p>
</li>
</ul>
<h2>Bug Fixes</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11904">#11904</a>: Fixed a regression in pytest 8.0.0 that would cause test collection to fail due to permission errors when using <code>--pyargs</code>.</p>
<p>This change improves the collection tree for tests specified using <code>--pyargs</code>, see <code>12043</code>{.interpreted-text role=&quot;pull&quot;} for a comparison with pytest 8.0 and &lt;8.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/b9a167f9bbbd6eda4f0360c5bf5b7f5af50f2bc4"><code>b9a167f</code></a> Prepare release version 8.1.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/00043f7f1047b29fdaeb18e169fe9d6146988cb8"><code>00043f7</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12038">#12038</a> from bluetech/fixtures-rm-arg2index</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f4e10251a4a003495b5228cea421d4de5fa0ce89"><code>f4e1025</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12048">#12048</a> from bluetech/fixture-teardown-excgroup</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/43492f5707b38dab9b62dfb829bb41a13579629f"><code>43492f5</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12051">#12051</a> from jakkdl/test_debugging_pythonbreakpoint</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/82fe28dae4eec900123175cee87245f37b964e5c"><code>82fe28d</code></a> [automated] Update plugin list (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12049">#12049</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/5e2ee7175c145f84ff9882be9496abb56e6e56f2"><code>5e2ee71</code></a> monkeypatch.delenv PYTHONBREAKPOINT in two tests that previously failed/skipped</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/89ee4493ccbcd118349082cd78eb52a761683120"><code>89ee449</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/11997">#11997</a> from nicoddemus/11475-importlib</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/8248946a552635f5751a58c7a6dfd24e98db7404"><code>8248946</code></a> Do not collect symlinked tests under Windows (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12050">#12050</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/434282e17f5f1f4fcc1464a0a0921cf19804bdd7"><code>434282e</code></a> fixtures: use exception group when multiple finalizers raise in fixture teardown</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/d6134bc21e27efee7a2e264bd089e6c223515904"><code>d6134bc</code></a> doc: document consider_namespace_packages option</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/7.4.0...8.1.0">compare view</a></li>
</ul>
</details>
<br />


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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:51:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/201" class=".btn">#201</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update pytest-ruff requirement from ^0.1.1 to ^0.3 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest-ruff](https://github.com/businho/pytest-ruff) to permit the latest version.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/2098829cfb8f95c2885c6dec3e229ed3092e2c1e"><code>2098829</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/8">#8</a> from skellys/fix/fix_v0_2</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/3e0cfef09777aff7411aad2bf50f89b8b4a72a62"><code>3e0cfef</code></a> Fix tests</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/55fe6eebaac0218374eddca721c7ece7a8711eba"><code>55fe6ee</code></a> fix: ruff formatting</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1d5e95fb066b6fc48352dfdc03f3ee7bf76b17fd"><code>1d5e95f</code></a> fix: remove debug stmts</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/82597a2bf91d0b05c977b89dec1a69e32f8bbdb4"><code>82597a2</code></a> fix: pytest --ruff and --ruff-format don't work at the command line</li>
<li>Additional commits viewable in <a href="https://github.com/businho/pytest-ruff/compare/v0.1.1...v0.3">compare view</a></li>
</ul>
</details>
<br />


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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:51:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/200" class=".btn">#200</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump pydantic from 1.10.13 to 1.10.14 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pydantic](https://github.com/pydantic/pydantic) from 1.10.13 to 1.10.14.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/releases">pydantic's releases</a>.</em></p>
<blockquote>
<h2>v1.10.14 2024-01-19</h2>
<h2>What's Changed</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7690">pydantic/pydantic#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/7740">pydantic/pydantic#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8540">pydantic/pydantic#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/pull/8587">pydantic/pydantic#8587</a></li>
<li>Fix <code>cached_property</code> handling in dataclasses when copied by <a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/pull/8407">pydantic/pydantic#8407</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> made their first contribution in <a href="https://redirect.github.com/pydantic/pydantic/pull/8407">pydantic/pydantic#8407</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14">https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pydantic/pydantic/blob/main/HISTORY.md">pydantic's changelog</a>.</em></p>
<blockquote>
<h2>v1.10.14 (2024-01-19)</h2>
<ul>
<li>Update install.md by <a href="https://github.com/dmontagu"><code>@​dmontagu</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/7690">#7690</a></li>
<li>Fix ci to only deploy docs on release by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/7740">#7740</a></li>
<li>Ubuntu fixes for V1 by <a href="https://github.com/sydney-runkle"><code>@​sydney-runkle</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/8540">#8540</a> and <a href="https://redirect.github.com/pydantic/pydantic/issues/8587">#8587</a></li>
<li>Fix cached_property handling in dataclasses when copied by <a href="https://github.com/rdbisme"><code>@​rdbisme</code></a> in <a href="https://redirect.github.com/pydantic/pydantic/issues/8407">#8407</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pydantic/pydantic/commit/3ddb509786089f9df0658303545ae4b66db2d47c"><code>3ddb509</code></a> Prep for 1.10.14 release (<a href="https://redirect.github.com/pydantic/pydantic/issues/8588">#8588</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/c6fc582ee9fc76acb64cbc0a5a55d0c5c8590205"><code>c6fc582</code></a> Minor tweak to V1 docs url fix (<a href="https://redirect.github.com/pydantic/pydantic/issues/8587">#8587</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/f0766c0e6028f9868e131208387549e3897b02bd"><code>f0766c0</code></a> Fix cached_property handling in dataclasses when copied in V1(<a href="https://redirect.github.com/pydantic/pydantic/issues/8407">#8407</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/4e290ab604cdc0579a447ee1736f1b6763f49812"><code>4e290ab</code></a> Ubuntu fixes for V1 (<a href="https://redirect.github.com/pydantic/pydantic/issues/8540">#8540</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/2e939dc3bfb88f54efb66f8f1a031ff22e4f9865"><code>2e939dc</code></a> Update v1 fixes ci to only deploy docs on release (<a href="https://redirect.github.com/pydantic/pydantic/issues/7740">#7740</a>)</li>
<li><a href="https://github.com/pydantic/pydantic/commit/ae53c9d9b3c083c529b9f6d5b2ea0718545e15d1"><code>ae53c9d</code></a> Update install.md (<a href="https://redirect.github.com/pydantic/pydantic/issues/7690">#7690</a>)</li>
<li>See full diff in <a href="https://github.com/pydantic/pydantic/compare/v1.10.13...v1.10.14">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pydantic&package-manager=pip&previous-version=1.10.13&new-version=1.10.14)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:50:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/199" class=".btn">#199</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Update pytest-asyncio requirement from 0.14.0 to 0.23.5 in /plugin_globals
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Updates the requirements on [pytest-asyncio](https://github.com/pytest-dev/pytest-asyncio) to permit the latest version.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest-asyncio/releases">pytest-asyncio's releases</a>.</em></p>
<blockquote>
<h2>pytest-asyncio 0.23.5</h2>
<h1>0.23.5 (2024-02-09)</h1>
<ul>
<li>Declare compatibility with pytest 8 <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/737">#737</a></li>
<li>Fix typing errors with recent versions of mypy <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a></li>
<li>Prevent DeprecationWarning about internal use of <code>asyncio.get_event_loop()</code> from affecting test cases <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/757">#757</a></li>
</ul>
<h2>Known issues</h2>
<p>As of v0.23, pytest-asyncio attaches an asyncio event loop to each item of the test suite (i.e. session, packages, modules, classes, functions) and allows tests to be run in those loops when marked accordingly. Pytest-asyncio currently assumes that async fixture scope is correlated with the new event loop scope. This prevents fixtures from being evaluated independently from the event loop scope and breaks some existing test suites (see <a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/706">#706</a>). For example, a test suite may require all fixtures and tests to run in the same event loop, but have async fixtures that are set up and torn down for each module. If you're affected by this issue, please continue using the v0.21 release, until it is resolved.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/3aef60532f2a1c634af5f4539eabdd4fbfffcabc"><code>3aef605</code></a> [build] Update actions/upload-artifact and actions/download-artifact to v4.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/4b1908d9ed26895c194a4bb8d4c61cef2dfc5067"><code>4b1908d</code></a> [fix] Prevent DeprecationWarning from bubbling to user code.</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/fc6d6cfeb2fd7db1572869b80517ec436ef95e7f"><code>fc6d6cf</code></a> Fix typing and update to mypy 1.8.0 (<a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/769">#769</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/6008cf16e2a5c6c365e249db975a8a1afec3c8bf"><code>6008cf1</code></a> Build(deps): Bump pluggy from 1.3.0 to 1.4.0 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/712c51bde9d385ecf69ee98e8c40fa6868b80a75"><code>712c51b</code></a> Build(deps): Bump coverage from 7.4.0 to 7.4.1 in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/42fd3041c3e44e3428adee10afa7935757375ff9"><code>42fd304</code></a> Build(deps): Bump hypothesis in /dependencies/default</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/a40b4f662454e3b33d44fc552958439db167a294"><code>a40b4f6</code></a> Build(deps): Bump urllib3 from 2.1.0 to 2.2.0 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/9d90f8ec6e68e2564f5116cf2accfe0b202af390"><code>9d90f8e</code></a> Build(deps): Bump certifi in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/fe5da0771dcc0b939ae9ee3d1b9a50cfc4860667"><code>fe5da07</code></a> Build(deps): Bump markupsafe from 2.1.4 to 2.1.5 in /dependencies/docs</li>
<li><a href="https://github.com/pytest-dev/pytest-asyncio/commit/42b140decf8de145e76dcd61894a7963b10e815b"><code>42b140d</code></a> fix compatibility with pytest ^8 (<a href="https://redirect.github.com/pytest-dev/pytest-asyncio/issues/776">#776</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest-asyncio/compare/v0.14.0...v0.23.5">compare view</a></li>
</ul>
</details>
<br />


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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:50:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/197" class=".btn">#197</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump rope from 0.19.0 to 1.12.0 in /redis_events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [rope](https://github.com/python-rope/rope) from 0.19.0 to 1.12.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/python-rope/rope/releases">rope's releases</a>.</em></p>
<blockquote>
<h2>1.12.0</h2>
<p>What's changed</p>
<p>Date: 2024-01-18</p>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/733">#733</a> skip directories with perm error when building autoimport index (<a href="https://github.com/MrBago"><code>@​MrBago</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/722">#722</a>, <a href="https://redirect.github.com/python-rope/rope/issues/723">#723</a> Remove site-packages from packages search tree (<a href="https://github.com/tkrabel"><code>@​tkrabel</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/738">#738</a> Implement os.PathLike on Resource (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/739">#739</a>, <a href="https://redirect.github.com/python-rope/rope/issues/736">#736</a> Ensure autoimport requests uses indexes (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/734">#734</a>, <a href="https://redirect.github.com/python-rope/rope/issues/735">#735</a> raise exception when extracting the start of a block without the end</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/MrBago"><code>@​MrBago</code></a> made their first contribution in <a href="https://redirect.github.com/python-rope/rope/pull/733">python-rope/rope#733</a></li>
<li><a href="https://github.com/raymyers"><code>@​raymyers</code></a> made their first contribution in <a href="https://redirect.github.com/python-rope/rope/pull/735">python-rope/rope#735</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/python-rope/rope/compare/1.11.0...1.12.0">https://github.com/python-rope/rope/compare/1.11.0...1.12.0</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python-rope/rope/blob/master/CHANGELOG.md">rope's changelog</a>.</em></p>
<blockquote>
<h1>Release 1.12.0</h1>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/733">#733</a> skip directories with perm error when building autoimport index (<a href="https://github.com/MrBago"><code>@​MrBago</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/722">#722</a>, <a href="https://redirect.github.com/python-rope/rope/issues/723">#723</a> Remove site-packages from packages search tree (<a href="https://github.com/tkrabel"><code>@​tkrabel</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/738">#738</a> Implement os.PathLike on Resource (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/739">#739</a>, <a href="https://redirect.github.com/python-rope/rope/issues/736">#736</a> Ensure autoimport requests uses indexes (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/734">#734</a>, <a href="https://redirect.github.com/python-rope/rope/issues/735">#735</a> raise exception when extracting the start of a block without the end</li>
</ul>
<h1>Release 1.11.0</h1>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/710">#710</a>, <a href="https://redirect.github.com/python-rope/rope/issues/561">#561</a> Implement <code>except*</code> syntax (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/711">#711</a> allow building documentation without having rope module installed (<a href="https://github.com/kloczek"><code>@​kloczek</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/719">#719</a> Allows the in-memory db to be shared across threads (<a href="https://github.com/tkrabel"><code>@​tkrabel</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/720">#720</a> create one sqlite3.Connection per thread using a thread local (<a href="https://github.com/tkrabel"><code>@​tkrabel</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/715">#715</a> change AutoImport's <code>get_modules</code> to be case sensitive (<a href="https://github.com/bagel897"><code>@​bagel897</code></a>)</li>
</ul>
<h1>Release 1.10.0</h1>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/708">#708</a>, <a href="https://redirect.github.com/python-rope/rope/issues/709">#709</a> Add support for Python 3.12 (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
</ul>
<h1>Release 1.9.0</h1>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/624">#624</a>, <a href="https://redirect.github.com/python-rope/rope/issues/693">#693</a> Implement <code>nonlocal</code> keyword (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/697">#697</a>, <a href="https://redirect.github.com/python-rope/rope/issues/565">#565</a> Automatically purge autoimport.db when there is schema change</li>
</ul>
<h1>Release 1.8.0</h1>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/650">#650</a> Install pre-commit hooks on rope repository (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/655">#655</a> Remove unused <strong>init</strong>() methods (<a href="https://github.com/edreamleo"><code>@​edreamleo</code></a>, <a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/656">#656</a> Reformat using black 23.1.0 (<a href="https://github.com/edreamleo"><code>@​edreamleo</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/674">#674</a> Fix/supress all mypy complaints (<a href="https://github.com/edreamleo"><code>@​edreamleo</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/680">#680</a> Remove a do-nothing statement in soi._handle_first_parameter (<a href="https://github.com/edreamleo"><code>@​edreamleo</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/687">#687</a>, <a href="https://redirect.github.com/python-rope/rope/issues/688">#688</a> Fix autoimport not scanning packages recursively (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
</ul>
<h1>Release 1.7.0</h1>
<h2>Feature</h2>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/548">#548</a> Implement MoveGlobal using string as destination module names (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
</ul>
<h2>Bug</h2>
<ul>
<li><a href="https://redirect.github.com/python-rope/rope/issues/627">#627</a> Fix parsing of octal literal (<a href="https://github.com/lieryan"><code>@​lieryan</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/643">#643</a>, <a href="https://redirect.github.com/python-rope/rope/issues/435">#435</a> Fix fstrings with mismatched parens (<a href="https://github.com/apmorton"><code>@​apmorton</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/646">#646</a> Fix renaming kwargs when refactoring from imports (<a href="https://github.com/apmorton"><code>@​apmorton</code></a>)</li>
<li><a href="https://redirect.github.com/python-rope/rope/issues/648">#648</a> Remove <strong>init</strong> from import statement when using sqlite autoimport (<a href="https://github.com/bagel897"><code>@​bagel897</code></a>)</li>
</ul>
<h2>Improvements</h2>
<ul>
<li>rope.contrib.generate improvements</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python-rope/rope/commit/faddd3a4ff9c1ffe34d471b5818c45d546b072f1"><code>faddd3a</code></a> Bump version number</li>
<li><a href="https://github.com/python-rope/rope/commit/b67a5caea70a1611ac4d8c5f2bb685603a8d1ed1"><code>b67a5ca</code></a> Update CHANGELOG.md</li>
<li><a href="https://github.com/python-rope/rope/commit/09753b14321e72c97fa18af4a004757b04029eca"><code>09753b1</code></a> Merge pull request <a href="https://redirect.github.com/python-rope/rope/issues/741">#741</a> from python-rope/all-contributors/add-raymyers</li>
<li><a href="https://github.com/python-rope/rope/commit/3688d324130f21e24f960e469099a5d27c2df571"><code>3688d32</code></a> update .all-contributorsrc [skip ci]</li>
<li><a href="https://github.com/python-rope/rope/commit/7241872a873b700b2ac52864b8e90ca4d6a6a59e"><code>7241872</code></a> update CONTRIBUTORS.md [skip ci]</li>
<li><a href="https://github.com/python-rope/rope/commit/ffc8551588aa76ab82c9b91e714db6a1d94607f5"><code>ffc8551</code></a> Merge pull request <a href="https://redirect.github.com/python-rope/rope/issues/735">#735</a> from raymyers/extract-incomplete-block</li>
<li><a href="https://github.com/python-rope/rope/commit/9cb3031e114dbb1d8ce9219988930bae6879eb98"><code>9cb3031</code></a> Use AST visitor for extract incomplete block check</li>
<li><a href="https://github.com/python-rope/rope/commit/f4fc0cdb1eb39f5a137477a4bba7287faaa6c4c2"><code>f4fc0cd</code></a> Add more tests around extract indentation</li>
<li><a href="https://github.com/python-rope/rope/commit/7ebf247970f743eb5090a4928167226998e2c70f"><code>7ebf247</code></a> Add error handling for extract of incomplete block</li>
<li><a href="https://github.com/python-rope/rope/commit/95585e86fee0c972b2c4dd71c3010100405ed007"><code>95585e8</code></a> Merge pull request <a href="https://redirect.github.com/python-rope/rope/issues/739">#739</a> from python-rope/fix-autoimport-nocase-index</li>
<li>Additional commits viewable in <a href="https://github.com/python-rope/rope/compare/0.19.0...1.12.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=rope&package-manager=pip&previous-version=0.19.0&new-version=1.12.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:49:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/195" class=".btn">#195</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.2.1 to 0.3 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.2.1 to 0.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.2.1...v0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.2.1&new-version=0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:44:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/194" class=".btn">#194</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump black from 23.7.0 to 24.2.0 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 23.7.0 to 24.2.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.2.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fixed a bug where comments where mistakenly removed along with redundant parentheses
(<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li>Move the <code>hug_parens_with_braces_and_square_brackets</code> feature to the unstable style
due to an outstanding crash and proposed formatting tweaks (<a href="https://redirect.github.com/psf/black/issues/4198">#4198</a>)</li>
<li>Fixed a bug where base expressions caused inconsistent formatting of ** in tenary
expression (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li>Checking for newline before adding one on docstring that is almost at the line limit
(<a href="https://redirect.github.com/psf/black/issues/4185">#4185</a>)</li>
<li>Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>).</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Fix issue where <em>Black</em> would ignore input files in the presence of symlinks (<a href="https://redirect.github.com/psf/black/issues/4222">#4222</a>)</li>
<li><em>Black</em> now ignores <code>pyproject.toml</code> that is missing a <code>tool.black</code> section when
discovering project root and configuration. Since <em>Black</em> continues to use version
control as an indicator of project root, this is expected to primarily change behavior
for users in a monorepo setup (desirably). If you wish to preserve previous behavior,
simply add an empty <code>[tool.black]</code> to the previously discovered <code>pyproject.toml</code>
(<a href="https://redirect.github.com/psf/black/issues/4204">#4204</a>)</li>
</ul>
<h3>Output</h3>
<ul>
<li>Black will swallow any <code>SyntaxWarning</code>s or <code>DeprecationWarning</code>s produced by the <code>ast</code>
module when performing equivalence checks (<a href="https://redirect.github.com/psf/black/issues/4189">#4189</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a JSONSchema and provide a validate-pyproject entry-point (<a href="https://redirect.github.com/psf/black/issues/4181">#4181</a>)</li>
</ul>
<h2>24.1.1</h2>
<p>Bugfix release to fix a bug that made Black unusable on certain file systems
with strict limits on path length.</p>
<h3>Preview style</h3>
<ul>
<li>Consistently add trailing comma on typed parameters (<a href="https://redirect.github.com/psf/black/issues/4164">#4164</a>)</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Shorten the length of the name of the cache file to fix crashes on file systems that
do not support long paths (<a href="https://redirect.github.com/psf/black/issues/4176">#4176</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.2.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fixed a bug where comments where mistakenly removed along with redundant parentheses
(<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li>Move the <code>hug_parens_with_braces_and_square_brackets</code> feature to the unstable style
due to an outstanding crash and proposed formatting tweaks (<a href="https://redirect.github.com/psf/black/issues/4198">#4198</a>)</li>
<li>Fixed a bug where base expressions caused inconsistent formatting of ** in tenary
expression (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li>Checking for newline before adding one on docstring that is almost at the line limit
(<a href="https://redirect.github.com/psf/black/issues/4185">#4185</a>)</li>
<li>Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>).</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Fix issue where <em>Black</em> would ignore input files in the presence of symlinks (<a href="https://redirect.github.com/psf/black/issues/4222">#4222</a>)</li>
<li><em>Black</em> now ignores <code>pyproject.toml</code> that is missing a <code>tool.black</code> section when
discovering project root and configuration. Since <em>Black</em> continues to use version
control as an indicator of project root, this is expected to primarily change behavior
for users in a monorepo setup (desirably). If you wish to preserve previous behavior,
simply add an empty <code>[tool.black]</code> to the previously discovered <code>pyproject.toml</code>
(<a href="https://redirect.github.com/psf/black/issues/4204">#4204</a>)</li>
</ul>
<h3>Output</h3>
<ul>
<li>Black will swallow any <code>SyntaxWarning</code>s or <code>DeprecationWarning</code>s produced by the <code>ast</code>
module when performing equivalence checks (<a href="https://redirect.github.com/psf/black/issues/4189">#4189</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a JSONSchema and provide a validate-pyproject entry-point (<a href="https://redirect.github.com/psf/black/issues/4181">#4181</a>)</li>
</ul>
<h2>24.1.1</h2>
<p>Bugfix release to fix a bug that made Black unusable on certain file systems with strict
limits on path length.</p>
<h3>Preview style</h3>
<ul>
<li>Consistently add trailing comma on typed parameters (<a href="https://redirect.github.com/psf/black/issues/4164">#4164</a>)</li>
</ul>
<h3>Configuration</h3>
<ul>
<li>Shorten the length of the name of the cache file to fix crashes on file systems that
do not support long paths (<a href="https://redirect.github.com/psf/black/issues/4176">#4176</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/6fdf8a4af28071ed1d079c01122b34c5d587207a"><code>6fdf8a4</code></a> Prepare release 24.2.0 (<a href="https://redirect.github.com/psf/black/issues/4226">#4226</a>)</li>
<li><a href="https://github.com/psf/black/commit/8af439407c051d55f3221cc93795d20bd9af49c9"><code>8af4394</code></a> fix: Don't remove comments along with parens (<a href="https://redirect.github.com/psf/black/issues/4218">#4218</a>)</li>
<li><a href="https://github.com/psf/black/commit/35e97769190d8c8fe94d9ea2d70d7d88b22a2642"><code>35e9776</code></a> Bump pre-commit/action from 3.0.0 to 3.0.1 (<a href="https://redirect.github.com/psf/black/issues/4225">#4225</a>)</li>
<li><a href="https://github.com/psf/black/commit/23dfc5b2c3b0694a8c27e58e28439591976aaf94"><code>23dfc5b</code></a> Fix ignoring input files for symlink reasons (<a href="https://redirect.github.com/psf/black/issues/4222">#4222</a>)</li>
<li><a href="https://github.com/psf/black/commit/a20100395cf6179a81289452efad1d8e72b19682"><code>a201003</code></a> Simplify check for symlinks that resolve outside root (<a href="https://redirect.github.com/psf/black/issues/4221">#4221</a>)</li>
<li><a href="https://github.com/psf/black/commit/dab37a6a1117d690d683121edc4d7c8fb8dd75a7"><code>dab37a6</code></a> Remove redundant parentheses in <code>case</code> statement <code>if</code> guards (<a href="https://redirect.github.com/psf/black/issues/4214">#4214</a>)</li>
<li><a href="https://github.com/psf/black/commit/32230e6f5c4bc6bb5c469451e15f3f54d9884b51"><code>32230e6</code></a> fix: bug where the doublestar operation had inconsistent formatting. (<a href="https://redirect.github.com/psf/black/issues/4154">#4154</a>)</li>
<li><a href="https://github.com/psf/black/commit/7edb50f5a0afc56bb648dc14640ced144366b43a"><code>7edb50f</code></a> fix: additional newline added to docstring when the previous line length is l...</li>
<li><a href="https://github.com/psf/black/commit/3e80de3447dee272e9977ab58b1560a669b7b848"><code>3e80de3</code></a> Bump furo from 2023.9.10 to 2024.1.29 in /docs (<a href="https://redirect.github.com/psf/black/issues/4211">#4211</a>)</li>
<li><a href="https://github.com/psf/black/commit/a08b480a2f39fb4fc7b210d8b450e33d3879f77d"><code>a08b480</code></a> Bump pypa/cibuildwheel from 2.16.4 to 2.16.5 (<a href="https://redirect.github.com/psf/black/issues/4212">#4212</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/23.7.0...24.2.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=23.7.0&new-version=24.2.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:43:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/192" class=".btn">#192</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump indy-credx from 1.0.3 to 1.1.1 in /basicmessage_storage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [indy-credx](https://github.com/hyperledger/indy-shared-rs) from 1.0.3 to 1.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/hyperledger/indy-shared-rs/releases">indy-credx's releases</a>.</em></p>
<blockquote>
<h2>v1.1.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Avoid stripping leading zeros from non-integer encoded attribute by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/indy-shared-rs/pull/43">hyperledger/indy-shared-rs#43</a></li>
<li>Update anoncreds-clsignatures minimum version by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/indy-shared-rs/pull/44">hyperledger/indy-shared-rs#44</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/indy-shared-rs/compare/v1.1.0...v1.1.1">https://github.com/hyperledger/indy-shared-rs/compare/v1.1.0...v1.1.1</a></p>
<h2>v1.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update dalek dependencies &amp; refactor by <a href="https://github.com/andrewwhitehead"><code>@​andrewwhitehead</code></a> in <a href="https://redirect.github.com/hyperledger/indy-shared-rs/pull/40">hyperledger/indy-shared-rs#40</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/hyperledger/indy-shared-rs/compare/v1.0.3...v1.1.0">https://github.com/hyperledger/indy-shared-rs/compare/v1.0.3...v1.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/d07500fcd6c67975da0bb9637fff10c1a40d0afe"><code>d07500f</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-shared-rs/issues/44">#44</a> from andrewwhitehead/upd/clsig-024</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/7d669010227789f204ad9357778eb8222dde144d"><code>7d66901</code></a> update anoncreds-clsignatures minimum version</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/84bb89ee62a1e2cb15d66e01cb3e361266257e67"><code>84bb89e</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-shared-rs/issues/43">#43</a> from andrewwhitehead/fix/zero-encode</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/6aa61b2073422e06e98b20640ec79627545f9c6f"><code>6aa61b2</code></a> handle negative integer; restrict to i32 range</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/5b3aa2c22e942a62b3ffecd2fee3780e04b58215"><code>5b3aa2c</code></a> avoid stripping leading zero from non-integer attribute</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/0260b93f76573613cedb486bc8836c75c47d4cf4"><code>0260b93</code></a> update python wrapper version</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/512336630333b36e578b702e78ee350e088b7930"><code>5123366</code></a> Merge pull request <a href="https://redirect.github.com/hyperledger/indy-shared-rs/issues/40">#40</a> from andrewwhitehead/upd/dalek2</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/684cafa10c8252585477095330bc1d372f66333e"><code>684cafa</code></a> manually clamp x25519 scalar for consistency with old version</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/bff120c85c7e1d304ccc7683dc671a160fdf65be"><code>bff120c</code></a> remove test from workflow</li>
<li><a href="https://github.com/hyperledger/indy-shared-rs/commit/733682397763dee048b817caa1544f0421e37822"><code>7336823</code></a> enable zeroize for dalek crates</li>
<li>Additional commits viewable in <a href="https://github.com/hyperledger/indy-shared-rs/compare/v1.0.3...v1.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=indy-credx&package-manager=pip&previous-version=1.0.3&new-version=1.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:41:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/189" class=".btn">#189</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump ruff from 0.1.11 to 0.3.0 in /oid4vci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [ruff](https://github.com/astral-sh/ruff) from 0.1.11 to 0.3.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/releases">ruff's releases</a>.</em></p>
<blockquote>
<h2>v0.3.0</h2>
<p>This release introduces the new Ruff formatter 2024.2 style and adds a new lint rule to
detect invalid formatter suppression comments.</p>
<h2>Changes</h2>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bandit</code>] Remove suspicious-lxml-import (<code>S410</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10154">#10154</a>)</li>
<li>[<code>pycodestyle</code>] Allow <code>os.environ</code> modifications between imports (<code>E402</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10066">#10066</a>)</li>
<li>[<code>pycodestyle</code>] Don't warn about a single whitespace character before a comma in a tuple (<code>E203</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10094">#10094</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>eradicate</code>] Detect commented out <code>case</code> statements (<code>ERA001</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10055">#10055</a>)</li>
<li>[<code>eradicate</code>] Detect single-line code for <code>try:</code>, <code>except:</code>, etc. (<code>ERA001</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10057">#10057</a>)</li>
<li>[<code>flake8-boolean-trap</code>] Allow boolean positionals in <code>__post_init__</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10027">#10027</a>)</li>
<li>[<code>flake8-copyright</code>] Allow © in copyright notices (<a href="https://redirect.github.com/astral-sh/ruff/pull/10065">#10065</a>)</li>
<li>[<code>isort</code>]: Use one blank line after imports in typing stub files (<a href="https://redirect.github.com/astral-sh/ruff/pull/9971">#9971</a>)</li>
<li>[<code>pylint</code>] New Rule <code>dict-iter-missing-items</code> (<code>PLE1141</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/9845">#9845</a>)</li>
<li>[<code>pylint</code>] Ignore <code>sys.version</code> and <code>sys.platform</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10054">#10054</a>)</li>
<li>[<code>pyupgrade</code>] Detect literals with unary operators (<code>UP018</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10060">#10060</a>)</li>
<li>[<code>ruff</code>] Expand rule for <code>list(iterable).pop(0)</code> idiom (<code>RUF015</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10148">#10148</a>)</li>
</ul>
<h3>Formatter</h3>
<p>This release introduces the Ruff 2024.2 style, stabilizing the following changes:</p>
<ul>
<li>Prefer splitting the assignment's value over the target or type annotation (<a href="https://redirect.github.com/astral-sh/ruff/pull/8943">#8943</a>)</li>
<li>Remove blank lines before class docstrings (<a href="https://redirect.github.com/astral-sh/ruff/pull/9154">#9154</a>)</li>
<li>Wrap multiple context managers in <code>with</code> parentheses when targeting Python 3.9 or newer (<a href="https://redirect.github.com/astral-sh/ruff/pull/9222">#9222</a>)</li>
<li>Add a blank line after nested classes with a dummy body (<code>...</code>) in typing stub files (<a href="https://redirect.github.com/astral-sh/ruff/pull/9155">#9155</a>)</li>
<li>Reduce vertical spacing for classes and functions with a dummy (<code>...</code>) body (<a href="https://redirect.github.com/astral-sh/ruff/issues/7440">#7440</a>, <a href="https://redirect.github.com/astral-sh/ruff/pull/9240">#9240</a>)</li>
<li>Add a blank line after the module docstring (<a href="https://redirect.github.com/astral-sh/ruff/pull/8283">#8283</a>)</li>
<li>Parenthesize long type hints in assignments (<a href="https://redirect.github.com/astral-sh/ruff/pull/9210">#9210</a>)</li>
<li>Preserve indent for single multiline-string call-expressions (<a href="https://redirect.github.com/astral-sh/ruff/pull/9637">#9673</a>)</li>
<li>Normalize hex escape and unicode escape sequences (<a href="https://redirect.github.com/astral-sh/ruff/pull/9280">#9280</a>)</li>
<li>Format module docstrings (<a href="https://redirect.github.com/astral-sh/ruff/pull/9725">#9725</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Explicitly disallow <code>extend</code> as part of a <code>--config</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/10135">#10135</a>)</li>
<li>Remove <code>build</code> from the default exclusion list (<a href="https://redirect.github.com/astral-sh/ruff/pull/10093">#10093</a>)</li>
<li>Deprecate <code>ruff &lt;path&gt;</code>, <code>ruff --explain</code>, <code>ruff --clean</code>, and <code>ruff --generate-shell-completion</code> in favor of <code>ruff check &lt;path&gt;</code>, <code>ruff rule</code>, <code>ruff clean</code>, and <code>ruff generate-shell-completion</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10169">#10169</a>)</li>
<li>Remove the deprecated CLI option <code>--format</code> from <code>ruff rule</code> and <code>ruff linter</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10170">#10170</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Avoid adding default initializers to stubs (<code>B006</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10152">#10152</a>)</li>
<li>[<code>flake8-type-checking</code>] Respect runtime-required decorators for function signatures (<a href="https://redirect.github.com/astral-sh/ruff/pull/10091">#10091</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/astral-sh/ruff/blob/main/CHANGELOG.md">ruff's changelog</a>.</em></p>
<blockquote>
<h2>0.3.0</h2>
<p>This release introduces the new Ruff formatter 2024.2 style and adds a new lint rule to
detect invalid formatter suppression comments.</p>
<h3>Preview features</h3>
<ul>
<li>[<code>flake8-bandit</code>] Remove suspicious-lxml-import (<code>S410</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10154">#10154</a>)</li>
<li>[<code>pycodestyle</code>] Allow <code>os.environ</code> modifications between imports (<code>E402</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10066">#10066</a>)</li>
<li>[<code>pycodestyle</code>] Don't warn about a single whitespace character before a comma in a tuple (<code>E203</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10094">#10094</a>)</li>
</ul>
<h3>Rule changes</h3>
<ul>
<li>[<code>eradicate</code>] Detect commented out <code>case</code> statements (<code>ERA001</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10055">#10055</a>)</li>
<li>[<code>eradicate</code>] Detect single-line code for <code>try:</code>, <code>except:</code>, etc. (<code>ERA001</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10057">#10057</a>)</li>
<li>[<code>flake8-boolean-trap</code>] Allow boolean positionals in <code>__post_init__</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10027">#10027</a>)</li>
<li>[<code>flake8-copyright</code>] Allow © in copyright notices (<a href="https://redirect.github.com/astral-sh/ruff/pull/10065">#10065</a>)</li>
<li>[<code>isort</code>]: Use one blank line after imports in typing stub files (<a href="https://redirect.github.com/astral-sh/ruff/pull/9971">#9971</a>)</li>
<li>[<code>pylint</code>] New Rule <code>dict-iter-missing-items</code> (<code>PLE1141</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/9845">#9845</a>)</li>
<li>[<code>pylint</code>] Ignore <code>sys.version</code> and <code>sys.platform</code> (<code>PLR1714</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10054">#10054</a>)</li>
<li>[<code>pyupgrade</code>] Detect literals with unary operators (<code>UP018</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10060">#10060</a>)</li>
<li>[<code>ruff</code>] Expand rule for <code>list(iterable).pop(0)</code> idiom (<code>RUF015</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10148">#10148</a>)</li>
</ul>
<h3>Formatter</h3>
<p>This release introduces the Ruff 2024.2 style, stabilizing the following changes:</p>
<ul>
<li>Prefer splitting the assignment's value over the target or type annotation (<a href="https://redirect.github.com/astral-sh/ruff/pull/8943">#8943</a>)</li>
<li>Remove blank lines before class docstrings (<a href="https://redirect.github.com/astral-sh/ruff/pull/9154">#9154</a>)</li>
<li>Wrap multiple context managers in <code>with</code> parentheses when targeting Python 3.9 or newer (<a href="https://redirect.github.com/astral-sh/ruff/pull/9222">#9222</a>)</li>
<li>Add a blank line after nested classes with a dummy body (<code>...</code>) in typing stub files (<a href="https://redirect.github.com/astral-sh/ruff/pull/9155">#9155</a>)</li>
<li>Reduce vertical spacing for classes and functions with a dummy (<code>...</code>) body (<a href="https://redirect.github.com/astral-sh/ruff/issues/7440">#7440</a>, <a href="https://redirect.github.com/astral-sh/ruff/pull/9240">#9240</a>)</li>
<li>Add a blank line after the module docstring (<a href="https://redirect.github.com/astral-sh/ruff/pull/8283">#8283</a>)</li>
<li>Parenthesize long type hints in assignments (<a href="https://redirect.github.com/astral-sh/ruff/pull/9210">#9210</a>)</li>
<li>Preserve indent for single multiline-string call-expressions (<a href="https://redirect.github.com/astral-sh/ruff/pull/9637">#9673</a>)</li>
<li>Normalize hex escape and unicode escape sequences (<a href="https://redirect.github.com/astral-sh/ruff/pull/9280">#9280</a>)</li>
<li>Format module docstrings (<a href="https://redirect.github.com/astral-sh/ruff/pull/9725">#9725</a>)</li>
</ul>
<h3>CLI</h3>
<ul>
<li>Explicitly disallow <code>extend</code> as part of a <code>--config</code> flag (<a href="https://redirect.github.com/astral-sh/ruff/pull/10135">#10135</a>)</li>
<li>Remove <code>build</code> from the default exclusion list (<a href="https://redirect.github.com/astral-sh/ruff/pull/10093">#10093</a>)</li>
<li>Deprecate <code>ruff &lt;path&gt;</code>, <code>ruff --explain</code>, <code>ruff --clean</code>, and <code>ruff --generate-shell-completion</code> in favor of <code>ruff check &lt;path&gt;</code>, <code>ruff rule</code>, <code>ruff clean</code>, and <code>ruff generate-shell-completion</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10169">#10169</a>)</li>
<li>Remove the deprecated CLI option <code>--format</code> from <code>ruff rule</code> and <code>ruff linter</code> (<a href="https://redirect.github.com/astral-sh/ruff/pull/10170">#10170</a>)</li>
</ul>
<h3>Bug fixes</h3>
<ul>
<li>[<code>flake8-bugbear</code>] Avoid adding default initializers to stubs (<code>B006</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10152">#10152</a>)</li>
<li>[<code>flake8-type-checking</code>] Respect runtime-required decorators for function signatures (<a href="https://redirect.github.com/astral-sh/ruff/pull/10091">#10091</a>)</li>
<li>[<code>pycodestyle</code>] Mark fixes overlapping with a multiline string as unsafe (<code>W293</code>) (<a href="https://redirect.github.com/astral-sh/ruff/pull/10049">#10049</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/astral-sh/ruff/commit/b53118ed0016ac37233d3dadbcea9ed3ac1f538e"><code>b53118e</code></a> Bump version to v0.3.0 (<a href="https://redirect.github.com/astral-sh/ruff/issues/10151">#10151</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/52f4c1e41be0ce09181c220b1e4918d5bb5ee596"><code>52f4c1e</code></a> Remove deprecated CLI option <code>--format</code> (<a href="https://redirect.github.com/astral-sh/ruff/issues/10170">#10170</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/eceffe74a06f0b1163491624c6c696ebdf3648e9"><code>eceffe7</code></a> Deprecate <code>ruff \&lt;path&gt;</code> <code>ruff --explain</code>, <code>ruff --clean</code> and `ruff --generate...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c73c497477f5abd0d4133c0508d233ebcd78aeba"><code>c73c497</code></a> [<code>pydocstyle</code>] Trim whitespace when removing blank lines after section (`D413...</li>
<li><a href="https://github.com/astral-sh/ruff/commit/c9c98c4fe350fc66d442737ac3b978387fb436e7"><code>c9c98c4</code></a> Fix mkdocs local link (<a href="https://redirect.github.com/astral-sh/ruff/issues/10167">#10167</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/72ccb34ba69969a15da3328248cdaebeccb82b38"><code>72ccb34</code></a> Fix ecosystem check for indico (<a href="https://redirect.github.com/astral-sh/ruff/issues/10164">#10164</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/dcc92f50cf3786fd3cc5a90d9c465fc80209aad6"><code>dcc92f5</code></a> Update black tests (<a href="https://redirect.github.com/astral-sh/ruff/issues/10166">#10166</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/a6f32ddc5e9582112e76ad25039e9b080e281dce"><code>a6f32dd</code></a> Ruff 2024.2 style (<a href="https://redirect.github.com/astral-sh/ruff/issues/9639">#9639</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/0293908b71eeaf610d8ce77d2950f0602fd88dc5"><code>0293908</code></a> Implement RUF028 to detect useless formatter suppression comments (<a href="https://redirect.github.com/astral-sh/ruff/issues/9899">#9899</a>)</li>
<li><a href="https://github.com/astral-sh/ruff/commit/36bc725eaa8d0decb4ad880ddb42094a967feb20"><code>36bc725</code></a> [<code>flake8-bugbear</code>] Avoid adding default initializers to stubs (<code>B006</code>) (<a href="https://redirect.github.com/astral-sh/ruff/issues/10152">#10152</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/astral-sh/ruff/compare/v0.1.11...v0.3.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=ruff&package-manager=pip&previous-version=0.1.11&new-version=0.3.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:30:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/183" class=".btn">#183</a>
            </td>
            <td>
                <b>
                    chore(deps-dev): Bump pytest-ruff from 0.2.1 to 0.3 in /rpc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest-ruff](https://github.com/businho/pytest-ruff) from 0.2.1 to 0.3.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/businho/pytest-ruff/commit/37b8e736063f61ca4b5118ac499ee63fb3943b17"><code>37b8e73</code></a> Support old pytests (<a href="https://redirect.github.com/businho/pytest-ruff/issues/13">#13</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/463bb48aed573d28b63b00e81f317ffcf0c2cbf9"><code>463bb48</code></a> Fix cov (<a href="https://redirect.github.com/businho/pytest-ruff/issues/14">#14</a>)</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/8a6a5a32602cd4936029ddae1bda4ce899b8d98f"><code>8a6a5a3</code></a> Run tox with 3.12 and drop 3.7</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/1ef9b2244f6dc63be9fefeef909092e4cf50c9a1"><code>1ef9b22</code></a> Merge pull request <a href="https://redirect.github.com/businho/pytest-ruff/issues/10">#10</a> from cclauss/patch-1</li>
<li><a href="https://github.com/businho/pytest-ruff/commit/951ece4fff3c07d9be59ab1dcb64bf7e7ad49130"><code>951ece4</code></a> Upgrade GitHub Actions and add Python 3.12</li>
<li>See full diff in <a href="https://github.com/businho/pytest-ruff/compare/v0.2.1...v0.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest-ruff&package-manager=pip&previous-version=0.2.1&new-version=0.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-04 04:23:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/182" class=".btn">#182</a>
            </td>
            <td>
                <b>
                    fix: DIDComm RPC plugin agent messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This fix relaxes the validation rules introduced by #78 preventing incoming agent messages from passing validation checks.

Rules removed:
* Agent messages no longer require `connection_id` or `state` to be included as part of the message. These are still used internally by DRPC records.

Tests and documentation have been updated to reflect the changes.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-01 20:03:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/177" class=".btn">#177</a>
            </td>
            <td>
                <b>
                    chore: update maintainers list
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
        Created At 2024-02-27 21:47:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/176" class=".btn">#176</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump es5-ext from 0.10.62 to 0.10.64 in /oid4vci/integration/afj
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [es5-ext](https://github.com/medikoo/es5-ext) from 0.10.62 to 0.10.64.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/releases">es5-ext's releases</a>.</em></p>
<blockquote>
<h2>0.10.64 (2024-02-27)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">Comparison since last release</a></p>
<h2>0.10.63 (2024-02-23)</h2>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
<hr />
<p><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">Comparison since last release</a></p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/medikoo/es5-ext/blob/main/CHANGELOG.md">es5-ext's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/medikoo/es5-ext/compare/v0.10.63...v0.10.64">0.10.64</a> (2024-02-27)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Revert update to postinstall script meant to fix Powershell issue, as it's a regression for some Linux terminals (<a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a">c2e2bb9</a>)</li>
</ul>
<h3><a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.63">0.10.63</a> (2024-02-23)</h3>
<h3>Bug Fixes</h3>
<ul>
<li>Do not rely on problematic regex (<a href="https://github.com/medikoo/es5-ext/commit/3551cdd7b2db08b1632841f819d008757d28e8e2">3551cdd</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/201">#201</a></li>
<li>Support ES2015+ function definitions in <code>function#toStringTokens()</code> (<a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602">a52e957</a>), addresses <a href="https://redirect.github.com/medikoo/es5-ext/issues/021">#021</a></li>
<li>Ensure postinstall script does not crash on Windows, fixes <a href="https://redirect.github.com/medikoo/es5-ext/issues/181">#181</a> (<a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f">bf8ed79</a>)</li>
</ul>
<h3>Maintenance Improvements</h3>
<ul>
<li>Simplify the manifest message (<a href="https://github.com/medikoo/es5-ext/commit/7855319f41b9736639cf4555bd2c419f17addf55">7855319</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/medikoo/es5-ext/commit/f76b03d8c49ce4871f37f428c0e1d3ee6637fcc4"><code>f76b03d</code></a> chore: Release v0.10.64</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/2881acda50de0848b456690769919ed4b86be489"><code>2881acd</code></a> chore: Bump dependencies</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/c2e2bb90c295c4c582445a6f03b2a3ad0b22550a"><code>c2e2bb9</code></a> fix: Revert update meant to fix Powershell issue, as it's a regression</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/16f2b7253d3d8d499d8cf1d3ca76c585da7f08d3"><code>16f2b72</code></a> docs: Fix date in the changelog</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/de4e03c4776a303284142f73f3f181a070615817"><code>de4e03c</code></a> chore: Release v0.10.63</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/3fd53b755ec883be8f119c747f0b04130741e456"><code>3fd53b7</code></a> chore: Upgrade<code> lint-staged</code> to v13</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/bf8ed799d57df53096da9d908ff577f305e1366f"><code>bf8ed79</code></a> chore: Ensure postinstall script does not crash on Windows</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/2cbbb0717bd8de6e38fcba1f0d45bc876e7a1951"><code>2cbbb07</code></a> chore: Bump dependencies</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/22d0416ea170000a115609f22a560dfa9193ebb0"><code>22d0416</code></a> chore: Bump LICENSE year</li>
<li><a href="https://github.com/medikoo/es5-ext/commit/a52e95736690ad1d465ebcd9791d54570e294602"><code>a52e957</code></a> fix: Support ES2015+ function definitions in <code>function#toStringTokens()</code></li>
<li>Additional commits viewable in <a href="https://github.com/medikoo/es5-ext/compare/v0.10.62...v0.10.64">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=es5-ext&package-manager=npm_and_yarn&previous-version=0.10.62&new-version=0.10.64)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-plugins/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 19:06:26 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-plugins/pull/175" class=".btn">#175</a>
            </td>
            <td>
                <b>
                    Add firebase push notification plugin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds the firebase push notification plugin with documentation, unit test and configurations.

****Note:**** Integration tests not completed. Quite involved, as it requires setting up a mediated connection and a dummy webhook server to make sure events are being triggered and attempting to contact firebase server. Will create another ticket for this task.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-27 19:04:15 +0000 UTC
    </div>
</div>

