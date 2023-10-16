---
layout: default
title: fabric-token-sdk
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-token-sdk
---

# fabric-token-sdk <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-token-sdk){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/508" class=".btn">#508</a>
            </td>
            <td>
                <b>
                    add tokengen function to update auditor and issuer certs in dlog pp files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                If the auditor or issuer certificate expires, we have to update it in the token chaincode. This action should *not* change the public parameters, because this would render existing tokens/proofs invalid.

This PR adds a command to the tokengen cli utility to update the auditor and/or issuers certificates in an existing `zkatdlog_pp.json`, without changing the public parameters.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 14:13:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/507" class=".btn">#507</a>
            </td>
            <td>
                <b>
                    use latest idemix
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
        Created At 2023-10-16 09:20:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/506" class=".btn">#506</a>
            </td>
            <td>
                <b>
                    use fsc logger for badger database
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Badger has noisy logs when writing:

```
badger 2023/10/14 14:23:14 INFO: Sent range 21 for iteration: [74720030326639616465313833666639626134363335393737663132626663346364623435333331393839383331323261316135316365383262353663666563313961ffffffffffffffcc, 74720030336166653834326463653735376631373764346131393034656433623436313863323964613630666632383561663537623363613462356437333232613836fffffffffffffffb) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 22 for iteration: [74720065353032323934376132623034663538646431336139373930336430346439336338313935366162653061613463636262333934376663396263663061316435ffffffffffffffdb, 74720066303236363664653166373534643461316234313133613433646162356266333566366662373339326665343466336234656137643464393262663130393631ffffffffffffffdf) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 23 for iteration: [74720062303332613234356530323032346232336434616361303934343439376162386632373766386534613834656537623934626336333566643837643236396632ffffffffffffffe6, 74720063373963346161323736366464376132356539313364333833633665613762386133313538396431316139616137663632333336353338306536393262643736fffffffffffffff1) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 24 for iteration: [74720066373264366464643866636164383063373237643762623063666632366335323630373434393966353631373464663836373538353332656438313432303036ffffffffffffffd9, 74720066626433353233383935346234656333343766636430376465303036633763656264393333313232393736616432626339336466646133626132346361313164ffffffffffffffdd) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 25 for iteration: [74720066626433353233383935346234656333343766636430376465303036633763656264393333313232393736616432626339336466646133626132346361313164ffffffffffffffdd, 74720066643039626431663435636336383637343333366138643134396166663837363837653639613337333232613466623266386532386432343433653732333637ffffffffffffffd3) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 26 for iteration: [74720066643039626431663435636336383637343333366138643134396166663837363837653639613337333232613466623266386532386432343433653732333637ffffffffffffffd3, 74780061616161616161616161616161616161616161616161616161610036323038326361613166373232343633623834343737366630623338326361643630313430353431656463353764336333366638666338643231316465353838fffffffffffffffc) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 27 for iteration: [6964736571ffffffffffffffe7, 74720030303138346335323166643862626532366566383239303263373630326163653761383666353562303134636439366236363934356335646135663538343232ffffffffffffffd5) of size: 1.1 MiB
badger 2023/10/14 14:23:14 INFO: Sent range 28 for iteration: [74780061616161616161616161616161616161616161616161616165630030303138346335323166643862626532366566383239303263373630326163653761383666353562303134636439366236363934356335646135663538343232ffffffffffffffd4, ) of size: 706 KiB
badger 2023/10/14 14:23:14 INFO: ttxdb.SetStatus Sent data of size 40 KiB
```

The output couldn't be controlled, because the badger was being initiated with default options including the default golang logger. 

This PR injects the FSC logger into the badger config, so that the format corresponds to the rest of the logs of the Token SDK and can be controlled via the logging.spec config key (example: `info,token-sdk.ttxdb.badger=warn` will keep 'info' as the standard level, but get rid of the noisy badger logs).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-14 12:49:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/505" class=".btn">#505</a>
            </td>
            <td>
                <b>
                    Bump golang.org/x/net from 0.14.0 to 0.17.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [golang.org/x/net](https://github.com/golang/net) from 0.14.0 to 0.17.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/golang/net/commit/b225e7ca6dde1ef5a5ae5ce922861bda011cfabd"><code>b225e7c</code></a> http2: limit maximum handler goroutines to MaxConcurrentStreams</li>
<li><a href="https://github.com/golang/net/commit/88194ad8ab44a02ea952c169883c3f57db6cf9f4"><code>88194ad</code></a> go.mod: update golang.org/x dependencies</li>
<li><a href="https://github.com/golang/net/commit/2b60a61f1e4cf3a5ecded0bd7e77ea168289e6de"><code>2b60a61</code></a> quic: fix several bugs in flow control accounting</li>
<li><a href="https://github.com/golang/net/commit/73d82efb96cacc0c378bc150b56675fc191894b9"><code>73d82ef</code></a> quic: handle DATA_BLOCKED frames</li>
<li><a href="https://github.com/golang/net/commit/5d5a036a503f8accd748f7453c0162115187be13"><code>5d5a036</code></a> quic: handle streams moving from the data queue to the meta queue</li>
<li><a href="https://github.com/golang/net/commit/350aad2603e57013fafb1a9e2089a382fe67dc80"><code>350aad2</code></a> quic: correctly extend peer's flow control window after MAX_DATA</li>
<li><a href="https://github.com/golang/net/commit/21814e71db756f39b69fb1a3e06350fa555a79b1"><code>21814e7</code></a> quic: validate connection id transport parameters</li>
<li><a href="https://github.com/golang/net/commit/a600b3518eed7a9a4e24380b4b249cb986d9b64d"><code>a600b35</code></a> quic: avoid redundant MAX_DATA updates</li>
<li><a href="https://github.com/golang/net/commit/ea633599b58dc6a50d33c7f5438edfaa8bc313df"><code>ea63359</code></a> http2: check stream body is present on read timeout</li>
<li><a href="https://github.com/golang/net/commit/ddd8598e5694aa5e966e44573a53e895f6fa5eb2"><code>ddd8598</code></a> quic: version negotiation</li>
<li>Additional commits viewable in <a href="https://github.com/golang/net/compare/v0.14.0...v0.17.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=golang.org/x/net&package-manager=go_modules&previous-version=0.14.0&new-version=0.17.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/fabric-token-sdk/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-11 23:13:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-token-sdk/pull/504" class=".btn">#504</a>
            </td>
            <td>
                <b>
                    Removed tx callback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Make External wallet signing more flexible
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-10 14:01:15 +0000 UTC
    </div>
</div>

