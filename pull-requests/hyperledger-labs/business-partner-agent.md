---
layout: default
title: business-partner-agent
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/business-partner-agent
---

# business-partner-agent <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/business-partner-agent){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/827" class=".btn">#827</a>
            </td>
            <td>
                <b>
                    Bump vuetify from 2.6.6 to 2.6.10 in /frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [vuetify](https://github.com/vuetifyjs/vuetify/tree/HEAD/packages/vuetify) from 2.6.6 to 2.6.10.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/vuetifyjs/vuetify/releases">vuetify's releases</a>.</em></p>
<blockquote>
<h2>v2.6.10</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>VCalendar:</strong> prevent XSS from eventName function (<a href="https://github.com/vuetifyjs/vuetify/commit/ade1434927f55a0eccf3d54f900f24c5fa85a176">ade1434</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15757">#15757</a></li>
<li><strong>VDialog:</strong> don't try to focus <code>tabindex=&quot;-1&quot;</code> or hidden inputs (<a href="https://github.com/vuetifyjs/vuetify/commit/89e3850c5478c7bf0ae6081a95f6d2b39e690e8f">89e3850</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15745">#15745</a></li>
<li><strong>VMenu:</strong> disable activatorFixed when attach is enabled (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15709">#15709</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/464529a0358704c27463b660eead65925adf0f6d">464529a</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14922">#14922</a></li>
<li><strong>VTextField:</strong> only show clear icon on hover or when focused (<a href="https://github.com/vuetifyjs/vuetify/commit/7a51ad0140dd17f9d718f6ceb84226d305c2c379">7a51ad0</a>)</li>
<li><strong>VTextField:</strong> prevent tabbing to clear button (<a href="https://github.com/vuetifyjs/vuetify/commit/f8ee680b1d78182852822fd12b63dd00a5803f40">f8ee680</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/11202">#11202</a></li>
<li><strong>web-types:</strong> add support for VDataTable pattern slots (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15694">#15694</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/ac45c98983717d5ee42c4e85de1deccbd698cc83">ac45c98</a>)</li>
</ul>
<h3>:microscope: Code Refactoring</h3>
<ul>
<li><strong>VSelect:</strong> render highlight with vnodes instead of innerHTML (<a href="https://github.com/vuetifyjs/vuetify/commit/4468e3c442284b512729e7b89768fd8762c2e9c1">4468e3c</a>)</li>
</ul>
<h3>BREAKING CHANGES</h3>
<ul>
<li><strong>VCalendar:</strong> <code>eventName</code> function can no longer render arbitrary HTML, convert to VNodes instead.
<code>eventSummary</code> can no longer be used with v-html, replace with <code>&lt;component :is=&quot;{ render: eventSummary }&quot; /&gt;</code></li>
</ul>
<h2>v2.6.9</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>VCalendar:</strong> add aria roles to monthly calendar (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14640">#14640</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/2cd34b4d29ee08b40d9b93e03ee38f50cb4a2a7f">2cd34b4</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14604">#14604</a></li>
<li><strong>VCalendar:</strong> forward all bound events to internal elements (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15592">#15592</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/299330cc64b9a3590822062dbba6f1028f6207d3">299330c</a>)</li>
<li><strong>VCarousel:</strong> add keys to delimiter buttons (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15459">#15459</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/8d3895bc0efd57bb2e5cc6bbf54c2b700e915be7">8d3895b</a>)</li>
<li><strong>VPagination:</strong> ignore invalid length values (<a href="https://github.com/vuetifyjs/vuetify/commit/f3f8d15e9c701c83ab12945ea105fe259aa87b7a">f3f8d15</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15499">#15499</a></li>
<li><strong>VRadio:</strong> change icon color when disabled (<a href="https://github.com/vuetifyjs/vuetify/commit/0cc43e293c0f64e12b210a543e2c71cf084f1ebc">0cc43e2</a>)</li>
<li><strong>VSwitch:</strong> only affect control opacity when disabled (<a href="https://github.com/vuetifyjs/vuetify/commit/1e0a4ad5cde6f4353a52ee5f5dc3731a602038f0">1e0a4ad</a>)</li>
</ul>
<h2>v2.6.8</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>VDataTable:</strong> display header text instead of value in group headers (<a href="https://github.com/vuetifyjs/vuetify/commit/100053fbd229edbab5f64287fe35ca203a24c4ce">100053f</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/11516">#11516</a></li>
<li><strong>VItemGroup:</strong> use valueComparator when updating value (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15395">#15395</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/8bedb7c05e7b4282ea71202cf9ffe562d31fe0f1">8bedb7c</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15394">#15394</a></li>
<li><strong>VSimpleCheckbox:</strong> directly specify ripple directive definition (<a href="https://github.com/vuetifyjs/vuetify/commit/00a9668d7a58bfd1ea3674e48cca2dc8336bbffc">00a9668</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/12224">#12224</a></li>
</ul>
<h2>v2.6.7</h2>
<h3>:wrench: Bug Fixes</h3>
<ul>
<li><strong>styles:</strong> resolve css validation errors (<a href="https://github.com/vuetifyjs/vuetify/commit/621f273bc1608038184255f57b10671dab2a031d">621f273</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15320">#15320</a></li>
<li><strong>VDialog:</strong> focus on internal content when shown (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14584">#14584</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/ffbaae129d36e40bb2926914f2960b09370befb2">ffbaae1</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14581">#14581</a></li>
<li><strong>VInput:</strong> allow text selection in disabled inputs (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14465">#14465</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/760490da75fc531fca9edcd4ef308f2698ba02aa">760490d</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14238">#14238</a></li>
<li><strong>VList:</strong> don't trigger keyboard events on disabled items (<a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15339">#15339</a>) (<a href="https://github.com/vuetifyjs/vuetify/commit/817df79726167fc547a86f1d7c0017080aa1a7e5">817df79</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15322">#15322</a></li>
<li><strong>VOtpInput:</strong> support paste and autofill on mobile (<a href="https://github.com/vuetifyjs/vuetify/commit/8c67ed8cf96334a86c6f087b7abfa845992098a2">8c67ed8</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14801">#14801</a></li>
<li><strong>VRadio:</strong> use correct disabled color for icons (<a href="https://github.com/vuetifyjs/vuetify/commit/31157988d61373af86c015e9e77ed7806b54b658">3115798</a>)</li>
<li><strong>VSelect:</strong> allow keyboard selection of items with value 0 (<a href="https://github.com/vuetifyjs/vuetify/commit/969aba42229275bd1d703d8c51890674105ac6c2">969aba4</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15166">#15166</a></li>
<li><strong>VTabs:</strong> use ResizeObserver if available (<a href="https://github.com/vuetifyjs/vuetify/commit/ff519c6121cc995069caba9b232c216633d6f801">ff519c6</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/4733">#4733</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/10455">#10455</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/12783">#12783</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14195">#14195</a> <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/15316">#15316</a></li>
<li><strong>VTimeline:</strong> disable arrow shadow on clickable cards (<a href="https://github.com/vuetifyjs/vuetify/commit/27ba2c9b7663ce70a35556a3c4336fec44f87605">27ba2c9</a>), closes <a href="https://github-redirect.dependabot.com/vuetifyjs/vuetify/issues/14193">#14193</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/fdfb6fc34d797d2798ae73b049f34e5098793caa"><code>fdfb6fc</code></a> chore(release): publish v2.6.10</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/cd193e41e4041ca0786f5dbcda454e94dd7bddb9"><code>cd193e4</code></a> fix(VSelectList): correct mask class</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/89e3850c5478c7bf0ae6081a95f6d2b39e690e8f"><code>89e3850</code></a> fix(VDialog): don't try to focus tabindex=&quot;-1&quot; or hidden inputs</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/4468e3c442284b512729e7b89768fd8762c2e9c1"><code>4468e3c</code></a> refactor(VSelect): render highlight with vnodes instead of innerHTML</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/ade1434927f55a0eccf3d54f900f24c5fa85a176"><code>ade1434</code></a> fix(VCalendar): prevent XSS from eventName function</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/464529a0358704c27463b660eead65925adf0f6d"><code>464529a</code></a> fix(VMenu): disabled activatorFixed when attach is enabled (<a href="https://github.com/vuetifyjs/vuetify/tree/HEAD/packages/vuetify/issues/15709">#15709</a>)</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/7a51ad0140dd17f9d718f6ceb84226d305c2c379"><code>7a51ad0</code></a> fix(VTextField): only show clear icon on hover or when focused</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/f8ee680b1d78182852822fd12b63dd00a5803f40"><code>f8ee680</code></a> fix(VTextField): prevent tabbing to clear button</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/170c7d14964d410deb70e6c4604fe6cef0608727"><code>170c7d1</code></a> chore(release): publish v2.6.9</li>
<li><a href="https://github.com/vuetifyjs/vuetify/commit/2cd34b4d29ee08b40d9b93e03ee38f50cb4a2a7f"><code>2cd34b4</code></a> fix(VCalendar): add aria roles to monthly calendar (<a href="https://github.com/vuetifyjs/vuetify/tree/HEAD/packages/vuetify/issues/14640">#14640</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/vuetifyjs/vuetify/commits/v2.6.10/packages/vuetify">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=vuetify&package-manager=npm_and_yarn&previous-version=2.6.6&new-version=2.6.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/business-partner-agent/network/alerts).

</details>

<a href="https://gitpod.io/#https://github.com/hyperledger-labs/business-partner-agent/pull/827"><img src="https://gitpod.io/button/open-in-gitpod.svg"/></a>


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-21 22:29:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/business-partner-agent/pull/826" class=".btn">#826</a>
            </td>
            <td>
                <b>
                    Credential attributes file support
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #820 

Draft PR requires changes from https://github.com/hyperledger-labs/acapy-java-client/pull/66

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-16 12:20:33 +0000 UTC
    </div>
</div>

