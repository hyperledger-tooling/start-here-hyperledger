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
                PR <a href="https://github.com/hyperledger/fabric/pull/4604" class=".btn">#4604</a>
            </td>
            <td>
                <b>
                    Bump jinja2 from 3.0.3 to 3.1.3 in /docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [jinja2](https://github.com/pallets/jinja) from 3.0.3 to 3.1.3.
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
<h2>3.1.2</h2>
<p>This is a fix release for the <a href="https://github.com/pallets/jinja/releases/tag/3.1.0">3.1.0</a> feature release.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-2">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-2</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/13?closed=1">https://github.com/pallets/jinja/milestone/13?closed=1</a></li>
</ul>
<h2>3.1.1</h2>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-1">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-1</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/12?closed=1">https://github.com/pallets/jinja/milestone/12?closed=1</a></li>
</ul>
<h2>3.1.0</h2>
<p>This is a feature release, which includes new features and removes previously deprecated features. The 3.1.x branch is now the supported bugfix branch, the 3.0.x branch has become a tag marking the end of support for that branch. We encourage everyone to upgrade, and to use a tool such as <a href="https://pypi.org/project/pip-tools/">pip-tools</a> to pin all dependencies and control upgrades. We also encourage upgrading to MarkupSafe 2.1.1, the latest version at this time.</p>
<ul>
<li>Changes: <a href="https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-0">https://jinja.palletsprojects.com/en/3.1.x/changes/#version-3-1-0</a></li>
<li>Milestone: <a href="https://github.com/pallets/jinja/milestone/8?closed=1">https://github.com/pallets/jinja/milestone/8?closed=1</a></li>
<li>MarkupSafe changes: <a href="https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1">https://markupsafe.palletsprojects.com/en/2.1.x/changes/#version-2-1-1</a></li>
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
<h2>Version 3.1.2</h2>
<p>Released 2022-04-28</p>
<ul>
<li>Add parameters to <code>Environment.overlay</code> to match <code>__init__</code>.
:issue:<code>1645</code></li>
<li>Handle race condition in <code>FileSystemBytecodeCache</code>. :issue:<code>1654</code></li>
</ul>
<h2>Version 3.1.1</h2>
<p>Released 2022-03-25</p>
<ul>
<li>The template filename on Windows uses the primary path separator.
:issue:<code>1637</code></li>
</ul>
<h2>Version 3.1.0</h2>
<p>Released 2022-03-24</p>
<ul>
<li>
<p>Drop support for Python 3.6. :pr:<code>1534</code></p>
</li>
<li>
<p>Remove previously deprecated code. :pr:<code>1544</code></p>
<ul>
<li><code>WithExtension</code> and <code>AutoEscapeExtension</code> are built-in now.</li>
<li><code>contextfilter</code> and <code>contextfunction</code> are replaced by
<code>pass_context</code>. <code>evalcontextfilter</code> and
<code>evalcontextfunction</code> are replaced by <code>pass_eval_context</code>.
<code>environmentfilter</code> and <code>environmentfunction</code> are replaced
by <code>pass_environment</code>.</li>
<li><code>Markup</code> and <code>escape</code> should be imported from MarkupSafe.</li>
<li>Compiled templates from very old Jinja versions may need to be
recompiled.</li>
<li>Legacy resolve mode for <code>Context</code> subclasses is no longer
supported. Override <code>resolve_or_missing</code> instead of</li>
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
<li>Additional commits viewable in <a href="https://github.com/pallets/jinja/compare/3.0.3...3.1.3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=jinja2&package-manager=pip&previous-version=3.0.3&new-version=3.1.3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger/fabric/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-11 19:35:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4603" class=".btn">#4603</a>
            </td>
            <td>
                <b>
                    Enhance queryapproved cmd to query all approved chaincode definitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR enhances queryapproved command to query all approved chaincode definitions.
See https://github.com/hyperledger/fabric/issues/4564 for the detail.

Also, this fixes an unstable test code on _lifecycle functions on queryapproved to query all approved chaincode definitions.

#### Type of change

- New feature
- Bug fix

#### Description

As a sub-task stemming from issue #4564, this enhances queryapproved command to query all approved chaincode definitions.
Also, this fixes an unstable test code on _lifecycle functions on queryapproved to query all approved chaincode definitions.

Once this patch is merged, I will submit patches to update the documantations:


#### Addtional Details

The example of output when executing the enhanced queryapproved in the implementation:

```
$ peer lifecycle chaincode queryapproved -C mychannel
Approved chaincode definition on channel 'mychannel':
name: basic2, sequence: 2, version: 1.0.1, init-required: false, package-id: basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a, endorsement plugin: escc, validation plugin: vscc
name: basic, sequence: 1, version: 1.0.1, init-required: false, package-id: basic_1.0.1:f4babb5fd92c0ab4bce8c6ac30ca7bbb4a55e6c37774582d11639b6036ae0273, endorsement plugin: escc, validation plugin: vscc
name: basic2, sequence: 1, version: 1.0.1, init-required: false, package-id: basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a, endorsement plugin: escc, validation plugin: vscc
```

```
 $ peer lifecycle chaincode queryapproved -C mychannel -O json
{
        "approved_chaincode_definitions": [
                {
                        "name": "basic2",
                        "sequence": 2,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a"
                                        }
                                }
                        }
                },
                {
                        "name": "basic",
                        "sequence": 1,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic_1.0.1:f4babb5fd92c0ab4bce8c6ac30ca7bbb4a55e6c37774582d11639b6036ae0273"
                                        }
                                }
                        }
                },
                {
                        "name": "basic2",
                        "sequence": 1,
                        "version": "1.0.1",
                        "endorsement_plugin": "escc",
                        "validation_plugin": "vscc",
                        "validation_parameter": "EiAvQ2hhbm5lbC9BcHBsaWNhdGlvbi9FbmRvcnNlbWVudA==",
                        "collections": {},
                        "source": {
                                "Type": {
                                        "LocalPackage": {
                                                "package_id": "basic2_1.0.1:dae4dca432d56265e87e6416b602b40e94e7f7cdc177031abda1c81d9ed4258a"
                                        }
                                }
                        }
                }
        ]
}
```

#### Releated PRs

- https://github.com/hyperledger/fabric-protos/pull/196
- https://github.com/hyperledger/fabric/pull/4592


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-10 10:14:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4602" class=".btn">#4602</a>
            </td>
            <td>
                <b>
                    added time to the test to make it long enough
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
        Created At 2024-01-10 05:32:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4601" class=".btn">#4601</a>
            </td>
            <td>
                <b>
                    Upgrade the CouchDB used to v3.3.3 (release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to CouchDB v3.3.3.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 14:19:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4600" class=".btn">#4600</a>
            </td>
            <td>
                <b>
                    Upgrade the CouchDB used to v3.3.3 (release-2.2)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Move to CouchDB v3.3.3.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 14:18:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4599" class=".btn">#4599</a>
            </td>
            <td>
                <b>
                    Fix doc typo
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fix remaining doc typo from prior commit.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 14:05:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4598" class=".btn">#4598</a>
            </td>
            <td>
                <b>
                    docs: fix typos (backport release-2.5)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                docs: fix typos
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-09 13:29:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4597" class=".btn">#4597</a>
            </td>
            <td>
                <b>
                    docs: fix typos
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
        Created At 2024-01-09 08:57:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4596" class=".btn">#4596</a>
            </td>
            <td>
                <b>
                    find and fix error
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Often fails this [test](https://github.com/hyperledger/fabric/blob/main/integration/raft/config_test.go#L1258) 
- https://github.com/hyperledger/fabric/actions/runs/7493668256/job/20399967195
- https://github.com/hyperledger/fabric/actions/runs/7483402876/job/20368656381
- https://github.com/hyperledger/fabric/actions/runs/7462441029/job/20304890927

Failure occurs when [waiting for the orderer to delete a channel](https://github.com/hyperledger/fabric/blob/main/integration/raft/config_test.go#L1336) 

[Here is an explanation](https://github.com/hyperledger/fabric/blob/main/integration/raft/config_test.go#L1314): why they added the removal of the channel with orderer

I'll describe what's going on:
- the orderer is in a constant cycle periodically performing the [function](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L339)
- send a command to remove channel. It passes the following functions [serveRemove](https://github.com/hyperledger/fabric/blob/main/orderer/common/channelparticipation/restapi.go#L360), [RemoveChannel](https://github.com/hyperledger/fabric/blob/main/orderer/common/multichannel/registrar.go#L769) (`r.lock` monopole is taken in this function), [Halt](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L226) (the actual removal of the channel is expected [here](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L228))
- let's return to the main loop, this is where the actual deletion should take place, it wants to execute the function [SwitchFollowerToChain](https://github.com/hyperledger/fabric/blob/main/orderer/common/follower/follower_chain.go#L357), but she can't, she needs a `r.lock` monopole.

==================================

The error in the raft tests is due to the struggle for monopoly control of r.lock in the SwitchChainToFollower and RemoveChannel functions.

RemoveChannel grabs monopoly control and waits for the channel to terminate. During termination, SwitchChainToFollower tries to grab monopoly control and fails.

Here is my variant of solving the error. If someone suggests a more correct and reddish way, it would be great.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-08 17:23:07 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4595" class=".btn">#4595</a>
            </td>
            <td>
                <b>
                    Upgrade the CouchDB used to v3.3.3 as per CVE-2023-45725.
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

Move to CouchDB v3.3.3.  There's a [security vulnerability](https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2023-45725) with CouchDB v3.3.2.  I **think** this only impacts the testing that happens to Fabric, but this PR is a good way to be sure.

#### Additional details

I have tested that CouchDB v3.3.3 is not majorly functionally different than CouchDB v3.3.2. (See its [Release Notes](https://docs.couchdb.org/en/stable/whatsnew/3.3.html#release-3-3-3)).  There have been no breaking API changes in v3.3.3, only bug fixes and security patches.

I would suggest backporting this to Fabric v2.5.x because it's only a CouchDB Patch.

#### Related issues

Tracked by https://github.com/hyperledger/fabric/issues/4594
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-05 15:34:04 +0000 UTC
    </div>
</div>

