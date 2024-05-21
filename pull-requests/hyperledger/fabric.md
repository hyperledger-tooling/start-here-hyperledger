---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4867" class=".btn">#4867</a>
            </td>
            <td>
                <b>
                    Bump requests from 2.31.0 to 2.32.0 in /docs in the pip group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the /docs directory: [requests](https://github.com/psf/requests).

Updates `requests` from 2.31.0 to 2.32.0
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/releases">requests's releases</a>.</em></p>
<blockquote>
<h2>v2.32.0</h2>
<h2>2.32.0 (2024-05-20)</h2>
<h2>🐍 PYCON US 2024 EDITION 🐍</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<ul>
<li>Requests has officially added support for CPython 3.12 (<a href="https://redirect.github.com/psf/requests/issues/6503">#6503</a>)</li>
<li>Requests has officially added support for PyPy 3.9 and 3.10 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
<li>Requests has officially dropped support for CPython 3.7 (<a href="https://redirect.github.com/psf/requests/issues/6642">#6642</a>)</li>
<li>Requests has officially dropped support for PyPy 3.7 and 3.8 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
</ul>
<p><strong>Documentation</strong></p>
<ul>
<li>Various typo fixes and doc improvements.</li>
</ul>
<p><strong>Packaging</strong></p>
<ul>
<li>Requests has started adopting some modern packaging practices.
The source files for the projects (formerly <code>requests</code>) is now located
in <code>src/requests</code> in the Requests sdist. (<a href="https://redirect.github.com/psf/requests/issues/6506">#6506</a>)</li>
<li>Starting in Requests 2.33.0, Requests will migrate to a PEP 517 build system
using <code>hatchling</code>. This should not impact the average user, but extremely old
versions of packaging utilities may have issues with the new packaging format.</li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/matthewarmand"><code>@​matthewarmand</code></a> made their first contribution in <a href="https://redirect.github.com/psf/requests/pull/6258">psf/requests#6258</a></li>
<li><a href="https://github.com/cpzt"><code>@​cpzt</code></a> made their first contribution in <a href="https://redirect.github.com/psf/requests/pull/6456">psf/requests#6456</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/requests/blob/main/HISTORY.md">requests's changelog</a>.</em></p>
<blockquote>
<h2>2.32.0 (2024-05-20)</h2>
<p><strong>Security</strong></p>
<ul>
<li>Fixed an issue where setting <code>verify=False</code> on the first request from a
Session will cause subsequent requests to the <em>same origin</em> to also ignore
cert verification, regardless of the value of <code>verify</code>.
(<a href="https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56">https://github.com/psf/requests/security/advisories/GHSA-9wx4-h78v-vm56</a>)</li>
</ul>
<p><strong>Improvements</strong></p>
<ul>
<li><code>verify=True</code> now reuses a global SSLContext which should improve
request time variance between first and subsequent requests. It should
also minimize certificate load time on Windows systems when using a Python
version built with OpenSSL 3.x. (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li>Requests now supports optional use of character detection
(<code>chardet</code> or <code>charset_normalizer</code>) when repackaged or vendored.
This enables <code>pip</code> and other projects to minimize their vendoring
surface area. The <code>Response.text()</code> and <code>apparent_encoding</code> APIs
will default to <code>utf-8</code> if neither library is present. (<a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a>)</li>
</ul>
<p><strong>Bugfixes</strong></p>
<ul>
<li>Fixed bug in length detection where emoji length was incorrectly
calculated in the request content-length. (<a href="https://redirect.github.com/psf/requests/issues/6589">#6589</a>)</li>
<li>Fixed deserialization bug in JSONDecodeError. (<a href="https://redirect.github.com/psf/requests/issues/6629">#6629</a>)</li>
<li>Fixed bug where an extra leading <code>/</code> (path separator) could lead
urllib3 to unnecessarily reparse the request URI. (<a href="https://redirect.github.com/psf/requests/issues/6644">#6644</a>)</li>
</ul>
<p><strong>Deprecations</strong></p>
<ul>
<li>Requests has officially added support for CPython 3.12 (<a href="https://redirect.github.com/psf/requests/issues/6503">#6503</a>)</li>
<li>Requests has officially added support for PyPy 3.9 and 3.10 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
<li>Requests has officially dropped support for CPython 3.7 (<a href="https://redirect.github.com/psf/requests/issues/6642">#6642</a>)</li>
<li>Requests has officially dropped support for PyPy 3.7 and 3.8 (<a href="https://redirect.github.com/psf/requests/issues/6641">#6641</a>)</li>
</ul>
<p><strong>Documentation</strong></p>
<ul>
<li>Various typo fixes and doc improvements.</li>
</ul>
<p><strong>Packaging</strong></p>
<ul>
<li>Requests has started adopting some modern packaging practices.
The source files for the projects (formerly <code>requests</code>) is now located
in <code>src/requests</code> in the Requests sdist. (<a href="https://redirect.github.com/psf/requests/issues/6506">#6506</a>)</li>
<li>Starting in Requests 2.33.0, Requests will migrate to a PEP 517 build system
using <code>hatchling</code>. This should not impact the average user, but extremely old
versions of packaging utilities may have issues with the new packaging format.</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/requests/commit/d6ebc4a2f1f68b7e355fb7e4dd5ffc0845547f9f"><code>d6ebc4a</code></a> v2.32.0</li>
<li><a href="https://github.com/psf/requests/commit/9a40d1277807f0a4f26c9a37eea8ec90faa8aadc"><code>9a40d12</code></a> Avoid reloading root certificates to improve concurrent performance (<a href="https://redirect.github.com/psf/requests/issues/6667">#6667</a>)</li>
<li><a href="https://github.com/psf/requests/commit/0c030f78d24f29a459dbf39b28b4cc765e2153d7"><code>0c030f7</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6702">#6702</a> from nateprewitt/no_char_detection</li>
<li><a href="https://github.com/psf/requests/commit/555b870eb19d497ddb67042645420083ec8efb02"><code>555b870</code></a> Allow character detection dependencies to be optional in post-packaging steps</li>
<li><a href="https://github.com/psf/requests/commit/d6dded3f00afcf56a7e866cb0732799045301eb0"><code>d6dded3</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6700">#6700</a> from franekmagiera/update-redirect-to-invalid-uri-test</li>
<li><a href="https://github.com/psf/requests/commit/bf24b7d8d17da34be720c19e5978b2d3bf94a53b"><code>bf24b7d</code></a> Use an invalid URI that will not cause httpbin to throw 500</li>
<li><a href="https://github.com/psf/requests/commit/2d5f54779ad174035c5437b3b3c1146b0eaf60fe"><code>2d5f547</code></a> Pin 3.8 and 3.9 runners back to macos-13 (<a href="https://redirect.github.com/psf/requests/issues/6688">#6688</a>)</li>
<li><a href="https://github.com/psf/requests/commit/f1bb07d39b74d6444e333879f8b8a3d9dd4d2311"><code>f1bb07d</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6687">#6687</a> from psf/dependabot/github_actions/github/codeql-act...</li>
<li><a href="https://github.com/psf/requests/commit/60047ade64b0b882cbc94e047198818ab580911e"><code>60047ad</code></a> Bump github/codeql-action from 3.24.0 to 3.25.0</li>
<li><a href="https://github.com/psf/requests/commit/31ebb8102c00f8cf8b396a6356743cca4362e07b"><code>31ebb81</code></a> Merge pull request <a href="https://redirect.github.com/psf/requests/issues/6682">#6682</a> from frenzymadness/pytest8</li>
<li>Additional commits viewable in <a href="https://github.com/psf/requests/compare/v2.31.0...v2.32.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=requests&package-manager=pip&previous-version=2.31.0&new-version=2.32.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 06:00:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4866" class=".btn">#4866</a>
            </td>
            <td>
                <b>
                    Bump Go to 1.22.3 (backport release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump Go to 1.22.3.
See details in #4861.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-21 04:03:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4863" class=".btn">#4863</a>
            </td>
            <td>
                <b>
                    Upgrading the fabric components 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
#### Type of change

- Improvement (improvement to code, performance, etc)

#### Description

I was trying to upgrade the chaincode version from v2.2 to v2.5.4 so I went to the documentation and tried to do the steps mentioned in the documentation. When I tried with those commands I faced different errors. The errors I encountered are couldn't run the orderer container as the orderer was looking for certificates which was not backed up. The opt path in the docker container has no files in it. Instead we have to backup from var directory which includes both the orderer and production folders. In  the peer container we have to mention the name of the fabric network for the chaincode container to start otherwise the chaincode container is not starting. So I fixed all the errors and made a new documentation for upgrading the fabric components and upgrading the capabilities.

#### Additional details
Added upgrading steps for couchdb and fabric-ca also.

#### Related issues

https://github.com/hyperledger/fabric/issues/4862


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-17 16:36:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4861" class=".btn">#4861</a>
            </td>
            <td>
                <b>
                    up go 1.22.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The following changes have been made:
- added new possible error based on platform and Go release
- changed the work with [encoding/json](https://go.dev/pkg/encoding/json/) - https://go.dev/doc/go1.22#minor_library_changes. 
`Marshaling and encoding functionality now escapes '\b' and '\f' characters as \b and \f instead of \u0008 and \u000c`.
- The creators of go overmuch with the change of cover work. So far I have turned on the old flag of cover operation - `GOEXPERIMENT=nocoverageredesign`. I will open a question in the go community. Most likely in the next release of go it will be necessary to remove this flag - https://github.com/golang/go/issues/67427. 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-16 12:32:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4859" class=".btn">#4859</a>
            </td>
            <td>
                <b>
                    add badger as alternative state database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- New feature

#### Description

BadgerDB was added as alternative for GolevelDB state database.
Choosing the better alternative for the GolevelDB was a goal of my research within the paper *"A Journey Towards the Most Efficient State Database For Hyperledger Fabric"*: 

  * [Short version](https://ieeexplore.ieee.org/document/10174970)
  * [Detailed version](https://www.oajaiml.com/uploads/archivepdf/36321188.pdf)

This PR adds Badger because it showed better performance results in comparison with GolevelDB, Bbolt and RocksDB. 

PR satisfies [potential future items of the current Hyperledger Fabric Roadmap](https://wiki.hyperledger.org/display/fabric/Hyperledger+Fabric+Roadmap#:~:text=Replace%20GolevelDB%20with%20faster%20database) where the goal to replace the GolevelDB with faster database is mentioned.
 

#### Additional details

Detailed Hyperledger Fabric performance reports mentioned in the papers above are availiable [here](https://drive.google.com/drive/folders/102_Kgpxsjcog5RNcXPo8MK1dvVYoGODp?usp=sharing). They were made using Hyperledger Caliper tool. The tool was used to measure main performance metrics on HLF peer with default GolevelDB and integrated Badger, Bbolt and RocksDB. More measuring details are described in the aforementioned studies.

To demonstrate Badger's potential advantage over GolevelDB, go benchmarks were added to the packages leveldbhelper and badgerdbhelper respectively. The results measured locally show that Badger has better performance for "*put*" operations than GolevelDB. The output is:

#### GolevelDB
```bash
go test -benchmem -run=^$ -bench ^BenchmarkLevelDBHelper$ github.com/hyperledger/fabric/common/ledger/util/leveldbhelper
goos: darwin
goarch: arm64
pkg: github.com/hyperledger/fabric/common/ledger/util/leveldbhelper
BenchmarkLevelDBHelper/get-leveldb-little-data-10                5452860               189.3 ns/op           108 B/op          4 allocs/op
BenchmarkLevelDBHelper/put-leveldb-10                                673           2768479 ns/op             248 B/op          3 allocs/op
BenchmarkLevelDBHelper/put-leveldb-type-2-10                         415           2560133 ns/op             204 B/op          3 allocs/op
PASS
ok      github.com/hyperledger/fabric/common/ledger/util/leveldbhelper  7.145s
```

#### Badger
```bash
 go test -benchmem -run=^$ -bench ^BenchmarkBadgerDBHelper$ github.com/hyperledger/fabric/common/ledger/util/badgerdbhelper
goos: darwin
goarch: arm64
pkg: github.com/hyperledger/fabric/common/ledger/util/badgerdbhelper
BenchmarkBadgerDBHelper/get-badgerdb-little-data-10          1388515               727.7 ns/op           410 B/op          8 allocs/op
BenchmarkBadgerDBHelper/put-badgerdb-10                           207873              5808 ns/op            1408 B/op         37 allocs/op
BenchmarkBadgerDBHelper/put-badgerdb-type-2-10                171474              7206 ns/op            1477 B/op         37 allocs/op
PASS
ok      github.com/hyperledger/fabric/common/ledger/util/badgerdbhelper 13.984s
```

The changes were tested locally and with GitHub CI/CD.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 19:49:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4858" class=".btn">#4858</a>
            </td>
            <td>
                <b>
                    chore: fix function names in comment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- DELETE MARKDOWN COMMENTS BEFORE SUBMITTING PULL REQUEST. -->

<!--- Provide a descriptive summary of your changes in the Title above. -->

#### Type of change


- Documentation update

#### Description

fix function names in comment

#### Additional details

<!--- Additional implementation details or comments to reviewers. -->
<!--- Summarize how the pull request was tested (if not obvious from commit). -->

#### Related issues

<!--- Include a link to any associated issues, e.g. Github issue or approved rfc. -->

<!---
#### Release Note
If change impacts current users, uncomment Release Note heading and provide
release note text.
Also, copy release note text into the release specific /release_notes file.
-->

<!--
Checklist (DELETE AFTER READING):

- `Signed-off-by` added to commits (required for DCO check to pass)
- Tests have been added/updated (required for bug fixes and features)
- Unit and/or integration tests pass locally
- Run linters and checks locally using 'make checks'
- If change requires documentation updates, make updates in pull request,
  or open a separate issue and provide link
- Squash commits into a single commit, unless a stack of commits is
  intentional to assist reviewers or to preserve review comments.
- For additional contribution guidelines see the project's CONTRIBUTING.md file
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-14 13:09:37 +0000 UTC
    </div>
</div>

