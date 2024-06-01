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
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1191" class=".btn">#1191</a>
            </td>
            <td>
                <b>
                    chore(deps): bump alpine from 3.17.1 to 3.20.0 in /.github/ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">docker</span>
            </td>
            <td>
                Bumps alpine from 3.17.1 to 3.20.0.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=alpine&package-manager=docker&previous-version=3.17.1&new-version=3.20.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1190" class=".btn">#1190</a>
            </td>
            <td>
                <b>
                    chore(deps): bump com.google.code.gson:gson from 2.8.9 to 2.11.0 in /aries/agents/mobile_demo/app
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps [com.google.code.gson:gson](https://github.com/google/gson) from 2.8.9 to 2.11.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/google/gson/releases">com.google.code.gson:gson's releases</a>.</em></p>
<blockquote>
<h2>Gson 2.11.0</h2>
<h1>Most important changes</h1>
<ul>
<li>Added default ProGuard / R8 rules (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2397">#2397</a>, <a href="https://redirect.github.com/google/gson/issues/2420">#2420</a>; <a href="https://github.com/sgjesse"><code>@​sgjesse</code></a>, <a href="https://redirect.github.com/google/gson/issues/2448">#2448</a>; <a href="https://github.com/sfreilich"><code>@​sfreilich</code></a>)<br />
If you are using ProGuard or R8 (for example for Android projects) you might not need any special Gson configuration anymore if your classes have a no-args constructor and use <code>@SerializedName</code> for their fields.</li>
<li>On Android, Gson now requires API level 21 or newer</li>
<li>Added new <code>Strictness</code> API (<a href="https://github.com/marten-voorberg"><code>@​marten-voorberg</code></a> &amp; fellow students, <a href="https://redirect.github.com/google/gson/issues/2437">#2437</a>)<br />
Some of Gson's API is still lenient by default, but you can now use the newly added methods <code>GsonBuilder#setStrictness</code>, <code>JsonReader#setStrictness</code> and <code>JsonWriter#setStrictness</code> with <code>Strictness.STRICT</code> to override this behavior and to instead strictly adhere to the JSON specification when parsing.</li>
<li>New <code>FormattingStyle</code> class to allow configuring line breaks in JSON output (<a href="https://github.com/mihnita"><code>@​mihnita</code></a>, <a href="https://redirect.github.com/google/gson/issues/2231">#2231</a>)<br />
Can be set using <code>GsonBuilder#setFormattingStyle</code> and <code>JsonWriter#setFormattingStyle</code>.</li>
<li><code>TypeToken</code> can no longer capture type variables by default (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2376">#2376</a>)<br />
This was previously a common source of issues. The newly thrown exception refers to a <a href="https://github.com/google/gson/blob/main/Troubleshooting.md#typetoken-type-variable">Troubleshooting Guide article</a> which explains this in more detail and provides suggestions for updating affected code.</li>
<li>Added serialization support for anonymous and local classes with a custom adapter (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2498">#2498</a>)<br />
This affects for example <code>List</code> implementations returned by libraries such as Guava which are implemented as anonymous class, which were previously serialized as <code>null</code>. Anonymous and local classes without custom adapter will still be serialized as <code>null</code>.</li>
<li>Added dependency on <code>com.google.errorprone:error_prone_annotations</code><br />
Your project can use Maven or Gradle dependency exclusions to remove the transitive error_prone_annotations dependency from Gson. Or if you are manually maintaining dependencies as JARs in your project you can omit error_prone_annotations. And it should still work correctly.<br />
But Gson itself does declare it as a required dependency, and if you don't perform any custom configuration, then Maven or Gradle will by default try to download and use it.</li>
<li>Many exception messages now refer to the <a href="https://github.com/google/gson/blob/main/Troubleshooting.md">Troubleshooting Guide</a> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2357">#2357</a>)<br />
Feedback regarding the Troubleshooting Guide is appreciated!</li>
<li>Officially documented that JVM languages other than Java might not be fully supported, see the <a href="https://github.com/google/gson/blob/main/README.md">README</a>.</li>
<li>Guarantee that <code>JsonElement#toString</code> produces JSON output (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2659">#2659</a>)</li>
</ul>
<h1>Other changes</h1>
<h2>Bug fixes</h2>
<ul>
<li>Fixed incorrect <code>JsonPrimitive#equals</code> results for large <code>BigInteger</code> values (<a href="https://github.com/MaicolAntali"><code>@​MaicolAntali</code></a>, <a href="https://redirect.github.com/google/gson/issues/2311">#2311</a>)</li>
<li>Fixed incorrect <code>JsonPrimitive#equals</code> results for large <code>BigDecimal</code> values (<a href="https://github.com/MaicolAntali"><code>@​MaicolAntali</code></a>, <a href="https://redirect.github.com/google/gson/issues/2364">#2364</a>)</li>
<li>Fixed <code>JsonReader</code> throwing <code>NumberFormatException</code> instead of <code>MalformedJsonException</code> for malformed Unicode escape sequences (<a href="https://github.com/MaicolAntali"><code>@​MaicolAntali</code></a>, <a href="https://redirect.github.com/google/gson/issues/2337">#2337</a>)</li>
<li>Fixed <code>TypeToken#getParameterized</code> returning bogus <code>ParameterizedType</code> for non-generic types (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2447">#2447</a>)</li>
<li>Fixed Java Record adapter not working for GraalVM Native Image (<a href="https://github.com/eamonnmcmanus"><code>@​eamonnmcmanus</code></a>, <a href="https://redirect.github.com/google/gson/issues/2465">#2465</a>)</li>
<li>Fixed <code>JsonWriter#name</code> not throwing exception when no JSON object is currently being written (<a href="https://github.com/shivam-sehgal"><code>@​shivam-sehgal</code></a>, <a href="https://redirect.github.com/google/gson/issues/2475">#2475</a>; <a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2476">#2476</a>)</li>
<li>Fixed <code>Gson#getDelegateAdapter</code> not working properly for <code>@JsonAdapter</code> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2435">#2435</a>)<br />
Note that <code>null</code> is now not allowed as <code>skipPast</code> value anymore, which was previously allowed but undocumented.</li>
<li>Fixed <code>GsonBuilder</code> not rejecting type adapters for <code>Object</code> and <code>JsonElement</code>, whose default adapters cannot be overridden (<a href="https://github.com/sachinp97"><code>@​sachinp97</code></a>; <a href="https://redirect.github.com/google/gson/issues/2479">#2479</a>)</li>
<li>Fixed no limits being enforced when deserializing <code>BigDecimal</code> and <code>BigInteger</code> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2510">#2510</a>)<br />
The new limits prevent potential performance problems when user code uses the deserialized numbers. Gson itself was and is not affected by these performance problems. The limits should be high enough to not cause issues for most use cases, but feedback is appreciated.</li>
<li>Fixed <code>GsonBuilder#setDateFormat</code> not rejecting invalid date formats (<a href="https://github.com/Carpe-Wang"><code>@​Carpe-Wang</code></a>, <a href="https://redirect.github.com/google/gson/issues/2538">#2538</a>)</li>
<li>Fixed <code>GsonBuilder#setDateFormat</code> not rejecting invalid date styles (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2545">#2545</a>)</li>
<li>Fixed <code>GsonBuilder#setDateFormat</code> ignoring partial DEFAULT style (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2556">#2556</a>)</li>
<li>Fixed <code>TypeToken#isAssignableFrom</code> throwing <code>AssertionError</code> in some cases (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2544">#2544</a>)</li>
<li>Fixed date adapters not restoring time zone after parsing (<a href="https://github.com/Carpe-Wang"><code>@​Carpe-Wang</code></a>, <a href="https://redirect.github.com/google/gson/issues/2549">#2549</a>)</li>
<li>Fixed <code>TypeToken#equals</code> erroneously returning <code>false</code> for equal generic type parameters in some cases (<a href="https://github.com/d-william"><code>@​d-william</code></a>, <a href="https://redirect.github.com/google/gson/issues/2599">#2599</a>)</li>
<li>Fixed incorrect inherited URLs in <code>pom.xml</code> (<a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2351">#2351</a>)</li>
</ul>
<h2>Performance improvements</h2>
<ul>
<li>Slightly reduce memory usage for reflection-based adapter (<a href="https://github.com/sembseth"><code>@​sembseth</code></a>, <a href="https://redirect.github.com/google/gson/issues/2325">#2325</a>; <a href="https://github.com/Marcono1234"><code>@​Marcono1234</code></a>, <a href="https://redirect.github.com/google/gson/issues/2440">#2440</a>)</li>
<li>Improved parsing speed of <code>ToNumberPolicy#LONG_OR_DOUBLE</code> (<a href="https://github.com/ctasada"><code>@​ctasada</code></a>, <a href="https://redirect.github.com/google/gson/issues/2674">#2674</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/google/gson/blob/main/CHANGELOG.md">com.google.code.gson:gson's changelog</a>.</em></p>
<blockquote>
<h1>Change Log</h1>
<p>The change log for versions newer than 2.10 is available only on the <a href="https://github.com/google/gson/releases">GitHub Releases page</a>.</p>
<h2>Version 2.10</h2>
<ul>
<li>Support for serializing and deserializing Java records, on Java ≥ 16. (<a href="https://redirect.github.com/google/gson/pull/2201">google/gson#2201</a>)</li>
<li>Add <code>JsonArray.asList</code> and <code>JsonObject.asMap</code> view methods (<a href="https://redirect.github.com/google/gson/pull/2225">google/gson#2225</a>)</li>
<li>Fix <code>TypeAdapterRuntimeTypeWrapper</code> not detecting reflective <code>TreeTypeAdapter</code> and <code>FutureTypeAdapter</code> (<a href="https://redirect.github.com/google/gson/pull/1787">google/gson#1787</a>)</li>
<li>Improve <code>JsonReader.skipValue()</code> (<a href="https://redirect.github.com/google/gson/pull/2062">google/gson#2062</a>)</li>
<li>Perform numeric conversion for primitive numeric type adapters (<a href="https://redirect.github.com/google/gson/pull/2158">google/gson#2158</a>)</li>
<li>Add <code>Gson.fromJson(..., TypeToken)</code> overloads (<a href="https://redirect.github.com/google/gson/pull/1700">google/gson#1700</a>)</li>
<li>Fix changes to <code>GsonBuilder</code> affecting existing <code>Gson</code> instances (<a href="https://redirect.github.com/google/gson/pull/1815">google/gson#1815</a>)</li>
<li>Make <code>JsonElement</code> conversion methods more consistent and fix javadoc (<a href="https://redirect.github.com/google/gson/pull/2178">google/gson#2178</a>)</li>
<li>Throw <code>UnsupportedOperationException</code> when <code>JsonWriter.jsonValue</code> is not supported (<a href="https://redirect.github.com/google/gson/pull/1651">google/gson#1651</a>)</li>
<li>Disallow <code>JsonObject</code> <code>Entry.setValue(null)</code> (<a href="https://redirect.github.com/google/gson/pull/2167">google/gson#2167</a>)</li>
<li>Fix <code>TypeAdapter.toJson</code> throwing AssertionError for custom IOException (<a href="https://redirect.github.com/google/gson/pull/2172">google/gson#2172</a>)</li>
<li>Convert null to JsonNull for <code>JsonArray.set</code> (<a href="https://redirect.github.com/google/gson/pull/2170">google/gson#2170</a>)</li>
<li>Fixed nullSafe usage. (<a href="https://redirect.github.com/google/gson/pull/1555">google/gson#1555</a>)</li>
<li>Validate <code>TypeToken.getParameterized</code> arguments (<a href="https://redirect.github.com/google/gson/pull/2166">google/gson#2166</a>)</li>
<li>Fix <a href="https://redirect.github.com/google/gson/issues/1702">#1702</a>: Gson.toJson creates CharSequence which does not implement toString (<a href="https://redirect.github.com/google/gson/pull/1703">google/gson#1703</a>)</li>
<li>Prefer existing adapter for concurrent <code>Gson.getAdapter</code> calls (<a href="https://redirect.github.com/google/gson/pull/2153">google/gson#2153</a>)</li>
<li>Improve <code>ArrayTypeAdapter</code> for <code>Object[]</code> (<a href="https://redirect.github.com/google/gson/pull/1716">google/gson#1716</a>)</li>
<li>Improve <code>AppendableWriter</code> performance (<a href="https://redirect.github.com/google/gson/pull/1706">google/gson#1706</a>)</li>
</ul>
<h2>Version 2.9.1</h2>
<ul>
<li>Make <code>Object</code> and <code>JsonElement</code> deserialization iterative rather than
recursive (<a href="https://redirect.github.com/google/gson/pull/1912">google/gson#1912</a>)</li>
<li>Added parsing support for enum that has overridden toString() method (<a href="https://redirect.github.com/google/gson/pull/1950">google/gson#1950</a>)</li>
<li>Removed support for building Gson with Gradle (<a href="https://redirect.github.com/google/gson/pull/2081">google/gson#2081</a>)</li>
<li>Removed obsolete <code>codegen</code> hierarchy (<a href="https://redirect.github.com/google/gson/pull/2099">google/gson#2099</a>)</li>
<li>Add support for reflection access filter (<a href="https://redirect.github.com/google/gson/pull/1905">google/gson#1905</a>)</li>
<li>Improve <code>TypeToken</code> creation validation (<a href="https://redirect.github.com/google/gson/pull/2072">google/gson#2072</a>)</li>
<li>Add explicit support for <code>float</code> in <code>JsonWriter</code> (<a href="https://redirect.github.com/google/gson/pull/2130">google/gson#2130</a>, <a href="https://redirect.github.com/google/gson/pull/2132">google/gson#2132</a>)</li>
<li>Fail when parsing invalid local date (<a href="https://redirect.github.com/google/gson/pull/2134">google/gson#2134</a>)</li>
</ul>
<p>Also many small improvements to javadoc.</p>
<h2>Version 2.9.0</h2>
<p><strong>The minimum supported Java version changes from 6 to 7.</strong></p>
<ul>
<li>Change target Java version to 7 (<a href="https://redirect.github.com/google/gson/pull/2043">google/gson#2043</a>)</li>
<li>Put <code>module-info.class</code> into Multi-Release JAR folder (<a href="https://redirect.github.com/google/gson/pull/2013">google/gson#2013</a>)</li>
<li>Improve error message when abstract class cannot be constructed (<a href="https://redirect.github.com/google/gson/pull/1814">google/gson#1814</a>)</li>
<li>Support EnumMap deserialization (<a href="https://redirect.github.com/google/gson/pull/2071">google/gson#2071</a>)</li>
<li>Add LazilyParsedNumber default adapter (<a href="https://redirect.github.com/google/gson/pull/2060">google/gson#2060</a>)</li>
<li>Fix JsonReader.hasNext() returning true at end of document (<a href="https://redirect.github.com/google/gson/pull/2061">google/gson#2061</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/google/gson/commit/828a97be0f8d58108b140b77df8dc76b657f4a87"><code>828a97b</code></a> [maven-release-plugin] prepare release gson-parent-2.11.0</li>
<li><a href="https://github.com/google/gson/commit/93bc0f23a13f9e9df3bf71894d479dbd5d952ba6"><code>93bc0f2</code></a> Skip signing graal-native-test module. (<a href="https://redirect.github.com/google/gson/issues/2675">#2675</a>)</li>
<li><a href="https://github.com/google/gson/commit/b153ca18bfef611edff4dbea85de79e153ea4809"><code>b153ca1</code></a> [maven-release-plugin] rollback the release of gson-parent-2.11.0</li>
<li><a href="https://github.com/google/gson/commit/0e3d2aab622fb50addb98b10b0a661cadda0f989"><code>0e3d2aa</code></a> [maven-release-plugin] prepare for next development iteration</li>
<li><a href="https://github.com/google/gson/commit/545b802d639917c50928ec96bcab49b0c70dbb7a"><code>545b802</code></a> [maven-release-plugin] prepare release gson-parent-2.11.0</li>
<li><a href="https://github.com/google/gson/commit/8bfdbb4e14172b013c3d1f56c3a36812075e2886"><code>8bfdbb4</code></a> Guarantee that <code>JsonElement.toString()</code> produces JSON (<a href="https://redirect.github.com/google/gson/issues/2659">#2659</a>)</li>
<li><a href="https://github.com/google/gson/commit/9008b093ac40f226643df17c767357aa1947984a"><code>9008b09</code></a> Extend Troubleshooting Guide with some ProGuard / R8 information (<a href="https://redirect.github.com/google/gson/issues/2656">#2656</a>)</li>
<li><a href="https://github.com/google/gson/commit/05652c3b7dea68a9ffc781b2cdf89076fce56b12"><code>05652c3</code></a> Document that other JVM languages are not fully supported (<a href="https://redirect.github.com/google/gson/issues/2666">#2666</a>)</li>
<li><a href="https://github.com/google/gson/commit/454a49127f9416f45221eecf311eefdca50e4cdc"><code>454a491</code></a> Improved Long-Double Number Policy (<a href="https://redirect.github.com/google/gson/issues/2674">#2674</a>)</li>
<li><a href="https://github.com/google/gson/commit/570d91194e223132982d56b6fa499af15fd7b1ea"><code>570d911</code></a> Bump the github-actions group with 4 updates (<a href="https://redirect.github.com/google/gson/issues/2671">#2671</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/google/gson/compare/gson-parent-2.8.9...gson-parent-2.11.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=com.google.code.gson:gson&package-manager=gradle&previous-version=2.8.9&new-version=2.11.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1189" class=".btn">#1189</a>
            </td>
            <td>
                <b>
                    chore(deps): bump androidx.camera:camera-camera2 from 1.2.3 to 1.3.3 in /aries/agents/mobile_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps androidx.camera:camera-camera2 from 1.2.3 to 1.3.3.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=androidx.camera:camera-camera2&package-manager=gradle&previous-version=1.2.3&new-version=1.3.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1188" class=".btn">#1188</a>
            </td>
            <td>
                <b>
                    chore(deps): bump androidx.compose:compose-bom from 2022.10.00 to 2022.12.00 in /aries/agents/mobile_demo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">java</span>
            </td>
            <td>
                Bumps androidx.compose:compose-bom from 2022.10.00 to 2022.12.00.


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=androidx.compose:compose-bom&package-manager=gradle&previous-version=2022.10.00&new-version=2022.12.00)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-06-01 02:33:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1187" class=".btn">#1187</a>
            </td>
            <td>
                <b>
                    chore: minor readme updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates Aries VCX Community Call timing
Adds note about aries-vcx-agent is not production ready and that a new framework is in development that will fill end developer's needs (as discussed on [5-15-24 community call](https://wiki.hyperledger.org/display/ARIES/2024-5-15+Aries-vcx+community+call))
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-31 16:11:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-vcx/pull/1186" class=".btn">#1186</a>
            </td>
            <td>
                <b>
                    Update MAINTAINERS.md
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates discord username formats
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-30 23:07:02 +0000 UTC
    </div>
</div>

