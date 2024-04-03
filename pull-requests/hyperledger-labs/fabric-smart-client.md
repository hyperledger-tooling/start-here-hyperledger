---
layout: default
title: fabric-smart-client
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-smart-client
---

# fabric-smart-client <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-smart-client){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/541" class=".btn">#541</a>
            </td>
            <td>
                <b>
                    Bump github.com/quic-go/quic-go from 0.38.2 to 0.42.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [github.com/quic-go/quic-go](https://github.com/quic-go/quic-go) from 0.38.2 to 0.42.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/quic-go/quic-go/releases">github.com/quic-go/quic-go's releases</a>.</em></p>
<blockquote>
<h2>v0.42.0</h2>
<h2>New Features</h2>
<ul>
<li>added a qlog tracer for events that happen before / outside of established connection: <a href="https://redirect.github.com/quic-go/quic-go/issues/4305">#4305</a></li>
</ul>
<h2>Notable Changes</h2>
<ul>
<li>added a <code>ClientHelloInfo.AddrVerified</code> field: <a href="https://redirect.github.com/quic-go/quic-go/issues/4360">#4360</a></li>
<li>move callback controlling address verification (<code>VerifySourceAddress</code>) to the <code>Transport</code>: <a href="https://redirect.github.com/quic-go/quic-go/issues/4253">#4253</a> and <a href="https://redirect.github.com/quic-go/quic-go/issues/4362">#4362</a></li>
<li>connections that are closed before being accepted are not removed from the server's accept queue: <a href="https://redirect.github.com/quic-go/quic-go/issues/4245">#4245</a></li>
<li>http3: added a <code>RoundTripOpt.CheckSettings</code> callback to check the server's SETTINGS: <a href="https://redirect.github.com/quic-go/quic-go/issues/4355">#4355</a></li>
<li>http3: send the HTTP/3 settings value for Extended CONNECT (RFC 9220): <a href="https://redirect.github.com/quic-go/quic-go/issues/4341">#4341</a></li>
<li>http3: don't modify the user's <code>quic.Config</code> to enable QUIC datagram support: <a href="https://redirect.github.com/quic-go/quic-go/issues/4340">#4340</a></li>
</ul>
<h2>Fixes</h2>
<ul>
<li>mitigate a memory exhaustion attack against QUIC's connection ID mechanism: <a href="https://redirect.github.com/quic-go/quic-go/issues/4369">#4369</a></li>
<li>don't delay acknowledgments for packets during the handshake: <a href="https://redirect.github.com/quic-go/quic-go/issues/4279">#4279</a></li>
<li>fix deadlock when closing both <code>Listener</code> and <code>Transport</code>: <a href="https://redirect.github.com/quic-go/quic-go/issues/4332">#4332</a></li>
<li>fix handling of IPv4-mapped IPv6 addresses: <a href="https://redirect.github.com/quic-go/quic-go/issues/4309">#4309</a></li>
<li>fix duplicate logging of the <code>key_discarded</code> event for Handshake packets: <a href="https://redirect.github.com/quic-go/quic-go/issues/4274">#4274</a></li>
<li>send CONNECTION_REFUSED when refusing connections: <a href="https://redirect.github.com/quic-go/quic-go/issues/4250">#4250</a></li>
<li>http3: tighten validation logic for the :protocol pseudo header: <a href="https://redirect.github.com/quic-go/quic-go/issues/4261">#4261</a></li>
</ul>
<h2>What's Changed</h2>
<ul>
<li>remove shutdown method on the Connection by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4249">quic-go/quic-go#4249</a></li>
<li>send the CONNECTION_REFUSED error when refusing a connection by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4250">quic-go/quic-go#4250</a></li>
<li>don't remove closed connections from the server's accept queue by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4245">quic-go/quic-go#4245</a></li>
<li>handshake: unexport Set{Read,Write}Key methods on the cryptoSetup by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4254">quic-go/quic-go#4254</a></li>
<li>handshake: fix documentation for updatableAEAD.SetWriteKey by <a href="https://github.com/putyWang"><code>@​putyWang</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4256">quic-go/quic-go#4256</a></li>
<li>add Transport config options to limit the number of handshakes by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4248">quic-go/quic-go#4248</a></li>
<li>remove the RequireAddressValidation callback from the Config by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4253">quic-go/quic-go#4253</a></li>
<li>fix incorrect statement about connection ID lengths in the Transport by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4247">quic-go/quic-go#4247</a></li>
<li>remove unneeded nil check for new connections in the server by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4260">quic-go/quic-go#4260</a></li>
<li>ci: update to Go 1.22rc2 by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4267">quic-go/quic-go#4267</a></li>
<li>fix flaky handshake limiting test by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4270">quic-go/quic-go#4270</a></li>
<li>http3: only use :protocol pseudo-header for Extended CONNECT by <a href="https://github.com/taoso"><code>@​taoso</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4261">quic-go/quic-go#4261</a></li>
<li>fix flaky accept queue test by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4280">quic-go/quic-go#4280</a></li>
<li>fix flaky handshake limiting test by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4281">quic-go/quic-go#4281</a></li>
<li>only log the discarding of Handshake keys once by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4274">quic-go/quic-go#4274</a></li>
<li>testutils: add a perspective function parameter to ComposeInitialPacket by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4276">quic-go/quic-go#4276</a></li>
<li>fix flaky outgoing streams map test by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4283">quic-go/quic-go#4283</a></li>
<li>wire: remove FrameParser interface, expose FrameParser struct by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4284">quic-go/quic-go#4284</a></li>
<li>ackhandler: remove unused RTTStats from the received packet handler by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4287">quic-go/quic-go#4287</a></li>
<li>testutils: make the package public by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4290">quic-go/quic-go#4290</a></li>
<li>ci: remove unused depguard check for qtls by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4291">quic-go/quic-go#4291</a></li>
<li>ci: make Codecov ignore testutils and testdata by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4292">quic-go/quic-go#4292</a></li>
<li>testutils: expose aliases for all frames by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4293">quic-go/quic-go#4293</a></li>
<li>ackhandler: don't delay ACKs for Initial and Handshake packets by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4288">quic-go/quic-go#4288</a></li>
<li>protocol: rename VersionNumber to Version by <a href="https://github.com/marten-seemann"><code>@​marten-seemann</code></a> in <a href="https://redirect.github.com/quic-go/quic-go/pull/4295">quic-go/quic-go#4295</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/quic-go/quic-go/commit/4a99b816ae3ab03ae5449d15aac45147c85ed47a"><code>4a99b81</code></a> close connection when an abnormally large number of frames are queued (<a href="https://redirect.github.com/quic-go/quic-go/issues/4369">#4369</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/9971fedd42e9cb853d05fa94809d84743ffa010f"><code>9971fed</code></a> use Transport.VerifySourceAddress to control the Retry Mechanism (<a href="https://redirect.github.com/quic-go/quic-go/issues/4362">#4362</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/497d3f58a556ea2aea596609e464e4f0b45b8031"><code>497d3f5</code></a> http3: add a RoundTripOpt to check the server's SETTINGS frame (<a href="https://redirect.github.com/quic-go/quic-go/issues/4355">#4355</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/ca787d6f0095a2e192792cf3a49f4f1ec06920f7"><code>ca787d6</code></a> add an AddrVerified field to the ClientHelloInfo (<a href="https://redirect.github.com/quic-go/quic-go/issues/4360">#4360</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/f1476390f2c161a66ec51a1b39b81f8e3e2407f6"><code>f147639</code></a> update gomock to v0.4.0 (<a href="https://redirect.github.com/quic-go/quic-go/issues/4361">#4361</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/06b421411d88a805723eb01321555a205e6ead9c"><code>06b4214</code></a> remove unused ReceiveStream.CloseRemote method (<a href="https://redirect.github.com/quic-go/quic-go/issues/4357">#4357</a>)</li>
<li><a href="https://github.com/quic-go/quic-go/commit/5fd5d7770dfcf7361337dccc57f6e56ea6a33c56"><code>5fd5d77</code></a> Merge pull request <a href="https://redirect.github.com/quic-go/quic-go/issues/4305">#4305</a> from quic-go/qlog-tracer</li>
<li><a href="https://github.com/quic-go/quic-go/commit/30e01b9524a4a9fbbb285d2280a31ac4c427d0bd"><code>30e01b9</code></a> use the transport tracer in integration tests</li>
<li><a href="https://github.com/quic-go/quic-go/commit/55c05aceed4bcc47219058f8d777076bb844815c"><code>55c05ac</code></a> qlog: log sent packets outside of a QUIC connection</li>
<li><a href="https://github.com/quic-go/quic-go/commit/aff90a6ffa3b09c73386f8980d67edc3f32679a3"><code>aff90a6</code></a> qlog: log sent Version Negotiation packets</li>
<li>Additional commits viewable in <a href="https://github.com/quic-go/quic-go/compare/v0.38.2...v0.42.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=github.com/quic-go/quic-go&package-manager=go_modules&previous-version=0.38.2&new-version=0.42.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-smart-client/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-02 14:23:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-smart-client/pull/540" class=".btn">#540</a>
            </td>
            <td>
                <b>
                    Test replicas
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
        Created At 2024-03-27 13:00:43 +0000 UTC
    </div>
</div>

