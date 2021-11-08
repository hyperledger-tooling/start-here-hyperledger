---
layout: default
title: aries-framework-javascript
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-framework-javascript
---

# aries-framework-javascript <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-framework-javascript){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/531" class=".btn">#531</a>
            </td>
            <td>
                <b>
                    feat: Add support for new out-of-band protocol Stage 1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is the first step in the implementation of #344. 

It corresponds approximately to Step 1 defined in [Aries RFC 0496: Transition to the Out of Band and DID Exchange Protocols](https://github.com/hyperledger/aries-rfcs/blob/main/features/0496-transition-to-oob-and-did-exchange/README.md).

As you can see I decided to create an Out-of-band module and keep the implementation there. I realized that putting it into the Connection module could cause more issues than benefits right now. It has only two drawbacks:
* API users would need to decide what method to call for now. But it allows more gradual adoption of new out-of-band by users. When we have a full implementation, users will ideally just call one method for OOB messages.
* I copy-pasted methods for connection creation. That can be solved by calling the whole Connections module from the OOB module.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-08 15:59:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/528" class=".btn">#528</a>
            </td>
            <td>
                <b>
                    fix(core): log errors if message is undeliverable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The error message being logged just indicated that a message is underliverable to a certain connection. It swallowed the underlying errors. This adds an `errors` property to the error log so that it is clear what the underlying errors are when a message is underliverable.

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 16:01:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/527" class=".btn">#527</a>
            </td>
            <td>
                <b>
                    fix(core)!: do not request ping res for connection
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BREAKING CHANGE: a trust ping response will not be requested anymore after completing a connection. This is not required, and also non-standard behaviour. It was also causing some tests to be flaky as response messages were stil being sent after one of the agents had already shut down.

Signed-off-by: Timo Glastra <timo@animo.id>

Maintainers: Before merging and squashing make sure to copy the `BREAKING CHANGE` entry to the commit message field, this is needed for automatic tracking of breaking changes


Fixes #515 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 15:28:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/526" class=".btn">#526</a>
            </td>
            <td>
                <b>
                    feat(core): validate outbound messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 15:07:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/525" class=".btn">#525</a>
            </td>
            <td>
                <b>
                    fix(core)!: improve proof request validation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BREAKING CHANGE: Proof request requestedAttributes and requestedPredicates are now a map instead of record. This is needed to have proper validation using class-validator.

Signed-off-by: Timo Glastra <timo@animo.id>

Maintainers: Before merging and squashing make sure to copy the `BREAKING CHANGE` entry to the commit message field, this is needed for automatic tracking of breaking changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 15:06:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/524" class=".btn">#524</a>
            </td>
            <td>
                <b>
                    fix(core): fix empty error log in console logger
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The console logger stringified the data object. Appereantly the Error class has no enumerable properties which means it will be stringified as an empty object. This fix checks if a (top level) value being transformed is an error and will transform the non-enumerable properties of the error.

Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 14:59:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/523" class=".btn">#523</a>
            </td>
            <td>
                <b>
                    refactor(core)!: simplify get creds for proof api
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                BREAKING CHANGE: The `ProofsModule.getRequestedCredentialsForProofRequest` expected some low level message objects as input. This is not in line with the public API of the rest of the framework and has been simplified to only require a proof record id and optionally a boolean whether the retrieved credentials should by filtered based on the proof proposal (if avaiable).

Signed-off-by: Timo Glastra <timo@animo.id>

Maintainers: Before merging and squashing make sure to copy the `BREAKING CHANGE` entry to the commit message field, this is needed for automatic tracking of breaking changes
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-07 13:29:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/521" class=".btn">#521</a>
            </td>
            <td>
                <b>
                    build(deps): bump validator from 13.6.0 to 13.7.0
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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-framework-javascript/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-03 19:28:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/516" class=".btn">#516</a>
            </td>
            <td>
                <b>
                    feat(core): update agent label and imageUrl plus per connection label and imageUrl
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #506 

This pr contains:

- Support for updating agent label
- Support for custom label on connection/invitation

I would also like to add support for a custom imageUrl on connection/label, but before that i would like some feedback on this draft.



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-02 07:37:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/513" class=".btn">#513</a>
            </td>
            <td>
                <b>
                    fix(core): improve wallet not initialized error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>

To help when user forgot to call `agent.initialize()` (https://github.com/hyperledger/aries-framework-javascript/issues/508)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 18:47:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-framework-javascript/pull/512" class=".btn">#512</a>
            </td>
            <td>
                <b>
                    fix(core): do not throw error on timeout in http
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Timo Glastra <timo@animo.id>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-01 16:52:01 +0000 UTC
    </div>
</div>

