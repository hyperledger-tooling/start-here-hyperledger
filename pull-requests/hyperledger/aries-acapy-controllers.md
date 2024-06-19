---
layout: default
title: aries-acapy-controllers
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-acapy-controllers
---

# aries-acapy-controllers <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-acapy-controllers){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-acapy-controllers/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Bump the npm_and_yarn group in /AliceFaberAcmeDemo/controllers/alice-controller with 4 updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps the npm_and_yarn group in /AliceFaberAcmeDemo/controllers/alice-controller with 4 updates: [@angular/core](https://github.com/angular/angular/tree/HEAD/packages/core), [vite](https://github.com/vitejs/vite/tree/HEAD/packages/vite), [braces](https://github.com/micromatch/braces) and [ws](https://github.com/websockets/ws).

Updates `@angular/core` from 16.2.12 to 17.0.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular/releases"><code>@​angular/core</code>'s releases</a>.</em></p>
<blockquote>
<h2>v17.0.0</h2>
<p><!-- raw HTML omitted --><!-- raw HTML omitted --></p>
<h1>17.0.0 (2023-11-08)</h1>
<h3></h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular/commit/59aa0634f4d4694203f2a69c40017fe5a3962514"><img src="https://img.shields.io/badge/59aa0634f4-build-yellow" alt="build - 59aa0634f4" /></a></td>
<td>remove support for Node.js v16 (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51755">#51755</a>)</td>
</tr>
</tbody>
</table>
<h3>animations</h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular/commit/e753278faae79a53e235e0d8e03f89555a712d80"><img src="https://img.shields.io/badge/e753278faa-feat-blue" alt="feat - e753278faa" /></a></td>
<td>Add the possibility of lazy loading animations code. (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/50738">#50738</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/698c058e1c975c573722407f4843a4a774ceb92a"><img src="https://img.shields.io/badge/698c058e1c-fix-green" alt="fix - 698c058e1c" /></a></td>
<td>remove code duplication between entry-points (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51500">#51500</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/0598613950c76f4a13601c6942e30ab4ce1e3b67"><img src="https://img.shields.io/badge/0598613950-refactor-yellow" alt="refactor - 0598613950" /></a></td>
<td>deprecation of <code>AnimationDriver.NOOP</code> (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51843">#51843</a>)</td>
</tr>
</tbody>
</table>
<h3>benchpress</h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular/commit/2da3551a703ebef401d76a8e88e388437e851d85"><img src="https://img.shields.io/badge/2da3551a70-feat-blue" alt="feat - 2da3551a70" /></a></td>
<td>report gc and render time spent in script (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/50771">#50771</a>)</td>
</tr>
</tbody>
</table>
<h3>common</h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular/commit/fe2fd7e1a898a4525c219065a6d0908988dfd7e2"><img src="https://img.shields.io/badge/fe2fd7e1a8-feat-blue" alt="feat - fe2fd7e1a8" /></a></td>
<td>make the warning for lazy-loaded lcp image an error (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51748">#51748</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/dde3fdabbd24b48dd6afd120d23e92a3605eb04d"><img src="https://img.shields.io/badge/dde3fdabbd-feat-blue" alt="feat - dde3fdabbd" /></a></td>
<td>upgrade warning to logged error for lazy-loaded LCP images using NgOptimizedImage (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52004">#52004</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/da056a1fe2816299319fb3f87416316be2029479"><img src="https://img.shields.io/badge/da056a1fe2-fix-green" alt="fix - da056a1fe2" /></a></td>
<td>add missing types field for <code>@​angular/common/</code>locales of exports in package.json (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52080">#52080</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/85843e8212e99deb8b70f3d3f8dfe002b978cbb1"><img src="https://img.shields.io/badge/85843e8212-fix-green" alt="fix - 85843e8212" /></a></td>
<td>allow to specify only some properties of <code>DatePipeConfig</code> (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51287">#51287</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/3bd85fb7b0723ed807bca771e9fa95af60a3cfaf"><img src="https://img.shields.io/badge/3bd85fb7b0-fix-green" alt="fix - 3bd85fb7b0" /></a></td>
<td>apply fixed_srcset_width value only to fixed srcsets (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52459">#52459</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/65b460448ec5fdcee5aecca0cdc3cf498b0832cb"><img src="https://img.shields.io/badge/65b460448e-fix-green" alt="fix - 65b460448e" /></a></td>
<td>missing space in ngSwitch equality warning (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52180">#52180</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/86c5e34601d7901a11688124aa902646524177eb"><img src="https://img.shields.io/badge/86c5e34601-fix-green" alt="fix - 86c5e34601" /></a></td>
<td>remove code duplication between entry-points (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51500">#51500</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/28a5925f53790067d45f1f68d204a36088dbf5e3"><img src="https://img.shields.io/badge/28a5925f53-fix-green" alt="fix - 28a5925f53" /></a></td>
<td>use === operator to match NgSwitch cases (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51504">#51504</a>)</td>
</tr>
</tbody>
</table>
<h3>compiler</h3>
<table>
<thead>
<tr>
<th>Commit</th>
<th>Description</th>
</tr>
</thead>
<tbody>
<tr>
<td><a href="https://github.com/angular/angular/commit/1934524a0c673fb65cd927c55c712f59446f9c93"><img src="https://img.shields.io/badge/1934524a0c-feat-blue" alt="feat - 1934524a0c" /></a></td>
<td>add docs extraction for type aliases (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52118">#52118</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/7f6d9a73ab8b658d0d8148080dfefb2550bee6b4"><img src="https://img.shields.io/badge/7f6d9a73ab-feat-blue" alt="feat - 7f6d9a73ab" /></a></td>
<td>expand class api doc extraction (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/a7fa25306f8ce47d8aa330531382106efec55a55"><img src="https://img.shields.io/badge/a7fa25306f-feat-blue" alt="feat - a7fa25306f" /></a></td>
<td>extract api docs for interfaces (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52006">#52006</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/7bfe20707fedff7290e12356a1545644b436d41c"><img src="https://img.shields.io/badge/7bfe20707f-feat-blue" alt="feat - 7bfe20707f" /></a></td>
<td>extract api for fn overloads and abtract classes (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52040">#52040</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/c7daf7ea1692391f7cac8f794ed777887a2764af"><img src="https://img.shields.io/badge/c7daf7ea16-feat-blue" alt="feat - c7daf7ea16" /></a></td>
<td>extract directive docs info (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/e0b1bb33d77babe881f77f52cb1b71e345f5696b"><img src="https://img.shields.io/badge/e0b1bb33d7-feat-blue" alt="feat - e0b1bb33d7" /></a></td>
<td>extract doc info for JsDoc (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/b9c70158abecd81a5af512c8b4da685851cf159f"><img src="https://img.shields.io/badge/b9c70158ab-feat-blue" alt="feat - b9c70158ab" /></a></td>
<td>extract docs for accessors, rest params, and types (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/a24ae994a0470fdac09a69937fd0580cff6c6d68"><img src="https://img.shields.io/badge/a24ae994a0-feat-blue" alt="feat - a24ae994a0" /></a></td>
<td>extract docs for top level functions and consts (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/2e41488296879685b19dfba8d78037690347bda3"><img src="https://img.shields.io/badge/2e41488296-feat-blue" alt="feat - 2e41488296" /></a></td>
<td>extract docs info for enums, pipes, and NgModules (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/34495b35337892ab209d9955ff7fe2897a0c5d41"><img src="https://img.shields.io/badge/34495b3533-feat-blue" alt="feat - 34495b3533" /></a></td>
<td>extract docs via exports (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51828">#51828</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/7e82df45c5bb72ec3dafaa07dc1eaa5d463b006c"><img src="https://img.shields.io/badge/7e82df45c5-feat-blue" alt="feat - 7e82df45c5" /></a></td>
<td>initial skeleton for API doc extraction (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51733">#51733</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/6795cccbbbfc17bbf88fb8197aa172cca67fa2d2"><img src="https://img.shields.io/badge/6795cccbbb-fix-green" alt="fix - 6795cccbbb" /></a></td>
<td>account for type-only imports in defer blocks (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52343">#52343</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/23bfa10ac809f6b27d32647210c52329f0e4262e"><img src="https://img.shields.io/badge/23bfa10ac8-fix-green" alt="fix - 23bfa10ac8" /></a></td>
<td>add diagnostic for inaccessible deferred trigger (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51922">#51922</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/31295a3cf907a61e7115d9039a83a232b263a676"><img src="https://img.shields.io/badge/31295a3cf9-fix-green" alt="fix - 31295a3cf9" /></a></td>
<td>allocating unnecessary slots in conditional instruction (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51913">#51913</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/2aaddd3f64bb8891bb4bdcadf05d427a89338112"><img src="https://img.shields.io/badge/2aaddd3f64-fix-green" alt="fix - 2aaddd3f64" /></a></td>
<td>allow comments between switch cases (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52449">#52449</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/ddd9df68bb2e907dd820f239aaf819425cb95df8"><img src="https://img.shields.io/badge/ddd9df68bb-fix-green" alt="fix - ddd9df68bb" /></a></td>
<td>allow decimals in defer block time values (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52433">#52433</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/7dbd47fb3015117c420f984181bfcb48e533525a"><img src="https://img.shields.io/badge/7dbd47fb30-fix-green" alt="fix - 7dbd47fb30" /></a></td>
<td>allow newlines in track and let expressions (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52137">#52137</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/0eae992c4e03b7c9039476e03b72e92d662293df"><img src="https://img.shields.io/badge/0eae992c4e-fix-green" alt="fix - 0eae992c4e" /></a></td>
<td>allow nullable values in for loop block (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/51997">#51997</a>)</td>
</tr>
<tr>
<td><a href="https://github.com/angular/angular/commit/073ebfe09eccd5d01d27fcc46fc5d4465c1851ff"><img src="https://img.shields.io/badge/073ebfe09e-fix-green" alt="fix - 073ebfe09e" /></a></td>
<td>apply style on :host attributes in prod builds. (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/49118">#49118</a>)</td>
</tr>
</tbody>
</table>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/angular/angular/blob/main/CHANGELOG.md"><code>@​angular/core</code>'s changelog</a>.</em></p>
<blockquote>
<h1>17.0.0 (2023-11-08)</h1>
<p><a href="http://goo.gle/angular-v17">Blog post &quot;Angular v17 is now available&quot;</a>.</p>
<h2>Breaking Changes</h2>
<h3></h3>
<ul>
<li>
<p>Node.js v16 support has been removed and the minimum support version has been bumped to 18.13.0.</p>
<p>Node.js v16 is planned to be End-of-Life on 2023-09-11. Angular will stop supporting Node.js v16 in Angular v17. For Node.js release schedule details, please see: <a href="https://github.com/nodejs/release#release-schedule">https://github.com/nodejs/release#release-schedule</a></p>
</li>
</ul>
<h3>common</h3>
<ul>
<li>the NgSwitch directive now defaults to the === equality operator,
migrating from the previously used == operator. NgSwitch expressions and / or
individual condition values need adjusting to this stricter equality
check. The added warning message should help pin-pointing NgSwitch
usages where adjustments are needed.</li>
</ul>
<h3>core</h3>
<ul>
<li>
<p>Angular now requires <code>zone.js</code> version <code>~0.14.0</code></p>
</li>
<li>
<p>Versions of TypeScript older than 5.2 are no longer supported.</p>
</li>
<li>
<p>The  <code>mutate</code> method was removed from the <code>WritableSignal</code> interface and completely
dropped from the public API surface. As an alternative, please use the <code>update</code> method and
make immutable changes to the object.</p>
<p>Example before:</p>
<pre lang="typescript"><code>items.mutate(itemsArray =&gt; itemsArray.push(newItem));
</code></pre>
<p>Example after:</p>
<pre lang="typescript"><code>items.update(itemsArray =&gt; [itemsArray, …newItem]);
</code></pre>
</li>
<li>
<p><code>OnPush</code> components that are created dynamically now
only have their host bindings refreshed and <code>ngDoCheck run</code> during change
detection if they are dirty.
Previously, a bug in the change detection would result in the <code>OnPush</code>
configuration of dynamically created components to be ignored when
executing host bindings and the <code>ngDoCheck</code> function. This is
rarely encountered but can happen if code has a handle on the
<code>ComponentRef</code> instance and updates values read in the <code>OnPush</code>
component template without then calling either <code>markForCheck</code> or
<code>detectChanges</code> on that component's <code>ChangeDetectorRef</code>.</p>
</li>
</ul>
<h3>platform-browser</h3>
<ul>
<li>
<p><code>REMOVE_STYLES_ON_COMPONENT_DESTROY</code> default value is now <code>true</code>. This causes CSS of components to be removed from the DOM when destroyed. You retain the previous behaviour by providing the <code>REMOVE_STYLES_ON_COMPONENT_DESTROY</code> injection token.</p>
<pre lang="ts"><code>import {REMOVE_STYLES_ON_COMPONENT_DESTROY} from '@angular/platform-browser';
...
providers: [{
</code></pre>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/angular/angular/commit/d4c20aca71932240e975c38294aa540dfcab9d22"><code>d4c20ac</code></a> refactor(core): Add warning when signal equality is false for object.is (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52532">#52532</a>)</li>
<li><a href="https://github.com/angular/angular/commit/43acd44cf8626860a8d410e61c89d67b9d83548e"><code>43acd44</code></a> refactor(core): Remove change detection flag used in g3 (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52530">#52530</a>)</li>
<li><a href="https://github.com/angular/angular/commit/9c2be715a3f6ea6b1d0184f5d79f5a3dfef4b576"><code>9c2be71</code></a> fix(migrations): Fixes a bug in the ngFor pre-v5 alias translation (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52531">#52531</a>)</li>
<li><a href="https://github.com/angular/angular/commit/c267f54bc36e1c92f526071e2d78455daf8a588c"><code>c267f54</code></a> fix(migrations): Update regex to better match ng-templates (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52529">#52529</a>)</li>
<li><a href="https://github.com/angular/angular/commit/83067b3ef257dbc7b1c20d50645615d19023ba51"><code>83067b3</code></a> fix(compiler): ng-template directive invoke twice at the root of control flow...</li>
<li><a href="https://github.com/angular/angular/commit/09e905ad672294d36f36eb2728b3483ab2e729fc"><code>09e905a</code></a> fix(migrations): account for separator characters inside strings (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52525">#52525</a>)</li>
<li><a href="https://github.com/angular/angular/commit/57404d4723d3634f2b5dfdc9af1af50d8f61da70"><code>57404d4</code></a> fix(migrations): handle comma-separated syntax in ngFor (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52525">#52525</a>)</li>
<li><a href="https://github.com/angular/angular/commit/a2ba5482c3032df808cb684444f76e2825a4fd36"><code>a2ba548</code></a> fix(core): use TNode instead of LView for mapping injector providers (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52436">#52436</a>)</li>
<li><a href="https://github.com/angular/angular/commit/6988a0070e9849b58738bba82d6f9eb9e3b27330"><code>6988a00</code></a> fix(migrations): handle ngIf else condition with no whitespaces (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52504">#52504</a>)</li>
<li><a href="https://github.com/angular/angular/commit/236b4483644096110b2427abea3fe95dd35d109f"><code>236b448</code></a> docs: omit repetitions (<a href="https://github.com/angular/angular/tree/HEAD/packages/core/issues/52413">#52413</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/angular/angular/commits/17.0.0/packages/core">compare view</a></li>
</ul>
</details>
<br />

Updates `vite` from 4.4.7 to 4.5.3
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/vitejs/vite/blob/v4.5.3/packages/vite/CHANGELOG.md">vite's changelog</a>.</em></p>
<blockquote>
<h2><!-- raw HTML omitted -->4.5.3 (2024-03-24)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>) (<a href="https://github.com/vitejs/vite/commit/96a7f3a">96a7f3a</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/16250">#16250</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.5.2 (2024-01-19)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: fs deny for case insensitive systems (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15653">#15653</a>) (<a href="https://github.com/vitejs/vite/commit/eeec23b">eeec23b</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15653">#15653</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.5.1 (2023-12-04)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: backport <a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15223">#15223</a>, proxy html path should be encoded (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15226">#15226</a>) (<a href="https://github.com/vitejs/vite/commit/41bb354">41bb354</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/15223">#15223</a> <a href="https://redirect.github.com/vitejs/vite/issues/15226">#15226</a></li>
</ul>
<h2>4.5.0 (2023-10-18)</h2>
<ul>
<li>feat: backport mdx as known js source (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14560">#14560</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14670">#14670</a>) (<a href="https://github.com/vitejs/vite/commit/45595ef">45595ef</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14560">#14560</a> <a href="https://redirect.github.com/vitejs/vite/issues/14670">#14670</a></li>
<li>feat: scan .marko files (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14669">#14669</a>) (<a href="https://github.com/vitejs/vite/commit/ed7bdc5">ed7bdc5</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14669">#14669</a></li>
<li>feat(ssr): backport ssr.resolve.conditions and ssr.resolve.externalConditions (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14498">#14498</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14668">#14668</a>) (<a href="https://github.com/vitejs/vite/commit/520139c">520139c</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14498">#14498</a> <a href="https://redirect.github.com/vitejs/vite/issues/14668">#14668</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.4.11 (2023-10-05)<!-- raw HTML omitted --></h2>
<ul>
<li>revert: &quot;fix: use string manipulation instead of regex to inject esbuild helpers (<a href="https://github.com/vitejs/vite/commit/54e1275">54e1275</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14094">#14094</a></li>
</ul>
<h2><!-- raw HTML omitted -->4.4.10 (2023-10-03)<!-- raw HTML omitted --></h2>
<ul>
<li>fix: add source map to Web Workers (fix <a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14216">#14216</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14217">#14217</a>) (<a href="https://github.com/vitejs/vite/commit/df6f32f">df6f32f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14216">#14216</a> <a href="https://redirect.github.com/vitejs/vite/issues/14217">#14217</a></li>
<li>fix: handle errors during <code>hasWorkspacePackageJSON</code> function (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14394">#14394</a>) (<a href="https://github.com/vitejs/vite/commit/6f6e5de">6f6e5de</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14394">#14394</a></li>
<li>fix: handle sourcemap correctly when multiple line import exists (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14232">#14232</a>) (<a href="https://github.com/vitejs/vite/commit/218861f">218861f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14232">#14232</a></li>
<li>fix: if host is specified check whether it is valid (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14013">#14013</a>) (<a href="https://github.com/vitejs/vite/commit/b1b816a">b1b816a</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14013">#14013</a></li>
<li>fix: include <code>vite/types/*</code> in exports field (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14296">#14296</a>) (<a href="https://github.com/vitejs/vite/commit/40e99a1">40e99a1</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14296">#14296</a></li>
<li>fix: initWasm options should be optional (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14152">#14152</a>) (<a href="https://github.com/vitejs/vite/commit/119c074">119c074</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14152">#14152</a></li>
<li>fix: restore builtins list (<a href="https://github.com/vitejs/vite/commit/f8b9adb">f8b9adb</a>)</li>
<li>fix: use string manipulation instead of regex to inject esbuild helpers (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14094">#14094</a>) (<a href="https://github.com/vitejs/vite/commit/128ad8f">128ad8f</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14094">#14094</a></li>
<li>fix: ws never connects after restarting server if server.hmr.server is set (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14127">#14127</a>) (<a href="https://github.com/vitejs/vite/commit/441642e">441642e</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14127">#14127</a></li>
<li>fix(analysis): warnings for dynamic imports that use static template literals (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14458">#14458</a>) (<a href="https://github.com/vitejs/vite/commit/0c6d289">0c6d289</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14458">#14458</a></li>
<li>fix(cli): convert special base (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14283">#14283</a>) (<a href="https://github.com/vitejs/vite/commit/d4bc0fb">d4bc0fb</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14283">#14283</a></li>
<li>fix(css): remove pure css chunk sourcemap (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14290">#14290</a>) (<a href="https://github.com/vitejs/vite/commit/cd7e033">cd7e033</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14290">#14290</a></li>
<li>fix(css): reset render cache on renderStart (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14326">#14326</a>) (<a href="https://github.com/vitejs/vite/commit/d334b3d">d334b3d</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14326">#14326</a></li>
<li>fix(glob): trigger HMR for glob in a  package (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14117">#14117</a>) (<a href="https://github.com/vitejs/vite/commit/0f582bf">0f582bf</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14117">#14117</a></li>
<li>fix(import-analysis): preserve importedUrls import order (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14465">#14465</a>) (<a href="https://github.com/vitejs/vite/commit/269aa43">269aa43</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14465">#14465</a></li>
<li>fix(manifest): preserve pure css chunk assets (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14297">#14297</a>) (<a href="https://github.com/vitejs/vite/commit/3d63ae6">3d63ae6</a>), closes <a href="https://redirect.github.com/vitejs/vite/issues/14297">#14297</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/vitejs/vite/commit/aac695e9f8f29da43c2f7c50c549fa3d3dfeeadc"><code>aac695e</code></a> release: v4.5.3</li>
<li><a href="https://github.com/vitejs/vite/commit/96a7f3a41ef2f9351c46f3ab12489bb4efa03cc9"><code>96a7f3a</code></a> fix: <code>fs.deny</code> with globs with directories (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/16250">#16250</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/d0360c12476ccc61e9e78c500ed1bd74ed65a2cf"><code>d0360c1</code></a> release: v4.5.2</li>
<li><a href="https://github.com/vitejs/vite/commit/eeec23bbc9d476c54a3a6d36e78455867185a7cb"><code>eeec23b</code></a> fix: fs deny for case insensitive systems (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15653">#15653</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/c0751156f0c015f6dbd5c7a58afd8cff2fde1a2f"><code>c075115</code></a> release: v4.5.1</li>
<li><a href="https://github.com/vitejs/vite/commit/41bb3546a839ed2c822367b3933770c0693a0fb0"><code>41bb354</code></a> fix: backport <a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15223">#15223</a>, proxy html path should be encoded (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/15226">#15226</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/055d2b86b0543a7c1a2a4d5bc7298af62bc51fa7"><code>055d2b8</code></a> release: v4.5.0</li>
<li><a href="https://github.com/vitejs/vite/commit/ed7bdc520679577509466ce808a1794ba8377204"><code>ed7bdc5</code></a> feat: scan .marko files (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14669">#14669</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/45595ef82f786d6b321ce002f2cd4951659114ac"><code>45595ef</code></a> feat: backport mdx as known js source (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14560">#14560</a>) (<a href="https://github.com/vitejs/vite/tree/HEAD/packages/vite/issues/14670">#14670</a>)</li>
<li><a href="https://github.com/vitejs/vite/commit/520139cdff88ae3a0bf89692133cce3e453cb29a"><code>520139c</code></a> feat(ssr): backport ssr.resolve.conditions and ssr.resolve.externalConditions...</li>
<li>Additional commits viewable in <a href="https://github.com/vitejs/vite/commits/v4.5.3/packages/vite">compare view</a></li>
</ul>
</details>
<br />

Updates `braces` from 3.0.2 to 3.0.3
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/micromatch/braces/commit/74b2db2938fad48a2ea54a9c8bf27a37a62c350d"><code>74b2db2</code></a> 3.0.3</li>
<li><a href="https://github.com/micromatch/braces/commit/88f1429a0f47e1dd3813de35211fc97ffda27f9e"><code>88f1429</code></a> update eslint. lint, fix unit tests.</li>
<li><a href="https://github.com/micromatch/braces/commit/415d660c3002d1ab7e63dbf490c9851da80596ff"><code>415d660</code></a> Snyk js braces 6838727 (<a href="https://redirect.github.com/micromatch/braces/issues/40">#40</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/190510f79db1adf21d92798b0bb6fccc1f72c9d6"><code>190510f</code></a> fix tests, skip 1 test in test/braces.expand</li>
<li><a href="https://github.com/micromatch/braces/commit/716eb9f12d820b145a831ad678618731927e8856"><code>716eb9f</code></a> readme bump</li>
<li><a href="https://github.com/micromatch/braces/commit/a5851e57f45c3431a94d83fc565754bc10f5bbc3"><code>a5851e5</code></a> Merge pull request <a href="https://redirect.github.com/micromatch/braces/issues/37">#37</a> from coderaiser/fix/vulnerability</li>
<li><a href="https://github.com/micromatch/braces/commit/2092bd1fb108d2c59bd62e243b70ad98db961538"><code>2092bd1</code></a> feature: braces: add maxSymbols (<a href="https://github.com/micromatch/braces/issues/">https://github.com/micromatch/braces/issues/</a>...</li>
<li><a href="https://github.com/micromatch/braces/commit/9f5b4cf47329351bcb64287223ffb6ecc9a5e6d3"><code>9f5b4cf</code></a> fix: vulnerability (<a href="https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727">https://security.snyk.io/vuln/SNYK-JS-BRACES-6838727</a>)</li>
<li><a href="https://github.com/micromatch/braces/commit/98414f9f1fabe021736e26836d8306d5de747e0d"><code>98414f9</code></a> remove funding file</li>
<li><a href="https://github.com/micromatch/braces/commit/665ab5d561c017a38ba7aafd92cc6655b91d8c14"><code>665ab5d</code></a> update keepEscaping doc (<a href="https://redirect.github.com/micromatch/braces/issues/27">#27</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/micromatch/braces/compare/3.0.2...3.0.3">compare view</a></li>
</ul>
</details>
<br />

Updates `ws` from 7.5.9 to 7.5.10
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/websockets/ws/releases">ws's releases</a>.</em></p>
<blockquote>
<h2>7.5.10</h2>
<h1>Bug fixes</h1>
<ul>
<li>Backported e55e5106 to the 7.x release line (22c28763).</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/websockets/ws/commit/d962d70649e393841ee1ed726a8f7ffbe90d0c06"><code>d962d70</code></a> [dist] 7.5.10</li>
<li><a href="https://github.com/websockets/ws/commit/22c28763234aa75a7e1b76f5c01c181260d7917f"><code>22c2876</code></a> [security] Fix crash when the Upgrade header cannot be read (<a href="https://redirect.github.com/websockets/ws/issues/2231">#2231</a>)</li>
<li>See full diff in <a href="https://github.com/websockets/ws/compare/7.5.9...7.5.10">compare view</a></li>
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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-acapy-controllers/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 19:18:12 +0000 UTC
    </div>
</div>

