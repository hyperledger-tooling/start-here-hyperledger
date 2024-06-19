---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Initial checkin for a new identity & policy contract family
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### THIS CONTRACT FAMILY IS WORK IN PROGRESS

Initial commit for a new contract family for identity and policy. An identity is a contract that manages a collection of hierarchically generated keys. As a result, a standard format for keys would involve <contract_id>/<key1>/key2>/.... 

The policy support is incomplete. Documentation for (and serialization/deserialization of) verifiable credentials and verifiable presentations is available. 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 22:19:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Add jupyter notebook interface for the digital asset (images) contracts
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds Jupyter notebook support for creating a token issuer for the digital asset contract family. The digital asset contract family is a demonstration contract that creates tokens and guardian objects for 24bit bitmap images. 

The notebooks for DA use widgets for uploading the image file and creating the tokens. This is a new approach.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 16:30:37 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/51" class=".btn">#51</a>
            </td>
            <td>
                <b>
                    Bump private-data-objects from `6a30f64` to `1fb32e8`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span>
            </td>
            <td>
                Bumps [private-data-objects](https://github.com/hyperledger-labs/private-data-objects) from `6a30f64` to `1fb32e8`.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/1fb32e8748cd94874851a6aee4d8ab952773d97b"><code>1fb32e8</code></a> replace WASM_MEM_CONFIG with PDO_MEMORY_CONFIG in docker tools</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/4bb3027e91648607f34de23f3b01b8334e081385"><code>4bb3027</code></a> Update documentation for the change to PDO_MEMORY_CONFIG environment/build va...</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/70bf620ab7801f521f715b33fbb2845b2a9e50c1"><code>70bf620</code></a> Simplify specification and use of the various memory configurations</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/214e656641b12bc769580e53ae6b436378ac1ac3"><code>214e656</code></a> small docker fixes to fix loglevel switch in tools</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/37ab11beaa4b5f68eb237ef2ac3deacdd12c5380"><code>37ab11b</code></a> Change the default value of PDO_DEBUG_BUILD to 1.</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/b6fd980ca3e89f1e2446850980db817354bed82e"><code>b6fd980</code></a> Port eservice build updates to pservice.</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/02ee00a93e4a96184a69ba156eeb8411f5a97bea"><code>02ee00a</code></a> Add sgx flag checks to pservice.</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/1f34ce025e0b9c26155d2c614a0e729535e83257"><code>1f34ce0</code></a> Update PDO TP with more sgx attestation checks.</li>
<li><a href="https://github.com/hyperledger-labs/private-data-objects/commit/c876a5eae6866837dca5c01be4101d6b2b523e30"><code>c876a5e</code></a> Make the sgx debug flag dependent on PDO_DEBUG_BUILD.</li>
<li>See full diff in <a href="https://github.com/hyperledger-labs/private-data-objects/compare/6a30f6426883c22760dd9bd5eef452e9db5b3692...1fb32e8748cd94874851a6aee4d8ab952773d97b">compare view</a></li>
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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)


</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-18 01:28:54 +0000 UTC
    </div>
</div>

