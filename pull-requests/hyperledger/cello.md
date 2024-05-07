---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/616" class=".btn">#616</a>
            </td>
            <td>
                <b>
                    Bump the pip group across 1 directory with 2 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 2 updates in the /src/api-engine directory: [djangorestframework-simplejwt](https://github.com/jazzband/djangorestframework-simplejwt) and [sqlparse](https://github.com/andialbrecht/sqlparse).

Updates `djangorestframework-simplejwt` from 5.2.2 to 5.3.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/jazzband/djangorestframework-simplejwt/releases">djangorestframework-simplejwt's releases</a>.</em></p>
<blockquote>
<h2>v5.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove EOL Python, Django and DRF versions by <a href="https://github.com/KOliver94"><code>@​KOliver94</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/754">jazzband/djangorestframework-simplejwt#754</a></li>
<li>Update Korean translations by <a href="https://github.com/TGoddessana"><code>@​TGoddessana</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/753">jazzband/djangorestframework-simplejwt#753</a></li>
<li>Declare support for type checking (closes <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/664">#664</a>) by <a href="https://github.com/PedroPerpetua"><code>@​PedroPerpetua</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/760">jazzband/djangorestframework-simplejwt#760</a></li>
<li>Remove usages of deprecated datetime.utcnow() and datetime.utcfromtimestamp() by <a href="https://github.com/kozlek"><code>@​kozlek</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/765">jazzband/djangorestframework-simplejwt#765</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/jazzband/djangorestframework-simplejwt/compare/v5.3.0...v5.3.1">https://github.com/jazzband/djangorestframework-simplejwt/compare/v5.3.0...v5.3.1</a></p>
<h2>v5.3.0</h2>
<h2>What's Changed</h2>
<ul>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/641">jazzband/djangorestframework-simplejwt#641</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/648">jazzband/djangorestframework-simplejwt#648</a></li>
<li>Added Slovenian translations by <a href="https://github.com/banDeveloper"><code>@​banDeveloper</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/645">jazzband/djangorestframework-simplejwt#645</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/652">jazzband/djangorestframework-simplejwt#652</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/655">jazzband/djangorestframework-simplejwt#655</a></li>
<li>Rename de_CH to DE by <a href="https://github.com/Andrew-Chen-Wang"><code>@​Andrew-Chen-Wang</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/653">jazzband/djangorestframework-simplejwt#653</a></li>
<li>Add Python 3.11 to CI, tox, and trove classifiers by <a href="https://github.com/joshuadavidthomas"><code>@​joshuadavidthomas</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/636">jazzband/djangorestframework-simplejwt#636</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/657">jazzband/djangorestframework-simplejwt#657</a></li>
<li>Add Inlang to enable community translations / make the contribution of translations easier  by <a href="https://github.com/jannesblobel"><code>@​jannesblobel</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/662">jazzband/djangorestframework-simplejwt#662</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/666">jazzband/djangorestframework-simplejwt#666</a></li>
<li>Update docs on serializer customization by <a href="https://github.com/2ykwang"><code>@​2ykwang</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/668">jazzband/djangorestframework-simplejwt#668</a></li>
<li>Fixes <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/676">#676</a> - Remove reference to django2.2 by <a href="https://github.com/mattseymour"><code>@​mattseymour</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/677">jazzband/djangorestframework-simplejwt#677</a></li>
<li>fix: rm unused serializers module in views.py by <a href="https://github.com/abel9851"><code>@​abel9851</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/681">jazzband/djangorestframework-simplejwt#681</a></li>
<li>feat: adding typehints by <a href="https://github.com/abczzz13"><code>@​abczzz13</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/683">jazzband/djangorestframework-simplejwt#683</a></li>
<li>Removing dj-22 and djmain from the tox config by <a href="https://github.com/abczzz13"><code>@​abczzz13</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/691">jazzband/djangorestframework-simplejwt#691</a></li>
<li>Add DRF 3.14 Support by <a href="https://github.com/Andrew-Chen-Wang"><code>@​Andrew-Chen-Wang</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/623">jazzband/djangorestframework-simplejwt#623</a></li>
<li>Update <code>django.po</code> for id translation by <a href="https://github.com/kiraware"><code>@​kiraware</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/685">jazzband/djangorestframework-simplejwt#685</a></li>
<li>add he_IL to locale by <a href="https://github.com/elam91"><code>@​elam91</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/679">jazzband/djangorestframework-simplejwt#679</a></li>
<li>Updated translations for Persian (fa) language by <a href="https://github.com/mahdirahimi1999"><code>@​mahdirahimi1999</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/708">jazzband/djangorestframework-simplejwt#708</a></li>
<li>Update customizing_token_claims.rst by <a href="https://github.com/rodrq"><code>@​rodrq</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/714">jazzband/djangorestframework-simplejwt#714</a></li>
<li>Added write_only=True for better doc generation by <a href="https://github.com/Yaser-Amiri"><code>@​Yaser-Amiri</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/699">jazzband/djangorestframework-simplejwt#699</a></li>
<li>Add support for Django 4.2 by <a href="https://github.com/johnthagen"><code>@​johnthagen</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/711">jazzband/djangorestframework-simplejwt#711</a></li>
<li>Add Arabic language translations by <a href="https://github.com/iamjazzar"><code>@​iamjazzar</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/690">jazzband/djangorestframework-simplejwt#690</a></li>
<li>[pre-commit.ci] pre-commit autoupdate by <a href="https://github.com/pre-commit-ci"><code>@​pre-commit-ci</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/694">jazzband/djangorestframework-simplejwt#694</a></li>
<li>Improve testing by <a href="https://github.com/kiraware"><code>@​kiraware</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/688">jazzband/djangorestframework-simplejwt#688</a></li>
<li>Revoke access token if user password is changed by <a href="https://github.com/mahdirahimi1999"><code>@​mahdirahimi1999</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/719">jazzband/djangorestframework-simplejwt#719</a></li>
<li>Updated translations for Persian (fa) language by <a href="https://github.com/mahdirahimi1999"><code>@​mahdirahimi1999</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/723">jazzband/djangorestframework-simplejwt#723</a></li>
<li>Release notes for version 5.3.0 by <a href="https://github.com/aqeelat"><code>@​aqeelat</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/735">jazzband/djangorestframework-simplejwt#735</a></li>
<li>Sync .mo files by <a href="https://github.com/aqeelat"><code>@​aqeelat</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/736">jazzband/djangorestframework-simplejwt#736</a></li>
<li>Sync .mo files by <a href="https://github.com/aqeelat"><code>@​aqeelat</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/737">jazzband/djangorestframework-simplejwt#737</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/banDeveloper"><code>@​banDeveloper</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/645">jazzband/djangorestframework-simplejwt#645</a></li>
<li><a href="https://github.com/joshuadavidthomas"><code>@​joshuadavidthomas</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/636">jazzband/djangorestframework-simplejwt#636</a></li>
<li><a href="https://github.com/jannesblobel"><code>@​jannesblobel</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/662">jazzband/djangorestframework-simplejwt#662</a></li>
<li><a href="https://github.com/mattseymour"><code>@​mattseymour</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/677">jazzband/djangorestframework-simplejwt#677</a></li>
<li><a href="https://github.com/abel9851"><code>@​abel9851</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/681">jazzband/djangorestframework-simplejwt#681</a></li>
<li><a href="https://github.com/abczzz13"><code>@​abczzz13</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/683">jazzband/djangorestframework-simplejwt#683</a></li>
<li><a href="https://github.com/kiraware"><code>@​kiraware</code></a> made their first contribution in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/685">jazzband/djangorestframework-simplejwt#685</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/jazzband/djangorestframework-simplejwt/blob/master/CHANGELOG.md">djangorestframework-simplejwt's changelog</a>.</em></p>
<blockquote>
<h2>5.3.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Remove EOL Python, Django and DRF version support by <a href="https://github.com/KOliver94"><code>@​KOliver94</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/754">#754</a></li>
<li>Declare support for type checking (closes <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/664">#664</a>) by <a href="https://github.com/PedroPerpetua"><code>@​PedroPerpetua</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/760">#760</a></li>
<li>Remove usages of deprecated datetime.utcnow() and datetime.utcfromtimestamp() in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/765">#765</a></li>
</ul>
<h4>Translation Updates:</h4>
<ul>
<li>Update Korean translations by <a href="https://github.com/TGoddessana"><code>@​TGoddessana</code></a> in <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/753">jazzband/djangorestframework-simplejwt#753</a></li>
</ul>
<h2>5.3.0</h2>
<h4>Notable Changes:</h4>
<ul>
<li>Added support for Python 3.11 by <a href="https://github.com/joshuadavidthomas"><code>@​joshuadavidthomas</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/636">#636</a></li>
<li>Added support for Django 4.2 by <a href="https://github.com/johnthagen"><code>@​johnthagen</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/711">#711</a></li>
<li>Added support for DRF 3.14 by <a href="https://github.com/Andrew-Chen-Wang"><code>@​Andrew-Chen-Wang</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/623">#623</a></li>
<li>Added Inlang to facilitate community translations by <a href="https://github.com/jannesblobel"><code>@​jannesblobel</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/662">#662</a></li>
<li>Revoke access token if user password is changed by <a href="https://github.com/mahdirahimi1999"><code>@​mahdirahimi1999</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/719">#719</a></li>
<li>Added type hints by <a href="https://github.com/abczzz13"><code>@​abczzz13</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/683">#683</a></li>
<li>Improved testing by <a href="https://github.com/kiraware"><code>@​kiraware</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/688">#688</a></li>
<li>Removed support for Django 2.2 by <a href="https://github.com/kiraware"><code>@​kiraware</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/688">#688</a></li>
</ul>
<h4>Documentation:</h4>
<ul>
<li>Added write_only=True to TokenBlacklistSerializer's refresh field for better doc generation by <a href="https://github.com/Yaser-Amiri"><code>@​Yaser-Amiri</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/699">#699</a></li>
<li>Updated docs on serializer customization by <a href="https://github.com/2ykwang"><code>@​2ykwang</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/668">#668</a></li>
</ul>
<h4>Translation Updates:</h4>
<ul>
<li>Updated translations for Persian (fa) language by <a href="https://github.com/mahdirahimi1999"><code>@​mahdirahimi1999</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/723">#723</a> and <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/708">jazzband/djangorestframework-simplejwt#708</a></li>
<li>Updated translations for Indonesian (id) language by <a href="https://github.com/kiraware"><code>@​kiraware</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/685">#685</a></li>
<li>Added Arabic language translations by <a href="https://github.com/iamjazzar"><code>@​iamjazzar</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/690">#690</a></li>
<li>Added Hebrew language translations by <a href="https://github.com/elam91"><code>@​elam91</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/679">#679</a></li>
<li>Added Slovenian language translations by <a href="https://github.com/banDeveloper"><code>@​banDeveloper</code></a> <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/pull/645">#645</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/8ae34dd128ef8c5a79d4632e29fa82162bc9a787"><code>8ae34dd</code></a> Remove usages of deprecated datetime.utcnow() and datetime.utcfromtimestamp()...</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/d810271a78b3a69e9b418ad064b981a20977cf2d"><code>d810271</code></a> Declare support for type checking (closes <a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/664">#664</a>) (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/760">#760</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/ef23fb852f83ac7ec82b9ba885011c69b874ab44"><code>ef23fb8</code></a> Update Korean translations (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/753">#753</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/19cf38e4a440fd648e82a94a7998ac857d48a28d"><code>19cf38e</code></a> Remove EOL Python, Django and DRF versions (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/754">#754</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/faf92e8e0894f2e744fc4451289ba26278e50bd5"><code>faf92e8</code></a> Sync .mo files (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/737">#737</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/16866f538e79c39a84676433cdef35b1dd5c72bc"><code>16866f5</code></a> Sync .mo files (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/736">#736</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/6c52647c4ec2a79c6ab57ba8314eb228346cddf7"><code>6c52647</code></a> Release version 5.3.0 (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/735">#735</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/47b7a08caddfedbdc008b9e3406b038cb2a8dd32"><code>47b7a08</code></a> Updated translations for Persian (fa) language (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/723">#723</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/a775004553031e10f2d97e9e80ae5ef72f5020f6"><code>a775004</code></a> Revoke access token if user password is changed (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/719">#719</a>)</li>
<li><a href="https://github.com/jazzband/djangorestframework-simplejwt/commit/d2cd59d0cc871a70b634db6825b8a9749d1fbe59"><code>d2cd59d</code></a> Improve testing (<a href="https://redirect.github.com/jazzband/djangorestframework-simplejwt/issues/688">#688</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/jazzband/djangorestframework-simplejwt/compare/v5.2.2...v5.3.1">compare view</a></li>
</ul>
</details>
<br />

Updates `sqlparse` from 0.4.4 to 0.5.0
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/andialbrecht/sqlparse/blob/master/CHANGELOG">sqlparse's changelog</a>.</em></p>
<blockquote>
<h2>Release 0.5.0 (Apr 13, 2024)</h2>
<p>Notable Changes</p>
<ul>
<li>Drop support for Python 3.5, 3.6, and 3.7.</li>
<li>Python 3.12 is now supported (pr725, by hugovk).</li>
<li>IMPORTANT: Fixes a potential denial of service attack (DOS) due to recursion
error for deeply nested statements. Instead of recursion error a generic
SQLParseError is raised. See the security advisory for details:
<a href="https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-2m57-hf25-phgg">https://github.com/andialbrecht/sqlparse/security/advisories/GHSA-2m57-hf25-phgg</a>
The vulnerability was discovered by <a href="https://github.com/uriyay-jfrog"><code>@​uriyay-jfrog</code></a>. Thanks for reporting!</li>
</ul>
<p>Enhancements:</p>
<ul>
<li>Splitting statements now allows to remove the semicolon at the end.
Some database backends love statements without semicolon (issue742).</li>
<li>Support TypedLiterals in get_parameters (pr749, by Khrol).</li>
<li>Improve splitting of Transact SQL when using GO keyword (issue762).</li>
<li>Support for some JSON operators (issue682).</li>
<li>Improve formatting of statements containing JSON operators (issue542).</li>
<li>Support for BigQuery and Snowflake keywords (pr699, by griffatrasgo).</li>
<li>Support parsing of OVER clause (issue701, pr768 by r33s3n6).</li>
</ul>
<p>Bug Fixes</p>
<ul>
<li>Ignore dunder attributes when creating Tokens (issue672).</li>
<li>Allow operators to precede dollar-quoted strings (issue763).</li>
<li>Fix parsing of nested order clauses (issue745, pr746 by john-bodley).</li>
<li>Thread-safe initialization of Lexer class (issue730).</li>
<li>Classify TRUNCATE as DDL and GRANT/REVOKE as DCL keywords (based on pr719
by josuc1, thanks for bringing this up!).</li>
<li>Fix parsing of PRIMARY KEY (issue740).</li>
</ul>
<p>Other</p>
<ul>
<li>Optimize performance of matching function (pr799, by admachainz).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/ddbd0ec3592545c914fe71e47118c04582d8bfb0"><code>ddbd0ec</code></a> Bump version.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/29f2e0a6609ddc1fa248faef1bc41616043c544e"><code>29f2e0a</code></a> Raise recursion limit for tests.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/b4a39d9850969b4e1d6940d32094ee0b42a2cf03"><code>b4a39d9</code></a> Raise SQLParseError instead of RecursionError.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/f1bcf2f8a7ddf6854c99990c56ff5394f4981d58"><code>f1bcf2f</code></a> Update AUHTORS and Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/e03b74e608b71dd06824c2cb42421c0d790248e3"><code>e03b74e</code></a> Fix Function.get_parameters(), add Funtion.get_window()</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/617b8f6cd3c55bacf2c80130901508518753f7e1"><code>617b8f6</code></a> Add OVER clause, and group it into Function (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/701">#701</a>)</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/d8f81471cfc2c39ac43128e2a0c8cc67c313cc40"><code>d8f8147</code></a> Update AUHTORS and Changelog.</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/012c9f10c8ddfa47ccf17ead28122492155cf6fc"><code>012c9f1</code></a> Optimize sqlparse.utils.imt().</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/46971e5a804b29e7dbd437155a8ceffab8ef1cd5"><code>46971e5</code></a> Fix parsing of PRIMARY KEY (fixes <a href="https://redirect.github.com/andialbrecht/sqlparse/issues/740">#740</a>).</li>
<li><a href="https://github.com/andialbrecht/sqlparse/commit/fc4b0beab89c5598d556572cb6db0165affb017b"><code>fc4b0be</code></a> Code cleanup.</li>
<li>Additional commits viewable in <a href="https://github.com/andialbrecht/sqlparse/compare/0.4.4...0.5.0">compare view</a></li>
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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-06 20:57:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/615" class=".btn">#615</a>
            </td>
            <td>
                <b>
                    Bump gh-pages from 2.2.0 to 6.1.1 in /src/dashboard in the npm_and_yarn group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group with 1 update in the /src/dashboard directory: [gh-pages](https://github.com/tschaub/gh-pages).

Updates `gh-pages` from 2.2.0 to 6.1.1
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/tschaub/gh-pages/releases">gh-pages's releases</a>.</em></p>
<blockquote>
<h2>v6.1.1</h2>
<h2>Fixes</h2>
<ul>
<li>fix: Add missing cname option not passed to the config by <a href="https://github.com/WillBAnders"><code>@​WillBAnders</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/535">tschaub/gh-pages#535</a></li>
</ul>
<h2>Dependency Updates</h2>
<ul>
<li>Bump eslint from 8.53.0 to 8.55.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/538">tschaub/gh-pages#538</a></li>
<li>Bump fs-extra from 11.1.1 to 11.2.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/537">tschaub/gh-pages#537</a></li>
<li>Bump eslint from 8.55.0 to 8.56.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/539">tschaub/gh-pages#539</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/WillBAnders"><code>@​WillBAnders</code></a> made their first contribution in <a href="https://redirect.github.com/tschaub/gh-pages/pull/535">tschaub/gh-pages#535</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tschaub/gh-pages/compare/v6.1.0...v6.1.1">https://github.com/tschaub/gh-pages/compare/v6.1.0...v6.1.1</a></p>
<h2>v6.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump eslint from 8.46.0 to 8.49.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/516">tschaub/gh-pages#516</a></li>
<li>Bump actions/checkout from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/515">tschaub/gh-pages#515</a></li>
<li>Bump chai from 4.3.7 to 4.3.8 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/513">tschaub/gh-pages#513</a></li>
<li>Bump dir-compare from 4.0.0 to 4.2.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/512">tschaub/gh-pages#512</a></li>
<li>Add --nojekyll and --cname options by <a href="https://github.com/tschaub"><code>@​tschaub</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/533">tschaub/gh-pages#533</a></li>
<li>Bump actions/setup-node from 3 to 4 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/527">tschaub/gh-pages#527</a></li>
<li>Bump chai from 4.3.8 to 4.3.10 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/520">tschaub/gh-pages#520</a></li>
<li>Bump eslint from 8.49.0 to 8.53.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/530">tschaub/gh-pages#530</a></li>
<li>Bump commander from 11.0.0 to 11.1.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/524">tschaub/gh-pages#524</a></li>
<li>Bump async from 3.2.4 to 3.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/529">tschaub/gh-pages#529</a></li>
<li>Bump sinon from 15.2.0 to 17.0.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/531">tschaub/gh-pages#531</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/tschaub/gh-pages/compare/v6.0.0...v6.1.0">https://github.com/tschaub/gh-pages/compare/v6.0.0...v6.1.0</a></p>
<h2>v6.0.0</h2>
<p>This release drops support for Node 14.  Otherwise, there are no special upgrade considerations.</p>
<h2>What's Changed</h2>
<ul>
<li>Update readme.md by <a href="https://github.com/harveer07"><code>@​harveer07</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/440">tschaub/gh-pages#440</a></li>
<li>Bump sinon from 15.0.1 to 15.0.3 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/474">tschaub/gh-pages#474</a></li>
<li>Bump eslint from 8.32.0 to 8.38.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/477">tschaub/gh-pages#477</a></li>
<li>Bump fs-extra from 8.1.0 to 11.1.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/473">tschaub/gh-pages#473</a></li>
<li>Add error message when --dist is not specified. by <a href="https://github.com/domsleee"><code>@​domsleee</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/504">tschaub/gh-pages#504</a></li>
<li>Bump word-wrap from 1.2.3 to 1.2.5 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/505">tschaub/gh-pages#505</a></li>
<li>Bump eslint from 8.38.0 to 8.46.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/506">tschaub/gh-pages#506</a></li>
<li>Bump semver from 6.3.0 to 6.3.1 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/500">tschaub/gh-pages#500</a></li>
<li>Bump sinon from 15.0.3 to 15.2.0 by <a href="https://github.com/dependabot"><code>@​dependabot</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/495">tschaub/gh-pages#495</a></li>
<li>Dependency updates and drop Node 14 by <a href="https://github.com/tschaub"><code>@​tschaub</code></a> in <a href="https://redirect.github.com/tschaub/gh-pages/pull/507">tschaub/gh-pages#507</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/harveer07"><code>@​harveer07</code></a> made their first contribution in <a href="https://redirect.github.com/tschaub/gh-pages/pull/440">tschaub/gh-pages#440</a></li>
<li><a href="https://github.com/domsleee"><code>@​domsleee</code></a> made their first contribution in <a href="https://redirect.github.com/tschaub/gh-pages/pull/504">tschaub/gh-pages#504</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/tschaub/gh-pages/blob/main/changelog.md">gh-pages's changelog</a>.</em></p>
<blockquote>
<h2>v6.1.1</h2>
<p>This release fixes an issue with the <code>--cname</code> option.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/535">#535</a> - fix: Add missing cname option not passed to the config (<a href="https://github.com/WillBAnders"><code>@​WillBAnders</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/539">#539</a> - Bump eslint from 8.55.0 to 8.56.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
</ul>
<h2>v6.1.0</h2>
<p>This release adds support for <code>--nojekyll</code> and <code>--cname</code> options.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/531">#531</a> - Bump sinon from 15.2.0 to 17.0.1 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/529">#529</a> - Bump async from 3.2.4 to 3.2.5 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/524">#524</a> - Bump commander from 11.0.0 to 11.1.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/530">#530</a> - Bump eslint from 8.49.0 to 8.53.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/520">#520</a> - Bump chai from 4.3.8 to 4.3.10 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/527">#527</a> - Bump actions/setup-node from 3 to 4 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/533">#533</a> - Add --nojekyll and --cname options (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/512">#512</a> - Bump dir-compare from 4.0.0 to 4.2.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/513">#513</a> - Bump chai from 4.3.7 to 4.3.8 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/515">#515</a> - Bump actions/checkout from 3 to 4 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/516">#516</a> - Bump eslint from 8.46.0 to 8.49.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
</ul>
<h2>v6.0.0</h2>
<p>This release drops support for Node 14.  Otherwise, there are no special upgrade considerations.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/507">#507</a> - Dependency updates and drop Node 14 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/495">#495</a> - Bump sinon from 15.0.3 to 15.2.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/500">#500</a> - Bump semver from 6.3.0 to 6.3.1 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/506">#506</a> - Bump eslint from 8.38.0 to 8.46.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/505">#505</a> - Bump word-wrap from 1.2.3 to 1.2.5 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/504">#504</a> - Add error message when --dist is not specified. (<a href="https://github.com/domsleee"><code>@​domsleee</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/473">#473</a> - Bump fs-extra from 8.1.0 to 11.1.1 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/477">#477</a> - Bump eslint from 8.32.0 to 8.38.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/474">#474</a> - Bump sinon from 15.0.1 to 15.0.3 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/440">#440</a> - Update readme.md (<a href="https://github.com/harveer07"><code>@​harveer07</code></a>)</li>
</ul>
<h2>v5.0.0</h2>
<p>Potentially breaking change: the <code>publish</code> method now always returns a promise.  Previously, it did not return a promise in some error cases.  This should not impact most users.</p>
<p>Updates to the development dependencies required a minimum Node version of 14 for the tests.  The library should still work on Node 12, but tests are no longer run in CI for version 12.  A future major version of the library may drop support for version 12 altogether.</p>
<ul>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/438">#438</a> - Remove quotation marks (<a href="https://github.com/Vicropht"><code>@​Vicropht</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/459">#459</a> - Bump async from 2.6.4 to 3.2.4 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/454">#454</a> - Bump email-addresses from 3.0.1 to 5.0.0 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/455">#455</a> - Bump actions/setup-node from 1 to 3 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/453">#453</a> - Bump actions/checkout from 2 to 3 (<a href="https://github.com/tschaub"><code>@​tschaub</code></a>)</li>
<li><a href="https://redirect.github.com/tschaub/gh-pages/pull/445">#445</a> - Update README to clarify project site configuration requirements with tools like CRA, webpack, Vite, etc. (<a href="https://github.com/Nezteb"><code>@​Nezteb</code></a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/tschaub/gh-pages/commit/e98ba0f5f8fc8da9d7596c604ee89d7d18ba1d5d"><code>e98ba0f</code></a> 6.1.1</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/122872fee4006039f5844790bad15f53ec711a28"><code>122872f</code></a> Log changes</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/3312dc4f4c9ebd841b545ec3833169a473a2be40"><code>3312dc4</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/535">#535</a> from WillBAnders/fix/missing-cname-option</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/b6b84541cb7918ce1b99ea9688808f63af0c356a"><code>b6b8454</code></a> Add test for cnameExists, asserting it replaces the existing CNAME</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/1c60556b34b99ebece5b22911e6f049feb37d746"><code>1c60556</code></a> Add debug logs for nojekyll/cname creation as recommended by <a href="https://github.com/paymand"><code>@​paymand</code></a></li>
<li><a href="https://github.com/tschaub/gh-pages/commit/727d7142bfeb9ba08621664156cae0dc1b80cfee"><code>727d714</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/539">#539</a> from tschaub/dependabot/npm_and_yarn/eslint-8.56.0</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/2a53e7657f1ea96c7f3707cb83275f2884e7b314"><code>2a53e76</code></a> Bump eslint from 8.55.0 to 8.56.0</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/96124afd25dc8c9e077bd48e1bd1558e2796b21b"><code>96124af</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/537">#537</a> from tschaub/dependabot/npm_and_yarn/fs-extra-11.2.0</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/09076df0439b9b6a49ac712b891647b264741aee"><code>09076df</code></a> Merge pull request <a href="https://redirect.github.com/tschaub/gh-pages/issues/538">#538</a> from tschaub/dependabot/npm_and_yarn/eslint-8.55.0</li>
<li><a href="https://github.com/tschaub/gh-pages/commit/81354958e27a0c8741a8bc2ec88f5748792a96ed"><code>8135495</code></a> Bump eslint from 8.53.0 to 8.55.0</li>
<li>Additional commits viewable in <a href="https://github.com/tschaub/gh-pages/compare/v2.2.0...v6.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=gh-pages&package-manager=npm_and_yarn&previous-version=2.2.0&new-version=6.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore <dependency name> major version` will close this group update PR and stop Dependabot creating any more for the specific dependency's major version (unless you unignore this specific dependency's major version or upgrade to it yourself)
- `@dependabot ignore <dependency name> minor version` will close this group update PR and stop Dependabot creating any more for the specific dependency's minor version (unless you unignore this specific dependency's minor version or upgrade to it yourself)
- `@dependabot ignore <dependency name>` will close this group update PR and stop Dependabot creating any more for the specific dependency (unless you unignore this specific dependency or upgrade to it yourself)
- `@dependabot unignore <dependency name>` will remove all of the ignore conditions of the specified dependency
- `@dependabot unignore <dependency name> <ignore condition>` will remove the ignore condition of the specified dependency and ignore conditions
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/cello/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-02 18:13:09 +0000 UTC
    </div>
</div>

