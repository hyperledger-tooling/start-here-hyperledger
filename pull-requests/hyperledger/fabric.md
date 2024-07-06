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
                PR <a href="https://github.com/hyperledger/fabric/pull/4922" class=".btn">#4922</a>
            </td>
            <td>
                <b>
                    Add help command to the make file, to list to be able to list available
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **Added ﻿make help Command**

**Summary**

This change introduces a ﻿make help command to list all available commands provided by the project's Makefile.

**Details**
	•	New Feature: ﻿make help command
	•	Purpose: Improve accessibility and usability by providing a self-documenting feature.
	•	Implementation:
	•	Added a ﻿help target to the Makefile.
	•	The ﻿help target prints out all available Makefile targets with descriptions.
	
	
**Usage**
Run the following command to see all available commands:

```
make help
```

This will output a list of all Makefile targets along with their descriptions, making it easier for developers to understand the available options without needing to read through the entire Makefile.

**Example Output**
```
Available commands:
help            List all commands with documentation
all             Builds all targets and runs all non-integration tests/checks
checks          Runs basic checks along with unit and integration tests
basic-checks    Performs basic checks like license, spelling, trailing spaces and linter
desk-check      Runs linters and verify to test changed packages
help-docs       Generate the command reference docs
check-help-docs Check for outdated command reference documentation
spelling        Check for spelling errors
references      Check for outdated references
license         Check for license headers
trailing-spaces Check for trailing spaces
gotools         Install go tools like golint
check-go-version Check for the correct go version
integration-test Runs the integration tests
integration-test-prereqs Setup prerequisites for integration tests
unit-test       Runs the go-test based unit tests
unit-tests      Alias for unit-test
docker-thirdparty Pull thirdparty docker images
docker-thirdparty-couchdb Pull couchdb docker image
verify          Runs unit tests for only the changed package tree
profile         Runs unit tests for all packages in coverprofile mode (slow)
linter          Runs all code checks
check-deps      Check for vendored dependencies that are no longer used
check-metrics-doc Check for outdated reference documentation
generate-metrics-doc Generate metrics reference documentation
check-swagger   Check for outdated swagger
generate-swagger Generate swagger
protos          Generate all protobuf artifacts based on .proto files
native          Ensures all native binaries are available
tools           Builds all tools
docker          Builds all docker images
release         Builds release packages for the host platform
release-all     Builds release packages for all target platforms
dist-all        Builds release packages for all target platforms
docker-list     Generates a list of docker images that 'make docker' produces
docker-clean    Ensures all docker images are available
docker-tag-latest Re-tags the images made by 'make docker' with the :latest tag
clean           Cleans the build area
clean-all       Cleans the build area and removes persistent state
dist-clean      Clean release packages for all target platforms
release-clean   Clean release packages for all target platforms
scan            Run all security scans
scan-govulncheck Run gosec security scan
```



            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-06 08:53:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4921" class=".btn">#4921</a>
            </td>
            <td>
                <b>
                    Bump certifi from 2023.11.17 to 2024.7.4 in /docs in the pip group across 1 directory
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps the pip group with 1 update in the /docs directory: [certifi](https://github.com/certifi/python-certifi).

Updates `certifi` from 2023.11.17 to 2024.7.4
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/certifi/python-certifi/commit/bd8153872e9c6fc98f4023df9c2deaffea2fa463"><code>bd81538</code></a> 2024.07.04 (<a href="https://redirect.github.com/certifi/python-certifi/issues/295">#295</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/06a2cbf21f345563dde6c28b60e29d57e9b210b3"><code>06a2cbf</code></a> Bump peter-evans/create-pull-request from 6.0.5 to 6.1.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/294">#294</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/13bba02b72bac97c432c277158bc04b4d2a6bc23"><code>13bba02</code></a> Bump actions/checkout from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/293">#293</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/e8abcd0e62b334c164b95d49fcabdc9ecbca0554"><code>e8abcd0</code></a> Bump pypa/gh-action-pypi-publish from 1.8.14 to 1.9.0 (<a href="https://redirect.github.com/certifi/python-certifi/issues/292">#292</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/124f4adf171e15cd9a91a8b6e0325ecc97be8fe1"><code>124f4ad</code></a> 2024.06.02 (<a href="https://redirect.github.com/certifi/python-certifi/issues/291">#291</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/c2196ce5d6ee675b27755a19948480a7823e2c6a"><code>c2196ce</code></a> --- (<a href="https://redirect.github.com/certifi/python-certifi/issues/290">#290</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/fefdeec7588ff1c05214b85a552afcad5fdb51b2"><code>fefdeec</code></a> Bump actions/checkout from 4.1.4 to 4.1.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/289">#289</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/3c5fb1560b826a7f83f1f9750173ff766492c9cf"><code>3c5fb15</code></a> Bump actions/download-artifact from 4.1.6 to 4.1.7 (<a href="https://redirect.github.com/certifi/python-certifi/issues/286">#286</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/4a9569a3eb58db8548536fc16c5c5c7af946a5b1"><code>4a9569a</code></a> Bump actions/checkout from 4.1.2 to 4.1.4 (<a href="https://redirect.github.com/certifi/python-certifi/issues/287">#287</a>)</li>
<li><a href="https://github.com/certifi/python-certifi/commit/1fc808626a895a916b1e4c2b63abae6c5eafdbe3"><code>1fc8086</code></a> Bump peter-evans/create-pull-request from 6.0.4 to 6.0.5 (<a href="https://redirect.github.com/certifi/python-certifi/issues/288">#288</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/certifi/python-certifi/compare/2023.11.17...2024.07.04">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=certifi&package-manager=pip&previous-version=2023.11.17&new-version=2024.7.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-07-05 23:32:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4919" class=".btn">#4919</a>
            </td>
            <td>
                <b>
                    Implement 'osnadmin channel info' subcommand and update tests #4890
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Implemented the osnadmin channel info subcommand to retrieve detailed information about a specific channel from an Ordering Service Node (OSN). This involved modifying the CLI commands and adding corresponding functionality to interact with the channel participation API.

Type of change
New feature
Implemented the osnadmin channel info subcommand to retrieve detailed information about a specific channel from an Ordering Service Node (OSN).

Introduced info subcommand under osnadmin channel to support querying individual channel details.
Updated existing tests and added new tests to cover the new feature and edge cases.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 18:13:28 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4918" class=".btn">#4918</a>
            </td>
            <td>
                <b>
                    fix data race in unit test
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
        Created At 2024-07-04 15:55:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4917" class=".btn">#4917</a>
            </td>
            <td>
                <b>
                    bump golang.org/x/crypto
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix:

Vulnerability found in dependency:
CVE-2023-42818
9.8
Improper Restriction of Excessive Authentication Attempts vulnerability with High severity found
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-04 09:18:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4916" class=".btn">#4916</a>
            </td>
            <td>
                <b>
                    bump go 1.22.5
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
        Created At 2024-07-03 12:38:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4915" class=".btn">#4915</a>
            </td>
            <td>
                <b>
                    bump go.etcd.io/etcd/pkg 3.5.14
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
        Created At 2024-07-02 22:07:56 +0000 UTC
    </div>
</div>

