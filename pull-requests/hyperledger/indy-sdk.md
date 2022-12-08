---
layout: default
title: indy-sdk
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/indy-sdk
---

# indy-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2564" class=".btn">#2564</a>
            </td>
            <td>
                <b>
                    Bump Newtonsoft.Json from 11.0.2 to 13.0.2 in /wrappers/dotnet/indy-sdk-dotnet-test
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">.NET</span>
            </td>
            <td>
                Bumps [Newtonsoft.Json](https://github.com/JamesNK/Newtonsoft.Json) from 11.0.2 to 13.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/JamesNK/Newtonsoft.Json/releases">Newtonsoft.Json's releases</a>.</em></p>
<blockquote>
<h2>13.0.2</h2>
<ul>
<li>New feature - Add support for DateOnly and TimeOnly</li>
<li>New feature - Add UnixDateTimeConverter.AllowPreEpoch property</li>
<li>New feature - Add copy constructor to JsonSerializerSettings</li>
<li>New feature - Add JsonCloneSettings with property to disable copying annotations</li>
<li>Change - Add nullable annotation to JToken.ToObject(Type, JsonSerializer)</li>
<li>Change - Reduced allocations by reusing boxed values</li>
<li>Fix - Fixed MaxDepth when used with ToObject inside of a JsonConverter</li>
<li>Fix - Fixed deserializing mismatched JToken types in properties</li>
<li>Fix - Fixed merging enumerable content and validate content</li>
<li>Fix - Fixed using $type with arrays of more than two dimensions</li>
<li>Fix - Fixed rare race condition in name table when deserializing on device with ARM processors</li>
<li>Fix - Fixed deserializing via constructor with ignored base type properties</li>
<li>Fix - Fixed MaxDepth not being used with ISerializable deserialization</li>
</ul>
<h2>13.0.1</h2>
<ul>
<li>New feature - Add JsonSelectSettings with configuration for a regex timeout</li>
<li>Change - Remove portable assemblies from NuGet package</li>
<li>Change - JsonReader and JsonSerializer MaxDepth defaults to 64</li>
<li>Change - Change InvalidCastException to JsonSerializationException on mismatched JToken</li>
<li>Fix - Fixed throwing missing member error on ignored fields</li>
<li>Fix - Fixed various nullable annotations</li>
<li>Fix - Fixed annotations not being copied when tokens are cloned</li>
<li>Fix - Fixed naming strategy not being used when deserializing dictionary enum keys</li>
<li>Fix - Fixed serializing nullable struct dictionaries</li>
<li>Fix - Fixed JsonWriter.WriteToken to allow null with string token</li>
<li>Fix - Fixed missing error when deserializing JToken with a contract type mismatch</li>
<li>Fix - Fixed JTokenWriter when writing comment to an object</li>
</ul>
<h2>12.0.3</h2>
<ul>
<li>New feature - Added support for nullable reference types</li>
<li>New feature - Added KebabCaseNamingStrategy</li>
<li>Change - Package now uses embedded package icon</li>
<li>Fix - Fixed bug when merging JToken with itself</li>
<li>Fix - Fixed performance of calling ICustomTypeDescriptor.GetProperties</li>
<li>Fix - Fixed serializing Enumerable.Empty and empty arrays on .NET Core 3.0</li>
<li>Fix - Fixed deserializing some collection types with constructor</li>
<li>Fix - Fixed deserializing IImmutableSet to ImmutableHashSet instead of ImmutableSortedSet</li>
<li>Fix - Fixed deserializing IImmutableDictionary to ImmutableDictionary instead of ImmutableSortedDictionary</li>
<li>Fix - Fixed deserializing into constructors with more than 256 parameters</li>
<li>Fix - Fixed hang when deserializing JTokenReader with preceding comment</li>
<li>Fix - Fixed JSONPath scanning with nested indexer</li>
<li>Fix - Fixed deserializing incomplete JSON object to JObject</li>
<li>Fix - Fixed using StringEnumConverter with naming strategy and specified values</li>
</ul>
<h2>12.0.2</h2>
<ul>
<li>New feature - Added MissingMemberHandling to JsonObjectAttribute and JsonObjectContract</li>
<li>New feature - Added constructor to JTokenReader to specify initial path</li>
<li>New feature - Added JsonProperty.IsRequiredSpecified</li>
<li>New feature - Added JsonContract.InternalConverter</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/4fba53a324c445f06ee08e45a015c346000a7ef2"><code>4fba53a</code></a> Remove prerelease for 13.0.2</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b15df4b50de66065711d5d613f2531e372297fcf"><code>b15df4b</code></a> Add missing headers</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/789bfd3bbcd3d5e567bcfb57a1d08fb8611adf96"><code>789bfd3</code></a> Update to 13.0.2-beta3</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b13717a1c13b0747853568f11fc9e2aa0abf4649"><code>b13717a</code></a> Add JsonCloneSettings to disable copy annotations (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2757">#2757</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/d0a328e8a46304d62d2174b8bba54721d02be3d3"><code>d0a328e</code></a> Fix MaxDepth not being used with ISerializable deserialization (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2736">#2736</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/aae9284e2091e4f2409df175d273cba496c21ccc"><code>aae9284</code></a> Update SDK</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/bd989708b17d5a47b43571414f69ecc0b699eccc"><code>bd98970</code></a> Update to 13.0.2-beta2</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/4dc9af66e07dea321ad101bfb379326127251a80"><code>4dc9af6</code></a> Add roll forward to global.json (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2726">#2726</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b8f4ef0f980a8ee36f511cdec2feb25d5d5d0054"><code>b8f4ef0</code></a> Fixing misspelling (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2698">#2698</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/cb9eed96665019f7398c53c540a87ce675f5d938"><code>cb9eed9</code></a> Fix deserializing via constructor with ignored base type properties (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2711">#2711</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/JamesNK/Newtonsoft.Json/compare/11.0.2...13.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=Newtonsoft.Json&package-manager=nuget&previous-version=11.0.2&new-version=13.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-08 00:51:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/indy-sdk/pull/2563" class=".btn">#2563</a>
            </td>
            <td>
                <b>
                    Bump Newtonsoft.Json from 10.0.3 to 13.0.2 in /samples/dotnet/Samples
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">.NET</span>
            </td>
            <td>
                Bumps [Newtonsoft.Json](https://github.com/JamesNK/Newtonsoft.Json) from 10.0.3 to 13.0.2.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/JamesNK/Newtonsoft.Json/releases">Newtonsoft.Json's releases</a>.</em></p>
<blockquote>
<h2>13.0.2</h2>
<ul>
<li>New feature - Add support for DateOnly and TimeOnly</li>
<li>New feature - Add UnixDateTimeConverter.AllowPreEpoch property</li>
<li>New feature - Add copy constructor to JsonSerializerSettings</li>
<li>New feature - Add JsonCloneSettings with property to disable copying annotations</li>
<li>Change - Add nullable annotation to JToken.ToObject(Type, JsonSerializer)</li>
<li>Change - Reduced allocations by reusing boxed values</li>
<li>Fix - Fixed MaxDepth when used with ToObject inside of a JsonConverter</li>
<li>Fix - Fixed deserializing mismatched JToken types in properties</li>
<li>Fix - Fixed merging enumerable content and validate content</li>
<li>Fix - Fixed using $type with arrays of more than two dimensions</li>
<li>Fix - Fixed rare race condition in name table when deserializing on device with ARM processors</li>
<li>Fix - Fixed deserializing via constructor with ignored base type properties</li>
<li>Fix - Fixed MaxDepth not being used with ISerializable deserialization</li>
</ul>
<h2>13.0.1</h2>
<ul>
<li>New feature - Add JsonSelectSettings with configuration for a regex timeout</li>
<li>Change - Remove portable assemblies from NuGet package</li>
<li>Change - JsonReader and JsonSerializer MaxDepth defaults to 64</li>
<li>Change - Change InvalidCastException to JsonSerializationException on mismatched JToken</li>
<li>Fix - Fixed throwing missing member error on ignored fields</li>
<li>Fix - Fixed various nullable annotations</li>
<li>Fix - Fixed annotations not being copied when tokens are cloned</li>
<li>Fix - Fixed naming strategy not being used when deserializing dictionary enum keys</li>
<li>Fix - Fixed serializing nullable struct dictionaries</li>
<li>Fix - Fixed JsonWriter.WriteToken to allow null with string token</li>
<li>Fix - Fixed missing error when deserializing JToken with a contract type mismatch</li>
<li>Fix - Fixed JTokenWriter when writing comment to an object</li>
</ul>
<h2>12.0.3</h2>
<ul>
<li>New feature - Added support for nullable reference types</li>
<li>New feature - Added KebabCaseNamingStrategy</li>
<li>Change - Package now uses embedded package icon</li>
<li>Fix - Fixed bug when merging JToken with itself</li>
<li>Fix - Fixed performance of calling ICustomTypeDescriptor.GetProperties</li>
<li>Fix - Fixed serializing Enumerable.Empty and empty arrays on .NET Core 3.0</li>
<li>Fix - Fixed deserializing some collection types with constructor</li>
<li>Fix - Fixed deserializing IImmutableSet to ImmutableHashSet instead of ImmutableSortedSet</li>
<li>Fix - Fixed deserializing IImmutableDictionary to ImmutableDictionary instead of ImmutableSortedDictionary</li>
<li>Fix - Fixed deserializing into constructors with more than 256 parameters</li>
<li>Fix - Fixed hang when deserializing JTokenReader with preceding comment</li>
<li>Fix - Fixed JSONPath scanning with nested indexer</li>
<li>Fix - Fixed deserializing incomplete JSON object to JObject</li>
<li>Fix - Fixed using StringEnumConverter with naming strategy and specified values</li>
</ul>
<h2>12.0.2</h2>
<ul>
<li>New feature - Added MissingMemberHandling to JsonObjectAttribute and JsonObjectContract</li>
<li>New feature - Added constructor to JTokenReader to specify initial path</li>
<li>New feature - Added JsonProperty.IsRequiredSpecified</li>
<li>New feature - Added JsonContract.InternalConverter</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/4fba53a324c445f06ee08e45a015c346000a7ef2"><code>4fba53a</code></a> Remove prerelease for 13.0.2</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b15df4b50de66065711d5d613f2531e372297fcf"><code>b15df4b</code></a> Add missing headers</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/789bfd3bbcd3d5e567bcfb57a1d08fb8611adf96"><code>789bfd3</code></a> Update to 13.0.2-beta3</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b13717a1c13b0747853568f11fc9e2aa0abf4649"><code>b13717a</code></a> Add JsonCloneSettings to disable copy annotations (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2757">#2757</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/d0a328e8a46304d62d2174b8bba54721d02be3d3"><code>d0a328e</code></a> Fix MaxDepth not being used with ISerializable deserialization (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2736">#2736</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/aae9284e2091e4f2409df175d273cba496c21ccc"><code>aae9284</code></a> Update SDK</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/bd989708b17d5a47b43571414f69ecc0b699eccc"><code>bd98970</code></a> Update to 13.0.2-beta2</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/4dc9af66e07dea321ad101bfb379326127251a80"><code>4dc9af6</code></a> Add roll forward to global.json (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2726">#2726</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/b8f4ef0f980a8ee36f511cdec2feb25d5d5d0054"><code>b8f4ef0</code></a> Fixing misspelling (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2698">#2698</a>)</li>
<li><a href="https://github.com/JamesNK/Newtonsoft.Json/commit/cb9eed96665019f7398c53c540a87ce675f5d938"><code>cb9eed9</code></a> Fix deserializing via constructor with ignored base type properties (<a href="https://github-redirect.dependabot.com/JamesNK/Newtonsoft.Json/issues/2711">#2711</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/JamesNK/Newtonsoft.Json/compare/10.0.3...13.0.2">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=Newtonsoft.Json&package-manager=nuget&previous-version=10.0.3&new-version=13.0.2)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/indy-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-07 18:28:06 +0000 UTC
    </div>
</div>

