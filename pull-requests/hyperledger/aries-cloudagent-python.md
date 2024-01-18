---
layout: default
title: aries-cloudagent-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-cloudagent-python
---

# aries-cloudagent-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-cloudagent-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2723" class=".btn">#2723</a>
            </td>
            <td>
                <b>
                    Remove exception on connectionless presentation problem report handler
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is to support being able to get callbacks to [vc-authn-oidc](https://github.com/bcgov/vc-authn-oidc) when a user declines the presentation request sent to their agent.

Presently ACA-PY is throwing an exception if the problem report does not contain a connection record.
Remove that exception and allow the recieve_problem_report to continue (and supply None for the connection ID in that case).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 23:16:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2722" class=".btn">#2722</a>
            </td>
            <td>
                <b>
                    Update the SupportedRFCs Document to be up to date
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I'd welcome feedback on this on other things we want to highlight in this document.

@dbluhm @andrewwhitehead @ianco, do you think these AIP 2.0 comments are still accurate:

| RFC | Supported | Notes |
 --- | :--: | -- |
| [0211-route-coordination](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0211-route-coordination)   | :warning:  | Only pre-AIP 2.0 version. Must be updated to use `did:key` for full AIP 2.0 support  |
| [0360-use-did-key](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0360-use-did-key)     | :warning:  |  Creating and resolving `did:key` DIDs is supported, but not all protocols are updated yet to use `did:key`. This is a breaking change for AIP 1.0 -> AIP 2.0.                |
| [0587-encryption-envelope-v2](https://github.com/hyperledger/aries-rfcs/tree/b3a3942ef052039e73cd23d847f42947f8287da2/features/0587-encryption-envelope-v2) | :construction: | Support for the DIDComm V2 envelope format is a work in progress, including the PRs ([AIP-2 base64url consistency](https://github.com/hyperledger/aries-cloudagent-python/pull/1188) and [Small AIP-2 updates](https://github.com/hyperledger/aries-cloudagent-python/pull/1056)) |

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 22:54:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2721" class=".btn">#2721</a>
            </td>
            <td>
                <b>
                    Fix subwallet record removal
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If subwallet initialization fails (for example due to an invalid wallet key: #2682) then the wallet record is meant to be removed. This could fail because a session was not being opened first.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 22:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2720" class=".btn">#2720</a>
            </td>
            <td>
                <b>
                    WIP: Breaking - remove endorser capability to write ledger transactions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                WIP as I am still testing the changes.

I didn't remove the "request endorser to write transaction" flag.  In the author I hardcode to false.  In the endorser I raise an error if the author requests this function.  (Handles the case where the endorser is updated and the author isn't.)

See issue #2711 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 21:44:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2719" class=".btn">#2719</a>
            </td>
            <td>
                <b>
                    Upgrade anoncreds to 0.2.0.dev7
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Used an exact version of the dev pre-release. Figured is would be changed anyway when this becomes non pre-release. 

Fixed some calls to the anoncreds library. Required fetching some additional objects from the wallet. Fixed the unit tests.

These would have been quicker and easier to fix if the unit tests caught them. For some of the unit tests I was able to interact with anoncreds and create objects with it, but for some objects like creating credentials and revocation registries I was mocking the objects. These ended up being the broken calls so only the integration tests caught them.

Would be nice if the unit tests could create all the anoncreds objects instead of mocking them. Will try and do this more when I see the opportunity. 

Changed the devcontainer poetry version to match the version used to upgrade.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 18:28:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2716" class=".btn">#2716</a>
            </td>
            <td>
                <b>
                    Fix incorrect Sphinx search library version reference
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I did test it locally, but I think my process is not picking things like this up.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 00:46:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2715" class=".btn">#2715</a>
            </td>
            <td>
                <b>
                    WIP - Anoncreds schema endorsement
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Work in progress. Opening for visibility.

I think this is working well. I want to manual test more, add some unit tests and add integration tests where the author and endorser are configured with command arguments.

Possibly refactor.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-16 22:51:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2713" class=".btn">#2713</a>
            </td>
            <td>
                <b>
                    Integration test for did:peer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                See issue #2703

Adds a (failing) test for --emit-did-peer-x (not included in regular GHA run)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 19:55:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2712" class=".btn">#2712</a>
            </td>
            <td>
                <b>
                    Update RTD requirements after security vulnerability recorded
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Also updates the generated Read The Docs documentation to the latest.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 18:45:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2710" class=".btn">#2710</a>
            </td>
            <td>
                <b>
                    Enable presentation issuance/verification through vc-api endpoints
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enables presentation issuance and verification using the vc_ld manager and addresses #2693.

There is also 4 new routes included matching the vc-api specification. (minor changes from the `/vc/ldp` endpoints, mostly key names and defaulting to `Ed25519Signature2018` `proofType` for issuance).
@dbluhm could you help me by reviewing the changes I've made to the vc_ld manager and models? You will see I added an if condition in the `verify_presentation` section to enable `assertionMethod` purpose if no challenge is provided, while minimizing the impact on the existing code/workflows. I also improved the presentation models, based on the existing credential ones.

I have a test instance of these changes running [here](https://agent.vc.opsec.id/api/doc#/vc-api).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 17:11:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2707" class=".btn">#2707</a>
            </td>
            <td>
                <b>
                    chore(deps): Bump jinja2 from 3.1.2 to 3.1.3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 3.1.2 to 3.1.3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/releases">jinja2's releases</a>.</em></p>
<blockquote>
<h2>3.1.3</h2>
<p>This is a fix release for the 3.1.x feature branch.</p>
<ul>
<li>Fix for <a href="https://github.com/pallets/jinja/security/advisories/GHSA-h5c8-rqwp-cp95">GHSA-h5c8-rqwp-cp95</a>. You are affected if you are using <code>xmlattr</code> and passing user input as attribute keys.</li>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-3</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/15?closed=1">https://github.com/pallets/jinja/milestone/15?closed=1</a></li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pallets/jinja/blob/main/CHANGES.rst">jinja2's changelog</a>.</em></p>
<blockquote>
<h2>Version 3.1.3</h2>
<p>Released 2024-01-10</p>
<ul>
<li>Fix compiler error when checking if required blocks in parent templates are
empty. :pr:<code>1858</code></li>
<li><code>xmlattr</code> filter does not allow keys with spaces. GHSA-h5c8-rqwp-cp95</li>
<li>Make error messages stemming from invalid nesting of <code>{% trans %}</code> blocks
more helpful. :pr:<code>1918</code></li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pallets/jinja/commit/d9de4bb215fd1cc8092a410fb834c7c4060b1fc1"><code>d9de4bb</code></a> release version 3.1.3</li>
<li><a href="https://github.com/pallets/jinja/commit/50124e16561f17f6c1ec85a692f6551418971cdc"><code>50124e1</code></a> skip test pypi</li>
<li><a href="https://github.com/pallets/jinja/commit/9ea7222ef3f184480be0d0884e30ccfb4172b17b"><code>9ea7222</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/da703f7aae36b1e88baaa20de334d7ff6378fdde"><code>da703f7</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/bce174692547464512383ec40e0f8338b8811983"><code>bce1746</code></a> use trusted publishing</li>
<li><a href="https://github.com/pallets/jinja/commit/7277d8068be593deab3555c7c14f974ada373af1"><code>7277d80</code></a> update pre-commit hooks</li>
<li><a href="https://github.com/pallets/jinja/commit/5c8a10522421270f66376a24ec8e0d6812bc4b14"><code>5c8a105</code></a> Make nested-trans-block exceptions nicer (<a href="https://redirect.github.com/pallets/jinja/issues/1918">#1918</a>)</li>
<li><a href="https://github.com/pallets/jinja/commit/19a55db3b411343309f2faaffaedbb089e841895"><code>19a55db</code></a> Make nested-trans-block exceptions nicer</li>
<li><a href="https://github.com/pallets/jinja/commit/716795349a41d4983a9a4771f7d883c96ea17be7"><code>7167953</code></a> Merge pull request from GHSA-h5c8-rqwp-cp95</li>
<li><a href="https://github.com/pallets/jinja/commit/7dd3680e6eea0d77fde024763657aa4d884ddb23"><code>7dd3680</code></a> xmlattr filter disallows keys with spaces</li>
<li>Additional commits viewable in <a href="https://github.com/pallets/jinja/compare/3.1.2...3.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=3.1.2&new-version=3.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/aries-cloudagent-python/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 21:21:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2706" class=".btn">#2706</a>
            </td>
            <td>
                <b>
                    feat: make VcLdpManager pluggable
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                As a follow up to #2705, this PR implements the example I gave of making `VcLdpManager` pluggable. This may be desirable to, for instance, change the issuance or verification behavior (e.g. using an external service to perform the signature or similar).

This is a bit "heavier" a change than what is proposed in #2348 in the sense that it would require slightly more effort to define the alternate DID lookup mechanism but I think this would still address the same problem it was seeking to solve. Given the straightforwardness of the change required in ACA-Py to support this, I am more in favor of it being handled this way.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 20:55:35 +0000 UTC
    </div>
</div>

