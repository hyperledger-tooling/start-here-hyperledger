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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2705" class=".btn">#2705</a>
            </td>
            <td>
                <b>
                    feat: inject profile
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds the Profile to the injection context. This enables creating a `ClassProvider` for a class that takes a profile in its init method:

```python
class ExamplePluggable:
    def __init__(self, profile: Profile):
        self.profile = profile
    def do_something(self):
        self.profile.notify("some:event", {"with": "data"})

async def setup(context: InjectionContext):
    context.injector.bind_provider(
        ExamplePluggable,
        ClassProvider(ExamplePluggable, ClassProvider.Inject(Profile))
    )

# ... Somewhere else ...
plugged_in = profile.inject(ExamplePluggable)
plugged_in.do_something()
```

It's a common pattern to create a class with a profile instance. This will make it easier to turn some of these components into pluggable components. For example, the `VcLdpManager`. At the moment, it's created directly where it's needed:

```python
manager = VcLdpManager(self.profile)
# do something with manager
```

With this change, I can create an (override-able) class provider for VcLdpManager, which changes the above into:

```python
manager = self.profile.inject(VcLdpManager)
# do something with manager
```

The only way this could be done previously was by binding providers in the Profile init method itself. This made it more difficult to make more components pluggable.

Side note: it's critical that the profile instance be injected as a weak reference or it will never be "finalized" (garbage collected) in multitenant contexts.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 14:56:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2704" class=".btn">#2704</a>
            </td>
            <td>
                <b>
                    fix: minor type hint corrections for VcLdpManager
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                These are some really minor fixes just to make type checking happy and to clarify the use of some values in the VcLdpManager.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 13:18:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2700" class=".btn">#2700</a>
            </td>
            <td>
                <b>
                    Update legacy bcgovimages references.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Resolves: #2118 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 19:48:07 +0000 UTC
    </div>
</div>

