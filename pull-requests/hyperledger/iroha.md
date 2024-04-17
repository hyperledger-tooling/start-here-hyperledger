---
layout: default
title: iroha
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha
---

# iroha <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4458" class=".btn">#4458</a>
            </td>
            <td>
                <b>
                    Feature/sup 10039/update branch ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 11:15:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4457" class=".btn">#4457</a>
            </td>
            <td>
                <b>
                    [refactor] #3240: Guard against secrets leakage
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Refactor</span>
            </td>
            <td>
                ## Description

* Added `Secret` to `PrivateKey`. Access to inner `PrivateKeyInner` now requires import of `ExposeSecret` trait via `expose_secret` method
* `Display`, `Debug` and `Serialize` implementations for `PrivateKey` now returns `"[REDACTED]"`
* Added `ExposedPrivateKey` wrapper which can be formatted and serialized as usual
* Note that I don't used `secrecy` crate because it requires to implement `Zeroize` trait, but inner key struct (`ed25519_dalek::SigningKey`) implement only `ZeroizeOnDrop`, and not `Zeroize`. So I used modified version of `Secret` which requires `ZeroizeOnDrop` instead of `Zeroize`. This potentially could be controversal, so any suggestions are welcome

### Linked issue

Closes #3240

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 11:09:20 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4456" class=".btn">#4456</a>
            </td>
            <td>
                <b>
                    [feature] #3470, #4299, #4300: improve config debug-ability
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Enhancement</span><span class="chip">iroha2</span><span class="chip">api-changes</span><span class="chip">config-changes</span><span class="chip">UI</span>
            </td>
            <td>
                ### Description

This PR contains a major improvement of the work done in https://github.com/hyperledger/iroha/pull/4239. This is a big step towards better debug-ability of Iroha configuration system due to better errors. And yet, there are still many things to improve further!

Key points:

- New `ConfigReader` API, which handles configuration sources in a dynamic manner rather than relying on `serde` completely, thus giving high flexibility in how to handle different cases. It is also built targeting Iroha domain specifically and doesn't have any extra stuff. Much less boilerplate.
- Heavy use of `error_stack` crate, which gives higher control over errors reporting than `eyre` does.
- `--trace-config` works! Uses `log` & `stderrlog` crates for it. Seems to be not a heavy solution for this. It is completely separate from `tracing` stack.

### Further enhancements

There are still many things that might be improved.

- Enhance use of attachments API provided by `error_stack`:
    - Use hooks to colour them conditionally
    - Attach hints and suggestions
    - Unify attachments further as specific structs, not just `format!`
- Use spans to config files, and build reports showing the actual file contents
- Fine-tune API of `ConfigReader`, use better naming and abstractions, perhaps.
- Optimise internals of `ConfigReader`. There is lots of naive code and extra allocations.
- Find a way to reduce extra context changes in `error_stack`. Sometimes it would be really cool to just "forward" underlying context without changing it, but currently it's how `error_stack` is designed. So, we have sometimes stacks like "Failed to load config -> Failed to load config -> failed to read file system -> ..."
- Possibly, introduce a `slim` compile feature for Iroha, which will remove `--trace-config` support alongside with `log` & `stderrlog` dependencies, and more
- Use a single multihash string for private keys, thus removing necessity to set private keys in env as two separate variables (e.g. `PRIVATE_KEY_ALGORITHM` + `PRIVATE_KEY_PAYLOAD`, and removing cratchy `env_custom` API from `ConfigReader`
    - https://github.com/hyperledger/iroha/issues/4412
- Migrate to Axum, finally! Errors handling in Torii might be improved a lot.
    - https://github.com/hyperledger/iroha/issues/3776

### Linked isues

Closes #3470, #4299, #4300

### Gallery

_Note: I've changed some bits after making these screenshots._

<details>

<summary>Some terminal screenshots</summary>

<img width="758" alt="Pasted image 20240417100106" src="https://github.com/hyperledger/iroha/assets/43530070/22189dd4-27e1-4793-a1cd-b53150d2eed7">

<img width="802" alt="Pasted image 20240417160528" src="https://github.com/hyperledger/iroha/assets/43530070/6426ef25-602b-437a-9eae-c6404b03c914">

<img width="651" alt="Pasted image 20240417160759" src="https://github.com/hyperledger/iroha/assets/43530070/292c5fa7-6900-4abb-a1f3-3d5b88f42ad1">

<img width="839" alt="Pasted image 20240417160900" src="https://github.com/hyperledger/iroha/assets/43530070/3eeb42e9-7d18-48ff-9390-fc79f7a6f56f">

<img width="659" alt="Pasted image 20240417161142" src="https://github.com/hyperledger/iroha/assets/43530070/1fda2bd1-3b2c-4067-9d9c-b63630e9be5f">

<img width="725" alt="Pasted image 20240417161212" src="https://github.com/hyperledger/iroha/assets/43530070/f33c9cd6-8456-451b-9aa0-bf2e7154d803">

<img width="878" alt="Pasted image 20240417161247" src="https://github.com/hyperledger/iroha/assets/43530070/292d7cc8-4356-4225-8b04-1dec96ed4316">

<img width="732" alt="Pasted image 20240417161611" src="https://github.com/hyperledger/iroha/assets/43530070/fe27e24f-e975-4e12-bcca-8120f4d6c93f">

<img width="1146" alt="Pasted image 20240417162020" src="https://github.com/hyperledger/iroha/assets/43530070/04d9a524-ad47-4d9b-be2f-c3516a7b4997">

</details>

### TODO

- [ ] Document internals of `iroha_config_base`
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-17 07:54:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4455" class=".btn">#4455</a>
            </td>
            <td>
                <b>
                    [ci] Remove arjentix from CODEOWNERS
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
        Created At 2024-04-17 06:10:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4454" class=".btn">#4454</a>
            </td>
            <td>
                <b>
                    [ci]: Update iroha2 stable/lts branch workflows triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                Update workflows triggers for iroha2 `stable/lts` branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 14:45:05 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4453" class=".btn">#4453</a>
            </td>
            <td>
                <b>
                    Feature/sup 10039/update branch ci
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 14:32:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4452" class=".btn">#4452</a>
            </td>
            <td>
                <b>
                    [ci]: Update iroha2 main branch workflows triggers
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                
### Description of the Change


Update workflows triggers for iroha2 `main` branch
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 14:32:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4451" class=".btn">#4451</a>
            </td>
            <td>
                <b>
                    Prepare updates for iroha1 CI new main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!-- You will not see HTML commented line in Pull Request body -->
<!-- Optional sections may be omitted. Just remove them or write None -->

<!-- ### Requirements -->
<!-- * Filling out the template is required. Any pull request that does not include enough information to be reviewed in a timely manner may be closed at the maintainers' discretion. -->
<!-- * All new code must have code coverage above 70% (https://docs.codecov.io/docs/about-code-coverage). -->
<!-- * CI builds must be passed. -->
<!-- * Critical and blocker issues reported by Sorabot must be fixed. -->
<!-- * Branch must be rebased onto base branch (https://soramitsu.atlassian.net/wiki/spaces/IS/pages/11173889/Rebase+and+merge+guide). -->


### Description of the Change

<!-- We must be able to understand the design of your change from this description. If we can't get a good idea of what the code will be doing from the description here, the pull request may be closed at the maintainers' discretion. -->
<!-- Keep in mind that the maintainer reviewing this PR may not be familiar with or have worked with the code here recently, so please walk us through the concepts. -->

### Benefits

<!-- What benefits will be realized by the code change? -->

### Possible Drawbacks 

<!-- What are the possible side-effects or negative impacts of the code change? -->
<!-- If no drawbacks, explicitly mention this (write None) -->

### Usage Examples or Tests *[optional]*

<!-- Point reviewers to the test, code example or documentation which shows usage example of this feature -->

### Alternate Designs *[optional]*

<!-- Explain what other alternates were considered and why the proposed version was selected -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 11:26:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4450" class=".btn">#4450</a>
            </td>
            <td>
                <b>
                    [chore] #4433: Reflect branch changes in files
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

Replace references to `iroha2-dev` with `main`, and `iroha2-stable` with `stable`. Leave `iroha2-lts` untouched for now, delete later.

### Linked issue

Related to #4433.

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-16 09:56:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4449" class=".btn">#4449</a>
            </td>
            <td>
                <b>
                    Bump sha256 from 1.4.0 to 1.5.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [sha256](https://github.com/baoyachi/sha256-rs) from 1.4.0 to 1.5.0.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/baoyachi/sha256-rs/commit/4184f8ef58a6f148f1dda5c83dcf2a98962f541e"><code>4184f8e</code></a> Update Cargo.toml</li>
<li><a href="https://github.com/baoyachi/sha256-rs/commit/70471a85cd4ab8a86605a6e5bddf6f09022afb3c"><code>70471a8</code></a> Merge pull request <a href="https://redirect.github.com/baoyachi/sha256-rs/issues/21">#21</a> from baoyachi/support_char_type</li>
<li><a href="https://github.com/baoyachi/sha256-rs/commit/5671f6cf77235f6e8bbff90913b4f992e8019185"><code>5671f6c</code></a> support char type</li>
<li>See full diff in <a href="https://github.com/baoyachi/sha256-rs/compare/1.4.0...1.5.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=sha256&package-manager=cargo&previous-version=1.4.0&new-version=1.5.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:29:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4448" class=".btn">#4448</a>
            </td>
            <td>
                <b>
                    Bump openssl from 0.10.61 to 0.10.64
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [openssl](https://github.com/sfackler/rust-openssl) from 0.10.61 to 0.10.64.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/sfackler/rust-openssl/releases">openssl's releases</a>.</em></p>
<blockquote>
<h2>openssl-v0.10.64</h2>
<h2>What's Changed</h2>
<ul>
<li>Make _STACK opaque for LibreSSL &gt;= 3.9.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2153">sfackler/rust-openssl#2153</a></li>
<li>enable x509 verify and groups list for boringssl by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2155">sfackler/rust-openssl#2155</a></li>
<li>Cleanup some not-required Path::new invocations by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2158">sfackler/rust-openssl#2158</a></li>
<li>fixed a clippy (nightly) warning by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2161">sfackler/rust-openssl#2161</a></li>
<li>Bump actions versions by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2162">sfackler/rust-openssl#2162</a></li>
<li>Add support for setting the nonce type and digest on a PKEY_CTX by <a href="https://github.com/facutuesca"><code>@​facutuesca</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2144">sfackler/rust-openssl#2144</a></li>
<li>rebuild openssl-sys if the underlying openssl has changed by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2157">sfackler/rust-openssl#2157</a></li>
<li>Added binding for EVP_default_properties_enable_fips by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2168">sfackler/rust-openssl#2168</a></li>
<li>LibreSSL 3.9: fix CRYPTO_malloc/free signatures by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2170">sfackler/rust-openssl#2170</a></li>
<li>Expose alias on X509 structs by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2167">sfackler/rust-openssl#2167</a></li>
<li>bump openssl and openssl-sys + changelogs by <a href="https://github.com/reaperhulk"><code>@​reaperhulk</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2175">sfackler/rust-openssl#2175</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.63...openssl-v0.10.64">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.63...openssl-v0.10.64</a></p>
<h2>openssl-v0.10.63</h2>
<h2>What's Changed</h2>
<ul>
<li>Allow passing a passphrase callback when loading a public key by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2135">sfackler/rust-openssl#2135</a></li>
<li>Expose several additional ciphers for symmetry with symm by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2140">sfackler/rust-openssl#2140</a></li>
<li>brew: add openssl@3.0 (for 3.0.x LTS releases) by <a href="https://github.com/chenrui333"><code>@​chenrui333</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2141">sfackler/rust-openssl#2141</a></li>
<li>Add PKey::from_dhx by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2142">sfackler/rust-openssl#2142</a></li>
<li>Make X509_PURPOSE opaque for LibreSSL &gt;= 3.9.0 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2145">sfackler/rust-openssl#2145</a></li>
<li>PEM parsing: check last error instead of first by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2148">sfackler/rust-openssl#2148</a></li>
<li>Expose brainpool NIDs on libressl by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2150">sfackler/rust-openssl#2150</a></li>
<li>Add two methods to the PKCS7 API by <a href="https://github.com/facutuesca"><code>@​facutuesca</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2111">sfackler/rust-openssl#2111</a></li>
<li>add more boringssl methods by <a href="https://github.com/zh-jq"><code>@​zh-jq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2138">sfackler/rust-openssl#2138</a></li>
<li>Release openssl v0.10.63 and openssl-sys v0.9.99 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2152">sfackler/rust-openssl#2152</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.62...openssl-v0.10.63">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.62...openssl-v0.10.63</a></p>
<h2>openssl-v0.10.62</h2>
<h2>What's Changed</h2>
<ul>
<li>fixes <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2119">#2119</a> -- use ErrorStack abstraction in X.509 error handling by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2120">sfackler/rust-openssl#2120</a></li>
<li>Fix building with latest BoringSSL by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2121">sfackler/rust-openssl#2121</a></li>
<li>Fix tests on macOS by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2123">sfackler/rust-openssl#2123</a></li>
<li>Upcoming API changes in LibreSSL 3.9 by <a href="https://github.com/botovq"><code>@​botovq</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2124">sfackler/rust-openssl#2124</a></li>
<li>Add <code>rand_priv_bytes</code> by <a href="https://github.com/overvenus"><code>@​overvenus</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2126">sfackler/rust-openssl#2126</a></li>
<li>Add nid constant for curve brainpoolP320r1 by <a href="https://github.com/nicklaswj"><code>@​nicklaswj</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2129">sfackler/rust-openssl#2129</a></li>
<li>Release openssl v0.10.62 and openssl-sys v0.9.98 by <a href="https://github.com/alex"><code>@​alex</code></a> in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2133">sfackler/rust-openssl#2133</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/overvenus"><code>@​overvenus</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2126">sfackler/rust-openssl#2126</a></li>
<li><a href="https://github.com/nicklaswj"><code>@​nicklaswj</code></a> made their first contribution in <a href="https://redirect.github.com/sfackler/rust-openssl/pull/2129">sfackler/rust-openssl#2129</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.62">https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.62</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4a19cd48259e0755d9a9067f4c1a51ee63844c66"><code>4a19cd4</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2175">#2175</a> from reaperhulk/changelog</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/4e0e05a6293043cf7b9392c0e286c8397ce75996"><code>4e0e05a</code></a> bump openssl and openssl-sys + changelogs</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/c2b124aa2c36b5fc792239391e614df7f6f1fb24"><code>c2b124a</code></a> Be explicit that aliases are not part of X.509 certificates</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/1abf4a5b792228f6e9d8676015623d6315def4c1"><code>1abf4a5</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2167">#2167</a> from alex/expose-alias</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a644ec2542473c854a02b7fe642621e813517979"><code>a644ec2</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2170">#2170</a> from botovq/crypto-free</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/83940d14e30ed4e7c885dd44e3002c1955d5d5ed"><code>83940d1</code></a> LibreSSL 3.9: fix CRYPTO_malloc/free signatures</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/51fc5694821d66983d8639d3b0b4a58024f92a1f"><code>51fc569</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2168">#2168</a> from sfackler/alex-patch-1</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/3c53dee153d4ab801cde3e10d914a16789464a6b"><code>3c53dee</code></a> Added binding for EVP_default_properties_enable_fips</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/a12abe1b92c526f6995632ba43f6bfc433b5997d"><code>a12abe1</code></a> Expose alias on X509 structs</li>
<li><a href="https://github.com/sfackler/rust-openssl/commit/3acf2eff0baf7db1a5722c14def50cf5b068538e"><code>3acf2ef</code></a> Merge pull request <a href="https://redirect.github.com/sfackler/rust-openssl/issues/2157">#2157</a> from reaperhulk/rebuild-if-changed</li>
<li>Additional commits viewable in <a href="https://github.com/sfackler/rust-openssl/compare/openssl-v0.10.61...openssl-v0.10.64">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=openssl&package-manager=cargo&previous-version=0.10.61&new-version=0.10.64)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:29:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4447" class=".btn">#4447</a>
            </td>
            <td>
                <b>
                    Bump black from 24.2.0 to 24.4.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [black](https://github.com/psf/black) from 24.2.0 to 24.4.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/releases">black's releases</a>.</em></p>
<blockquote>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<p>This release is a milestone: it fixes Black's first CVE security vulnerability. If you
run Black on untrusted input, or if you habitually put thousands of leading tab
characters in your docstrings, you are strongly encouraged to upgrade immediately to fix
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.</p>
<p>This release also fixes a bug in Black's AST safety check that allowed Black to make
incorrect changes to certain f-strings that are valid in Python 3.12 and higher.</p>
<h3>Stable style</h3>
<ul>
<li>Don't move comments along with delimiters, which could cause crashes (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li>Strengthen AST safety check to catch more unsafe changes to strings. Previous versions
of Black would incorrectly format the contents of certain unusual f-strings containing
nested strings with the same quote type. Now, Black will crash on such strings until
support for the new f-string syntax is implemented. (<a href="https://redirect.github.com/psf/black/issues/4270">#4270</a>)</li>
<li>Fix a bug where line-ranges exceeding the last code line would not work as expected
(<a href="https://redirect.github.com/psf/black/issues/4273">#4273</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix catastrophic performance on docstrings that contain large numbers of leading tab
characters. This fixes
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.
(<a href="https://redirect.github.com/psf/black/issues/4278">#4278</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Note what happens when <code>--check</code> is used with <code>--quiet</code> (<a href="https://redirect.github.com/psf/black/issues/4236">#4236</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/psf/black/blob/main/CHANGES.md">black's changelog</a>.</em></p>
<blockquote>
<h2>24.4.0</h2>
<h3>Stable style</h3>
<ul>
<li>Fix unwanted crashes caused by AST equivalency check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
</ul>
<h3>Preview style</h3>
<ul>
<li><code>if</code> guards in <code>case</code> blocks are now wrapped in parentheses when the line is too long.
(<a href="https://redirect.github.com/psf/black/issues/4269">#4269</a>)</li>
<li>Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
</ul>
<h3>Integrations</h3>
<ul>
<li>Add a new option <code>use_pyproject</code> to the GitHub Action <code>psf/black</code>. This will read the
Black version from <code>pyproject.toml</code>. (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
</ul>
<h2>24.3.0</h2>
<h3>Highlights</h3>
<p>This release is a milestone: it fixes Black's first CVE security vulnerability. If you
run Black on untrusted input, or if you habitually put thousands of leading tab
characters in your docstrings, you are strongly encouraged to upgrade immediately to fix
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.</p>
<p>This release also fixes a bug in Black's AST safety check that allowed Black to make
incorrect changes to certain f-strings that are valid in Python 3.12 and higher.</p>
<h3>Stable style</h3>
<ul>
<li>Don't move comments along with delimiters, which could cause crashes (<a href="https://redirect.github.com/psf/black/issues/4248">#4248</a>)</li>
<li>Strengthen AST safety check to catch more unsafe changes to strings. Previous versions
of Black would incorrectly format the contents of certain unusual f-strings containing
nested strings with the same quote type. Now, Black will crash on such strings until
support for the new f-string syntax is implemented. (<a href="https://redirect.github.com/psf/black/issues/4270">#4270</a>)</li>
<li>Fix a bug where line-ranges exceeding the last code line would not work as expected
(<a href="https://redirect.github.com/psf/black/issues/4273">#4273</a>)</li>
</ul>
<h3>Performance</h3>
<ul>
<li>Fix catastrophic performance on docstrings that contain large numbers of leading tab
characters. This fixes
<a href="https://cve.mitre.org/cgi-bin/cvename.cgi?name=CVE-2024-21503">CVE-2024-21503</a>.
(<a href="https://redirect.github.com/psf/black/issues/4278">#4278</a>)</li>
</ul>
<h3>Documentation</h3>
<ul>
<li>Note what happens when <code>--check</code> is used with <code>--quiet</code> (<a href="https://redirect.github.com/psf/black/issues/4236">#4236</a>)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/psf/black/commit/8fe627072f15ff2e3d380887b92f7868efaf6d05"><code>8fe6270</code></a> Prepare release 24.4.0 (<a href="https://redirect.github.com/psf/black/issues/4307">#4307</a>)</li>
<li><a href="https://github.com/psf/black/commit/6b25e7cdabe2cd0dc2ec9d0009668af085b1e732"><code>6b25e7c</code></a> Bump peter-evans/find-comment from 3.0.0 to 3.1.0 (<a href="https://redirect.github.com/psf/black/issues/4304">#4304</a>)</li>
<li><a href="https://github.com/psf/black/commit/07fe1ca88abee9a0c88efb6b4213ea04d3fe2eae"><code>07fe1ca</code></a> docs: remove repetitive word (<a href="https://redirect.github.com/psf/black/issues/4303">#4303</a>)</li>
<li><a href="https://github.com/psf/black/commit/3383f531bc25955eebb2644ba5b389413bd10219"><code>3383f53</code></a> GitHub Action: Allow reading version from pyproject.toml (<a href="https://redirect.github.com/psf/black/issues/4294">#4294</a>)</li>
<li><a href="https://github.com/psf/black/commit/c8f1a5542c257491e1e093b1404481ece7f7e02c"><code>c8f1a55</code></a> [pre-commit.ci] pre-commit autoupdate (<a href="https://redirect.github.com/psf/black/issues/4297">#4297</a>)</li>
<li><a href="https://github.com/psf/black/commit/836acad86371578527408a4c8f968cde1302e130"><code>836acad</code></a> Improve AST safety check (<a href="https://redirect.github.com/psf/black/issues/4290">#4290</a>)</li>
<li><a href="https://github.com/psf/black/commit/13bd0925eb347926399a5bcb8b70853549f3da07"><code>13bd092</code></a> fix: Stop moving multiline strings to a new line unless inside brackets (<a href="https://redirect.github.com/psf/black/issues/4289">#4289</a>)</li>
<li><a href="https://github.com/psf/black/commit/c9d2635b55d03cd125465cd6d7477e6c3cb8fba3"><code>c9d2635</code></a> Remove mocking from tests (<a href="https://redirect.github.com/psf/black/issues/4287">#4287</a>)</li>
<li><a href="https://github.com/psf/black/commit/bf1195612c00b008ea67ea0472ae527956eb66fe"><code>bf11956</code></a> Fix two logging calls in the test helper (<a href="https://redirect.github.com/psf/black/issues/4286">#4286</a>)</li>
<li><a href="https://github.com/psf/black/commit/97993f997fe01cf565924072e4915126cdb86ed2"><code>97993f9</code></a> Bump pypa/cibuildwheel from 2.16.5 to 2.17.0 (<a href="https://redirect.github.com/psf/black/issues/4283">#4283</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/psf/black/compare/24.2.0...24.4.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=black&package-manager=pip&previous-version=24.2.0&new-version=24.4.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4446" class=".btn">#4446</a>
            </td>
            <td>
                <b>
                    Bump libsodium-sys-stable from 1.20.4 to 1.20.5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [libsodium-sys-stable](https://github.com/jedisct1/libsodium-sys-stable) from 1.20.4 to 1.20.5.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/023d96bd60b358174a7eadd72e04891f032309e6"><code>023d96b</code></a> Ignore *~</li>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/6fba98c492d333b8445af35aa3765311c340090d"><code>6fba98c</code></a> Update .gitignore</li>
<li><a href="https://github.com/jedisct1/libsodium-sys-stable/commit/81ae10406db2f4fe3a4b21c5d9095f14e9fc2c8c"><code>81ae104</code></a> Update libsodium</li>
<li>See full diff in <a href="https://github.com/jedisct1/libsodium-sys-stable/compare/1.20.4...1.20.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=libsodium-sys-stable&package-manager=cargo&previous-version=1.20.4&new-version=1.20.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4445" class=".btn">#4445</a>
            </td>
            <td>
                <b>
                    Bump pytest from 8.0.0 to 8.1.1 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [pytest](https://github.com/pytest-dev/pytest) from 8.0.0 to 8.1.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/pytest-dev/pytest/releases">pytest's releases</a>.</em></p>
<blockquote>
<h2>8.1.1</h2>
<h1>pytest 8.1.1 (2024-03-08)</h1>
<p>::: {.note}
::: {.title}
Note
:::</p>
<p>This release is not a usual bug fix release -- it contains features and improvements, being a follow up
to <code>8.1.0</code>, which has been yanked from PyPI.
:::</p>
<h2>Features</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11475">#11475</a>: Added the new <code>consider_namespace_packages</code>{.interpreted-text role=&quot;confval&quot;} configuration option, defaulting to <code>False</code>.</p>
<p>If set to <code>True</code>, pytest will attempt to identify modules that are part of <a href="https://packaging.python.org/en/latest/guides/packaging-namespace-packages">namespace packages</a> when importing modules.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11653">#11653</a>: Added the new <code>verbosity_test_cases</code>{.interpreted-text role=&quot;confval&quot;} configuration option for fine-grained control of test execution verbosity.
See <code>Fine-grained verbosity &lt;pytest.fine_grained_verbosity&gt;</code>{.interpreted-text role=&quot;ref&quot;} for more details.</p>
</li>
</ul>
<h2>Improvements</h2>
<ul>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/10865">#10865</a>: <code>pytest.warns</code>{.interpreted-text role=&quot;func&quot;} now validates that <code>warnings.warn</code>{.interpreted-text role=&quot;func&quot;} was called with a [str]{.title-ref} or a [Warning]{.title-ref}.
Currently in Python it is possible to use other types, however this causes an exception when <code>warnings.filterwarnings</code>{.interpreted-text role=&quot;func&quot;} is used to filter those warnings (see [CPython <a href="https://redirect.github.com/pytest-dev/pytest/issues/103577">#103577</a>](<a href="https://redirect.github.com/python/cpython/issues/103577">python/cpython#103577</a>) for a discussion).
While this can be considered a bug in CPython, we decided to put guards in pytest as the error message produced without this check in place is confusing.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11311">#11311</a>: When using <code>--override-ini</code> for paths in invocations without a configuration file defined, the current working directory is used
as the relative directory.</p>
<p>Previoulsy this would raise an <code>AssertionError</code>{.interpreted-text role=&quot;class&quot;}.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11475">#11475</a>: <code>--import-mode=importlib &lt;import-mode-importlib&gt;</code>{.interpreted-text role=&quot;ref&quot;} now tries to import modules using the standard import mechanism (but still without changing :py<code>sys.path</code>{.interpreted-text role=&quot;data&quot;}), falling back to importing modules directly only if that fails.</p>
<p>This means that installed packages will be imported under their canonical name if possible first, for example <code>app.core.models</code>, instead of having the module name always be derived from their path (for example <code>.env310.lib.site_packages.app.core.models</code>).</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11801">#11801</a>: Added the <code>iter_parents() &lt;_pytest.nodes.Node.iter_parents&gt;</code>{.interpreted-text role=&quot;func&quot;} helper method on nodes.
It is similar to <code>listchain &lt;_pytest.nodes.Node.listchain&gt;</code>{.interpreted-text role=&quot;func&quot;}, but goes from bottom to top, and returns an iterator, not a list.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11850">#11850</a>: Added support for <code>sys.last_exc</code>{.interpreted-text role=&quot;data&quot;} for post-mortem debugging on Python&gt;=3.12.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11962">#11962</a>: In case no other suitable candidates for configuration file are found, a <code>pyproject.toml</code> (even without a <code>[tool.pytest.ini_options]</code> table) will be considered as the configuration file and define the <code>rootdir</code>.</p>
</li>
<li>
<p><a href="https://redirect.github.com/pytest-dev/pytest/issues/11978">#11978</a>: Add <code>--log-file-mode</code> option to the logging plugin, enabling appending to log-files. This option accepts either <code>&quot;w&quot;</code> or <code>&quot;a&quot;</code> and defaults to <code>&quot;w&quot;</code>.</p>
<p>Previously, the mode was hard-coded to be <code>&quot;w&quot;</code> which truncates the file before logging.</p>
</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pytest-dev/pytest/commit/81653ee385f4c62ee7e64502a7b7530096553115"><code>81653ee</code></a> Adjust changelog manually for 8.1.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/e60b4b9ed80f761e3a51868a01338911a567b093"><code>e60b4b9</code></a> Prepare release version 8.1.1</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/15fbe57c44fed6737f5c6dad99cf4437b6755a6c"><code>15fbe57</code></a> [8.1.x] Revert legacy path removals (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12093">#12093</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/86c3aab005a98de7e12ee5e37782837f5db70ac3"><code>86c3aab</code></a> [8.1.x] Do not import duplicated modules with --importmode=importlib (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12077">#12077</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/5b82b0cd20c3adcc21f34ae30c595c7355a87e23"><code>5b82b0c</code></a> [8.1.x] Yank version 8.1.0 (<a href="https://redirect.github.com/pytest-dev/pytest/issues/12076">#12076</a>)</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/0a536810dc5f51dac99bdb90dde06704b5aa034e"><code>0a53681</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12054">#12054</a> from pytest-dev/release-8.1.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/b9a167f9bbbd6eda4f0360c5bf5b7f5af50f2bc4"><code>b9a167f</code></a> Prepare release version 8.1.0</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/00043f7f1047b29fdaeb18e169fe9d6146988cb8"><code>00043f7</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12038">#12038</a> from bluetech/fixtures-rm-arg2index</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/f4e10251a4a003495b5228cea421d4de5fa0ce89"><code>f4e1025</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12048">#12048</a> from bluetech/fixture-teardown-excgroup</li>
<li><a href="https://github.com/pytest-dev/pytest/commit/43492f5707b38dab9b62dfb829bb41a13579629f"><code>43492f5</code></a> Merge pull request <a href="https://redirect.github.com/pytest-dev/pytest/issues/12051">#12051</a> from jakkdl/test_debugging_pythonbreakpoint</li>
<li>Additional commits viewable in <a href="https://github.com/pytest-dev/pytest/compare/8.0.0...8.1.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=pytest&package-manager=pip&previous-version=8.0.0&new-version=8.1.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4444" class=".btn">#4444</a>
            </td>
            <td>
                <b>
                    Bump erased-serde from 0.3.31 to 0.4.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [erased-serde](https://github.com/dtolnay/erased-serde) from 0.3.31 to 0.4.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/erased-serde/releases">erased-serde's releases</a>.</em></p>
<blockquote>
<h2>0.4.1</h2>
<ul>
<li>Fix panic when Serialize impl returns error that does not come from a Serializer (<a href="https://redirect.github.com/dtolnay/erased-serde/issues/100">#100</a>, thanks <a href="https://github.com/KodrAus"><code>@​KodrAus</code></a>)</li>
</ul>
<h2>0.4.0</h2>
<p>This release includes a redesign of the erased serialization API (<a href="https://redirect.github.com/dtolnay/erased-serde/issues/93">#93</a>) with the following advantages:</p>
<ul>
<li>Eliminates all reliance on unsafe code within the serialization implementation</li>
<li>Reduces overhead of erased serialization vs monomorphized serialization by a factor of 2 (<a href="https://redirect.github.com/dtolnay/erased-serde/issues/99">#99</a>)</li>
<li>Supports serializers which have non-'static <code>Ok</code> types</li>
</ul>
<h2>0.4.0-rc.1</h2>
<p>No release notes provided.</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/erased-serde/commit/4726cdb49deb6ab857fb389eb68e77389ce2ddcd"><code>4726cdb</code></a> Release 0.4.1</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/4e04e70902ed51c994e7ef45ce92c9af5c274883"><code>4e04e70</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/erased-serde/issues/101">#101</a> from dtolnay/sererror</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/c670c72da5ee0341cf7b52e835def2332182ac5c"><code>c670c72</code></a> Preserve error message of errors originated from Serialize impl</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/6893670ccaaa2af7829d614f3f99cc9dfc4b372a"><code>6893670</code></a> Ignore box_collection clippy lint</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/7ddf6aadd8ec8d784640f28a224b294f04daf7b8"><code>7ddf6aa</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/erased-serde/issues/100">#100</a> from KodrAus/fix/failing-serialize-impl</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/8227d205737bb13a4045c666870e4e5e9d300afa"><code>8227d20</code></a> handle the case where a Serialize fails without calling the Serializer</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/160c15393ecf2aae62639070fe24a2d907862cac"><code>160c153</code></a> Release 0.4.0</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/2e4897701901593481a9db9fc40a784b4c4e676e"><code>2e48977</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/erased-serde/issues/99">#99</a> from dtolnay/bench</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/7349ad4b4cd950d16b217f67f3590904178e23d2"><code>7349ad4</code></a> Add serialization benchmark</li>
<li><a href="https://github.com/dtolnay/erased-serde/commit/a8fdff9a4cd23575ab16b349bbe764feac6788d8"><code>a8fdff9</code></a> Release 0.4.0-rc.1</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/erased-serde/compare/0.3.31...0.4.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=erased-serde&package-manager=cargo&previous-version=0.3.31&new-version=0.4.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4443" class=".btn">#4443</a>
            </td>
            <td>
                <b>
                    Bump cryptography from 42.0.3 to 42.0.5 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [cryptography](https://github.com/pyca/cryptography) from 42.0.3 to 42.0.5.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/pyca/cryptography/blob/main/CHANGELOG.rst">cryptography's changelog</a>.</em></p>
<blockquote>
<p>42.0.5 - 2024-02-23</p>
<pre><code>
* Limit the number of name constraint checks that will be performed in
  :mod:`X.509 path validation &lt;cryptography.x509.verification&gt;` to protect
  against denial of service attacks.
* Upgrade ``pyo3`` version, which fixes building on PowerPC.
<p>.. _v42-0-4:</p>
<p>42.0.4 - 2024-02-20
</code></pre></p>
<ul>
<li>Fixed a null-pointer-dereference and segfault that could occur when creating
a PKCS#12 bundle. Credit to <strong>Alexander-Programming</strong> for reporting the
issue. <strong>CVE-2024-26130</strong></li>
<li>Fixed ASN.1 encoding for PKCS7/SMIME signed messages. The fields <code>SMIMECapabilities</code>
and <code>SignatureAlgorithmIdentifier</code> should now be correctly encoded according to the
definitions in :rfc:<code>2633</code> :rfc:<code>3370</code>.</li>
</ul>
<p>.. _v42-0-3:</p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/pyca/cryptography/commit/33833f031d9d36234e11d9671be150d53b9e598d"><code>33833f0</code></a> Release 42.0.5 (<a href="https://redirect.github.com/pyca/cryptography/issues/10470">#10470</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/4be53bf20cc90cbac01f5f94c5d1aecc5289ba1f"><code>4be53bf</code></a> Added a budget for NC checks to protect against DoS (<a href="https://redirect.github.com/pyca/cryptography/issues/10467">#10467</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10468">#10468</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/8e9de309f850a17409da5de39cfcd9296c25ea36"><code>8e9de30</code></a> Bump pyo3 from 0.20.2 to 0.20.3 in /src/rust (<a href="https://redirect.github.com/pyca/cryptography/issues/10462">#10462</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10465">#10465</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/fe18470f7d05f963e7267e34fdf985d81ea6ceea"><code>fe18470</code></a> Bump for 42.0.4 release (<a href="https://redirect.github.com/pyca/cryptography/issues/10445">#10445</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/aaa2dd06ed470695de818405a982d4c459869803"><code>aaa2dd0</code></a> Fix ASN.1 issues in PKCS#7 and S/MIME signing (<a href="https://redirect.github.com/pyca/cryptography/issues/10373">#10373</a>) (<a href="https://redirect.github.com/pyca/cryptography/issues/10442">#10442</a>)</li>
<li><a href="https://github.com/pyca/cryptography/commit/7a4d012991061974da5d9cb7614de65eac94f49b"><code>7a4d012</code></a> Fixes <a href="https://redirect.github.com/pyca/cryptography/issues/10422">#10422</a> -- don't crash when a PKCS#12 key and cert don't match (<a href="https://redirect.github.com/pyca/cryptography/issues/10423">#10423</a>) ...</li>
<li><a href="https://github.com/pyca/cryptography/commit/df314bb182bdfd661333969a94325e4680d785f6"><code>df314bb</code></a> backport actions m1 switch to 42.0.x (<a href="https://redirect.github.com/pyca/cryptography/issues/10415">#10415</a>)</li>
<li>See full diff in <a href="https://github.com/pyca/cryptography/compare/42.0.3...42.0.5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=cryptography&package-manager=pip&previous-version=42.0.3&new-version=42.0.5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4442" class=".btn">#4442</a>
            </td>
            <td>
                <b>
                    Bump mypy from 1.8.0 to 1.9.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [mypy](https://github.com/python/mypy) from 1.8.0 to 1.9.0.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/python/mypy/blob/master/CHANGELOG.md">mypy's changelog</a>.</em></p>
<blockquote>
<h1>Mypy Release Notes</h1>
<h2>Mypy 1.9</h2>
<p>We’ve just uploaded mypy 1.9 to the Python Package Index (<a href="https://pypi.org/project/mypy/">PyPI</a>). Mypy is a static type checker for Python. This release includes new features, performance improvements and bug fixes. You can install it as follows:</p>
<pre><code>python3 -m pip install -U mypy
</code></pre>
<p>You can read the full documentation for this release on <a href="http://mypy.readthedocs.io">Read the Docs</a>.</p>
<h4>Breaking Changes</h4>
<p>Because the version of typeshed we use in mypy 1.9 doesn't support 3.7, neither does mypy 1.9. (Jared Hance, PR <a href="https://redirect.github.com/python/mypy/pull/16883">16883</a>)</p>
<p>We are planning to enable
<a href="https://mypy.readthedocs.io/en/stable/command_line.html#cmdoption-mypy-local-partial-types">local partial types</a> (enabled via the
<code>--local-partial-types</code> flag) later this year by default. This change
was announced years ago, but now it's finally happening. This is a
major backward-incompatible change, so we'll probably include it as
part of the upcoming mypy 2.0 release. This makes daemon and
non-daemon mypy runs have the same behavior by default.</p>
<p>Local partial types can also be enabled in the mypy config file:</p>
<pre><code>local_partial_types = True
</code></pre>
<p>We are looking at providing a tool to make it easier to migrate
projects to use <code>--local-partial-types</code>, but it's not yet clear whether
this is practical. The migration usually involves adding some
explicit type annotations to module-level and class-level variables.</p>
<h4>Basic Support for Type Parameter Defaults (PEP 696)</h4>
<p>This release contains new experimental support for type parameter
defaults (<a href="https://peps.python.org/pep-0696">PEP 696</a>). Please try it
out! This feature was contributed by Marc Mueller.</p>
<p>Since this feature will be officially introduced in the next Python
feature release (3.13), you will need to import <code>TypeVar</code>, <code>ParamSpec</code>
or <code>TypeVarTuple</code> from <code>typing_extensions</code> to use defaults for now.</p>
<p>This example adapted from the PEP defines a default for <code>BotT</code>:</p>
<pre lang="python"><code>from typing import Generic
from typing_extensions import TypeVar
<p>class Bot: ...</p>
<p>BotT = TypeVar(&quot;BotT&quot;, bound=Bot, default=Bot)
&lt;/tr&gt;&lt;/table&gt;
</code></pre></p>
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/python/mypy/commit/5ff46f8b3706d005fabab2227ec84476d605bfd4"><code>5ff46f8</code></a> Remove +dev.</li>
<li><a href="https://github.com/python/mypy/commit/155909ad1bde747d89fcd091621d7cd9b1e15818"><code>155909a</code></a> [Release 1.9] Unsupport targetting 3.7. (<a href="https://redirect.github.com/python/mypy/issues/16883">#16883</a>) (<a href="https://redirect.github.com/python/mypy/issues/16900">#16900</a>)</li>
<li><a href="https://github.com/python/mypy/commit/6615cabe57c661114d0ed44784f67301619faadf"><code>6615cab</code></a> [Release 1.9] Stubtest: ignore a new protocol dunder (<a href="https://redirect.github.com/python/mypy/issues/16895">#16895</a>) (<a href="https://redirect.github.com/python/mypy/issues/16899">#16899</a>)</li>
<li><a href="https://github.com/python/mypy/commit/b956e6a57c4dd36d670097a3eccf7dc092348fec"><code>b956e6a</code></a> stubtest: Private parameters can be omitted (<a href="https://redirect.github.com/python/mypy/issues/16507">#16507</a>)</li>
<li><a href="https://github.com/python/mypy/commit/ede0b200a10186a095378516d840389f8da4edd4"><code>ede0b20</code></a> Bump ruff to 0.2.0 (<a href="https://redirect.github.com/python/mypy/issues/16870">#16870</a>)</li>
<li><a href="https://github.com/python/mypy/commit/7bdd61f2d89ecd2cee4ebe6eb2375a72b29f0b10"><code>7bdd61f</code></a> stubgen: Fix crash on star unpack of TypeVarTuple (<a href="https://redirect.github.com/python/mypy/issues/16869">#16869</a>)</li>
<li><a href="https://github.com/python/mypy/commit/8c2ef9dde8aa803e04038427ad84f09664d9d93f"><code>8c2ef9d</code></a> Update hashes in sync-typeshed.py following recent typeshed sync</li>
<li><a href="https://github.com/python/mypy/commit/0dd4b6f7576be3d3857fecefb298decdf0711ac7"><code>0dd4b6f</code></a> Revert use of <code>ParamSpec</code> for <code>functools.wraps</code></li>
<li><a href="https://github.com/python/mypy/commit/dd12a2d810f2bbe7a8686674397043b18575480f"><code>dd12a2d</code></a> Revert typeshed ctypes change</li>
<li><a href="https://github.com/python/mypy/commit/d132999ba631b332d0684173897e5947591f4acc"><code>d132999</code></a> Revert sum literal integer change (<a href="https://redirect.github.com/python/mypy/issues/13961">#13961</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/python/mypy/compare/v1.8.0...1.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=mypy&package-manager=pip&previous-version=1.8.0&new-version=1.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4441" class=".btn">#4441</a>
            </td>
            <td>
                <b>
                    Bump async-trait from 0.1.74 to 0.1.76
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">rust</span>
            </td>
            <td>
                Bumps [async-trait](https://github.com/dtolnay/async-trait) from 0.1.74 to 0.1.76.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/dtolnay/async-trait/releases">async-trait's releases</a>.</em></p>
<blockquote>
<h2>0.1.76</h2>
<ul>
<li>Documentation improvements</li>
</ul>
<h2>0.1.75</h2>
<ul>
<li>Documentation improvements</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/dtolnay/async-trait/commit/627124bf67cc173c7564454e71dfccc30f6bc5f5"><code>627124b</code></a> Release 0.1.76</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/f8aa269375241ba9b642b6f8ca8baa61be33b24e"><code>f8aa269</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/256">#256</a> from dtolnay/miritracing</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/48e29e43c0a3d64166f805fb15978e8ffd487e43"><code>48e29e4</code></a> Re-enable tracing integration test under Miri</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/3c656d37343f9a4585934c1f74a6c33f79133bab"><code>3c656d3</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/255">#255</a> from dtolnay/asyncblock</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/381fd7564e6d29d6647da1099e12de36136a4a03"><code>381fd75</code></a> Update explanation to show async block expansion</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/3caf301d1ba67025598441ef3669115def954473"><code>3caf301</code></a> Merge pull request <a href="https://redirect.github.com/dtolnay/async-trait/issues/254">#254</a> from dtolnay/doc</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/c1576be43953b849e65963ea67930be789dfb372"><code>c1576be</code></a> Update documentation to discuss object safety in Rust 1.75+</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/034d8db0b851a3e401b3a374ee57fe4492283a74"><code>034d8db</code></a> Release 0.1.75</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/0d469fcea4cd16c49e8d0bc797ea4b51a11054f0"><code>0d469fc</code></a> Add a funding file</li>
<li><a href="https://github.com/dtolnay/async-trait/commit/b4a3886153fa49c833e22e9a8259a8bf5b897cd2"><code>b4a3886</code></a> Update ui test suite to nightly-2023-11-20</li>
<li>Additional commits viewable in <a href="https://github.com/dtolnay/async-trait/compare/0.1.74...0.1.76">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=async-trait&package-manager=cargo&previous-version=0.1.74&new-version=0.1.76)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:28:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4440" class=".btn">#4440</a>
            </td>
            <td>
                <b>
                    Bump docker/setup-buildx-action from 2 to 3
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [docker/setup-buildx-action](https://github.com/docker/setup-buildx-action) from 2 to 3.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/setup-buildx-action/releases">docker/setup-buildx-action's releases</a>.</em></p>
<blockquote>
<h2>v3.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/264">docker/setup-buildx-action#264</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/267">docker/setup-buildx-action#267</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.10.0...v3.0.0">https://github.com/docker/setup-buildx-action/compare/v2.10.0...v3.0.0</a></p>
<h2>v2.10.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.7.1 to 0.10.0 by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/258">docker/setup-buildx-action#258</a></li>
<li>Bump word-wrap from 1.2.3 to 1.2.5 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/253">docker/setup-buildx-action#253</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.9.1...v2.10.0">https://github.com/docker/setup-buildx-action/compare/v2.9.1...v2.10.0</a></p>
<h2>v2.9.1</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.7.0 to 0.7.1 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/248">docker/setup-buildx-action#248</a>
<ul>
<li>Fixes an issue where building Buildx does not match the local platform (<a href="https://redirect.github.com/docker/actions-toolkit/pull/135">docker/actions-toolkit#135</a>)</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.9.0...v2.9.1">https://github.com/docker/setup-buildx-action/compare/v2.9.0...v2.9.1</a></p>
<h2>v2.9.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.6.0 to 0.7.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/246">docker/setup-buildx-action#246</a>
<ul>
<li>Adds support to cache Buildx binary to hosted tool cache and GHA cache backend</li>
</ul>
</li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.8.0...v2.9.0">https://github.com/docker/setup-buildx-action/compare/v2.8.0...v2.9.0</a></p>
<h2>v2.8.0</h2>
<ul>
<li>Only set specific flags for drivers supporting them by <a href="https://github.com/nicks"><code>@​nicks</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/241">docker/setup-buildx-action#241</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.5.0 to 0.6.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/242">docker/setup-buildx-action#242</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.7.0...v2.8.0">https://github.com/docker/setup-buildx-action/compare/v2.7.0...v2.8.0</a></p>
<h2>v2.7.0</h2>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/237">docker/setup-buildx-action#237</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/238">docker/setup-buildx-action#238</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.6.0...v2.7.0">https://github.com/docker/setup-buildx-action/compare/v2.6.0...v2.7.0</a></p>
<h2>v2.6.0</h2>
<ul>
<li>Set node name for k8s driver when appending nodes by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/219">docker/setup-buildx-action#219</a></li>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.1.0-beta.18 to 0.3.0 in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/220">docker/setup-buildx-action#220</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/229">docker/setup-buildx-action#229</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/231">docker/setup-buildx-action#231</a> <a href="https://redirect.github.com/docker/setup-buildx-action/pull/236">docker/setup-buildx-action#236</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.5.0...v2.6.0">https://github.com/docker/setup-buildx-action/compare/v2.5.0...v2.6.0</a></p>
<h2>v2.5.0</h2>
<ul>
<li><code>cleanup</code> input to remove builder and temp files by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/213">docker/setup-buildx-action#213</a></li>
<li>do not remove builder using the <code>docker</code> driver by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/218">docker/setup-buildx-action#218</a></li>
<li>fix current context as builder name for <code>docker</code> driver by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/setup-buildx-action/pull/209">docker/setup-buildx-action#209</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/setup-buildx-action/compare/v2.4.1...v2.5.0">https://github.com/docker/setup-buildx-action/compare/v2.4.1...v2.5.0</a></p>
<h2>v2.4.1</h2>
<ul>
<li>Get releases from actions toolkit by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> (<a href="https://redirect.github.com/docker/setup-buildx-action/issues/200">#200</a>)</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/setup-buildx-action/commit/d70bba72b1f3fd22344832f00baa16ece964efeb"><code>d70bba7</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/307">#307</a> from crazy-max/bump-toolkit</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/7638634cb70c02d327dde3b558f22b0db32054a3"><code>7638634</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c68420fe0b4de2444121eec8f08bc2500c8d9216"><code>c68420f</code></a> bump <code>@​docker/actions-toolkit</code> from 0.19.0 to 0.20.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/2b51285047da1547ffb1b2203d8be4c0af6b1f20"><code>2b51285</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/306">#306</a> from docker/dependabot/npm_and_yarn/docker/actions-to...</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/0f00370563710ebfbdf4287b76a0a5d88864e7f9"><code>0f00370</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/11c9683db9ea73b2090280c1cfa7d725bd8a60fa"><code>11c9683</code></a> build(deps): bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/56a16b8f2aa74bcbd3ab9ec13027cd3ac8e3f94f"><code>56a16b8</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/303">#303</a> from crazy-max/fix-inputs</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/c23f46eb919af18b86ac6f0f4646a63a7a452b4d"><code>c23f46e</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/f876da6242168c5bb185ad517fb42f0b59fba456"><code>f876da6</code></a> rename and align config inputs</li>
<li><a href="https://github.com/docker/setup-buildx-action/commit/b7cf918227e7a90a94eea8534a6b0cc1965a0ccd"><code>b7cf918</code></a> Merge pull request <a href="https://redirect.github.com/docker/setup-buildx-action/issues/304">#304</a> from crazy-max/rm-docs-dir</li>
<li>Additional commits viewable in <a href="https://github.com/docker/setup-buildx-action/compare/v2...v3">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/setup-buildx-action&package-manager=github_actions&previous-version=2&new-version=3)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:27:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4439" class=".btn">#4439</a>
            </td>
            <td>
                <b>
                    Bump faker from 23.2.0 to 24.9.0 in /client_cli/pytests
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">python</span>
            </td>
            <td>
                Bumps [faker](https://github.com/joke2k/faker) from 23.2.0 to 24.9.0.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/releases">faker's releases</a>.</em></p>
<blockquote>
<h2>Release v24.9.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.9.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.8.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.8.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.7.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.7.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.7.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.7.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.6.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.6.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.5.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.5.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.4.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.4.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.3.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.3.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.2.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.2.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.2.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.2.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.1.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.1.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.1.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.1.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v24.0.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v24.0.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v23.3.0</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v23.3.0/CHANGELOG.md">CHANGELOG.md</a>.</p>
<h2>Release v23.2.1</h2>
<p>See <a href="https://github.com/joke2k/faker/blob/refs/tags/v23.2.1/CHANGELOG.md">CHANGELOG.md</a>.</p>
</blockquote>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/joke2k/faker/blob/master/CHANGELOG.md">faker's changelog</a>.</em></p>
<blockquote>
<h3><a href="https://github.com/joke2k/faker/compare/v24.8.0...v24.9.0">v24.9.0 - 2024-04-12</a></h3>
<ul>
<li>Update <code>uk_UA</code> phone provider. Thanks <a href="https://github.com/lozik4"><code>@​lozik4</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.7.1...v24.8.0">v24.8.0 - 2024-04-09</a></h3>
<ul>
<li>Fix wrong pricetag format in <code>ru_RU</code> locale. Thanks <a href="https://github.com/Pandede"><code>@​Pandede</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.7.0...v24.7.1">v24.7.1 - 2024-04-05</a></h3>
<ul>
<li>Fix previous release issue.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.6.0...v24.7.0">v24.7.0 - 2024-04-05</a></h3>
<ul>
<li>Update last names for <code>de_DE</code> locale. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
<li>Update phone number formats for <code>cs_CZ</code>, <code>sk_SK</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.5.0...v24.6.0">v24.6.0 - 2024-04-05</a></h3>
<ul>
<li>Update versions in <code>user_agent</code> provider. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.4.0...v24.5.0">v24.5.0 - 2024-04-05</a></h3>
<ul>
<li>Add type hints stubs. Thanks <a href="https://github.com/KaylaHood"><code>@​KaylaHood</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.3.0...v24.4.0">v24.4.0 - 2024-03-25</a></h3>
<ul>
<li>Add address words for <code>cs_CZ</code>. Thanks <a href="https://github.com/george0st"><code>@​george0st</code></a></li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.2.1...v24.3.0">v24.3.0 - 2024-03-18</a></h3>
<ul>
<li>Add phone number formats to nl_BE. Thanks <a href="https://github.com/maximegmd"><code>@​maximegmd</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.2.0...v24.2.1">v24.2.1 - 2024-03-18</a></h3>
<ul>
<li>Return capitalized city names in <code>hu_HU</code>. Thanks <a href="https://github.com/AlexLitvino"><code>@​AlexLitvino</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.1.1...v24.2.0">v24.2.0 - 2024-03-13</a></h3>
<ul>
<li>Add <code>uk-UA</code> credit card provider. Thanks <a href="https://github.com/lozik4"><code>@​lozik4</code></a>.</li>
<li>Upgrade <code>uk_UA</code> person provider. Thanks <a href="https://github.com/lozik4"><code>@​lozik4</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.1.0...v24.1.1">v24.1.1 - 2024-03-13</a></h3>
<ul>
<li>Fix prefix for male <code>bg_BG</code> names  Thanks <a href="https://github.com/DimitarVanguelov"><code>@​DimitarVanguelov</code></a>.</li>
</ul>
<h3><a href="https://github.com/joke2k/faker/compare/v24.0.0...v24.1.0">v24.1.0 - 2024-03-08</a></h3>
<ul>
<li>Add Grenville to <code>land_coords</code> in geo provider. Thanks <a href="https://github.com/lozik4"><code>@​lozik4</code></a>.</li>
<li>Fix Kyiv name. Thanks <a href="https://github.com/lozik4"><code>@​lozik4</code></a>.</li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/joke2k/faker/commit/e6c74d02517693bf1c4bd0c979492785a27d4882"><code>e6c74d0</code></a> Bump version: 24.8.0 → 24.9.0</li>
<li><a href="https://github.com/joke2k/faker/commit/12f5a9729fd1c1c74faf64a0528aa28c59aaf5ea"><code>12f5a97</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/b8aceb2a7a510148e5bbb826dd3bdede60f28450"><code>b8aceb2</code></a> Format code</li>
<li><a href="https://github.com/joke2k/faker/commit/11055a7be38043bd9fcf9a897e8a2029b8374460"><code>11055a7</code></a> Update <code>uk_UA</code> phone provider (<a href="https://redirect.github.com/joke2k/faker/issues/2016">#2016</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/c6324723fad295780cfd0594ef595eaf738565d9"><code>c632472</code></a> Update coding_style.rst</li>
<li><a href="https://github.com/joke2k/faker/commit/769e3dd06d6dfcdd64942b01c7b4fdf6a401286a"><code>769e3dd</code></a> Bump version: 24.7.1 → 24.8.0</li>
<li><a href="https://github.com/joke2k/faker/commit/34c6e0251206b9c67c492a08286e438e55da3636"><code>34c6e02</code></a> :pencil: Update CHANGELOG.md</li>
<li><a href="https://github.com/joke2k/faker/commit/58a76584007945f1bd4294fbd20cc56cf69311ab"><code>58a7658</code></a> Fix wrong pricetag format in <code>ru_RU</code> locale (<a href="https://redirect.github.com/joke2k/faker/issues/2018">#2018</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/89e20696809a7402f018ba9971de197ac41dd553"><code>89e2069</code></a> Remove duplicate assigned HTTP Status codes (<a href="https://redirect.github.com/joke2k/faker/issues/2017">#2017</a>)</li>
<li><a href="https://github.com/joke2k/faker/commit/591cffeb14e2d92747f1f49639fcbbe1ed4a80a9"><code>591cffe</code></a> Merge branch 'george0st-repair_sk_phone'</li>
<li>Additional commits viewable in <a href="https://github.com/joke2k/faker/compare/v23.2.0...v24.9.0">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=faker&package-manager=pip&previous-version=23.2.0&new-version=24.9.0)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:27:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4438" class=".btn">#4438</a>
            </td>
            <td>
                <b>
                    Bump actions/upload-artifact from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/upload-artifact](https://github.com/actions/upload-artifact) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/upload-artifact/releases">actions/upload-artifact's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>The release of upload-artifact@v4 and download-artifact@v4 are major changes to the backend architecture of Artifacts. They have numerous performance and behavioral improvements.</p>
<p>ℹ️ However, this is a major update that includes breaking changes. Artifacts created with versions v3 and below are not compatible with the v4 actions. Uploads and downloads <em>must</em> use the same major actions versions. There are also key differences from previous versions that may require updates to your workflows.</p>
<p>For more information, please see:</p>
<ol>
<li>The <a href="https://github.blog/changelog/2023-12-14-github-actions-artifacts-v4-is-now-generally-available/">changelog</a> post.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/README.md">README</a>.</li>
<li>The <a href="https://github.com/actions/upload-artifact/blob/main/docs/MIGRATION.md">migration documentation</a>.</li>
<li>As well as the underlying npm package, <a href="https://github.com/actions/toolkit/tree/main/packages/artifact"><code>@​actions/artifact</code></a> documentation.</li>
</ol>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/vmjoseph"><code>@​vmjoseph</code></a> made their first contribution in <a href="https://redirect.github.com/actions/upload-artifact/pull/464">actions/upload-artifact#464</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v4.0.0">https://github.com/actions/upload-artifact/compare/v3...v4.0.0</a></p>
<h2>v3.1.3</h2>
<h2>What's Changed</h2>
<ul>
<li>chore(github): remove trailing whitespaces by <a href="https://github.com/ljmf00"><code>@​ljmf00</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/313">actions/upload-artifact#313</a></li>
<li>Bump <code>@​actions/artifact</code> version to v1.1.2 by <a href="https://github.com/bethanyj28"><code>@​bethanyj28</code></a> in <a href="https://redirect.github.com/actions/upload-artifact/pull/436">actions/upload-artifact#436</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/upload-artifact/compare/v3...v3.1.3">https://github.com/actions/upload-artifact/compare/v3...v3.1.3</a></p>
<h2>v3.1.2</h2>
<ul>
<li>Update all <code>@actions/*</code> NPM packages to their latest versions- <a href="https://redirect.github.com/actions/upload-artifact/issues/374">#374</a></li>
<li>Update all dev dependencies to their most recent versions - <a href="https://redirect.github.com/actions/upload-artifact/issues/375">#375</a></li>
</ul>
<h2>v3.1.1</h2>
<ul>
<li>Update actions/core package to latest version to remove <code>set-output</code> deprecation warning <a href="https://redirect.github.com/actions/upload-artifact/issues/351">#351</a></li>
</ul>
<h2>v3.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Bump <code>@​actions/artifact</code> to v1.1.0 (<a href="https://redirect.github.com/actions/upload-artifact/pull/327">actions/upload-artifact#327</a>)
<ul>
<li>Adds checksum headers on artifact upload (<a href="https://redirect.github.com/actions/toolkit/pull/1095">actions/toolkit#1095</a>) (<a href="https://redirect.github.com/actions/toolkit/pull/1063">actions/toolkit#1063</a>)</li>
</ul>
</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/upload-artifact/commit/5d5d22a31266ced268874388b861e4b58bb5c2f3"><code>5d5d22a</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/515">#515</a> from actions/eggyhead/update-artifact-v2.1.1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/f1e993d9663a03508e7fc0370c744c4b963f0044"><code>f1e993d</code></a> update artifact license</li>
<li><a href="https://github.com/actions/upload-artifact/commit/4881bfd3f27855c63733d8cfff17721cc0ad611f"><code>4881bfd</code></a> updating dist:</li>
<li><a href="https://github.com/actions/upload-artifact/commit/a30777e2653648a0a7bbd3efb5c96ef9131b96cc"><code>a30777e</code></a> <a href="https://github.com/eggyhead"><code>@​eggyhead</code></a></li>
<li><a href="https://github.com/actions/upload-artifact/commit/3a8048248f2f288c271830f8ecf2a1c5d8eb0e9a"><code>3a80482</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/511">#511</a> from actions/robherley/migration-docs-typo</li>
<li><a href="https://github.com/actions/upload-artifact/commit/9d63e3f2f81d9dc4e13d83fc330408f8a94b79d1"><code>9d63e3f</code></a> Merge branch 'main' into robherley/migration-docs-typo</li>
<li><a href="https://github.com/actions/upload-artifact/commit/dfa1ab292d2fdd78d056187f11c568c16ab53de9"><code>dfa1ab2</code></a> fix typo with v3 artifact downloads in migration guide</li>
<li><a href="https://github.com/actions/upload-artifact/commit/d00351bf698398c17253d21cf8f90e57a344e14b"><code>d00351b</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/509">#509</a> from markmssd/patch-1</li>
<li><a href="https://github.com/actions/upload-artifact/commit/707f5a7b71e0fb01c5df1e16e9679a3292606ef2"><code>707f5a7</code></a> Update limitation of <code>10</code> artifacts upload to <code>500</code></li>
<li><a href="https://github.com/actions/upload-artifact/commit/26f96dfa697d77e81fd5907df203aa23a56210a8"><code>26f96df</code></a> Merge pull request <a href="https://redirect.github.com/actions/upload-artifact/issues/505">#505</a> from actions/robherley/merge-artifacts</li>
<li>Additional commits viewable in <a href="https://github.com/actions/upload-artifact/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/upload-artifact&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:27:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4437" class=".btn">#4437</a>
            </td>
            <td>
                <b>
                    Bump docker/build-push-action from 4 to 5
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [docker/build-push-action](https://github.com/docker/build-push-action) from 4 to 5.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/docker/build-push-action/releases">docker/build-push-action's releases</a>.</em></p>
<blockquote>
<h2>v5.0.0</h2>
<ul>
<li>Node 20 as default runtime (requires <a href="https://github.com/actions/runner/releases/tag/v2.308.0">Actions Runner v2.308.0</a> or later) by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/954">docker/build-push-action#954</a></li>
<li>Bump <code>@​actions/core</code> from 1.10.0 to 1.10.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/959">docker/build-push-action#959</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0">https://github.com/docker/build-push-action/compare/v4.2.1...v5.0.0</a></p>
<h2>v4.2.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>warn if docker config can't be parsed by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/957">docker/build-push-action#957</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.2.0...v4.2.1">https://github.com/docker/build-push-action/compare/v4.2.0...v4.2.1</a></p>
<h2>v4.2.0</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>display proxy configuration  by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/872">docker/build-push-action#872</a></li>
<li>chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.6.0 to 0.8.0 in <a href="https://redirect.github.com/docker/build-push-action/pull/930">docker/build-push-action#930</a></li>
<li>chore(deps): Bump word-wrap from 1.2.3 to 1.2.5 in <a href="https://redirect.github.com/docker/build-push-action/pull/925">docker/build-push-action#925</a></li>
<li>chore(deps): Bump semver from 6.3.0 to 6.3.1 in <a href="https://redirect.github.com/docker/build-push-action/pull/902">docker/build-push-action#902</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.1.1...v4.2.0">https://github.com/docker/build-push-action/compare/v4.1.1...v4.2.0</a></p>
<h2>v4.1.1</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Bump <code>@​docker/actions-toolkit</code> from 0.3.0 to 0.5.0 by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/880">docker/build-push-action#880</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.1.0...v4.1.1">https://github.com/docker/build-push-action/compare/v4.1.0...v4.1.1</a></p>
<h2>v4.1.0</h2>
<blockquote>
<p><strong>Note</strong></p>
<p>Buildx v0.10 enables support for a minimal <a href="https://slsa.dev/provenance/">SLSA Provenance</a> attestation, which requires support for <a href="https://github.com/opencontainers/image-spec">OCI-compliant</a> multi-platform images. This may introduce issues with registry and runtime support (e.g. <a href="https://redirect.github.com/docker/buildx/issues/1533">Google Cloud Run and AWS Lambda</a>). You can optionally disable the default provenance attestation functionality using <code>provenance: false</code>.</p>
</blockquote>
<ul>
<li>Switch to actions-toolkit implementation by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/811">docker/build-push-action#811</a>  <a href="https://redirect.github.com/docker/build-push-action/pull/838">docker/build-push-action#838</a> <a href="https://redirect.github.com/docker/build-push-action/pull/855">docker/build-push-action#855</a> <a href="https://redirect.github.com/docker/build-push-action/pull/860">docker/build-push-action#860</a> <a href="https://redirect.github.com/docker/build-push-action/pull/875">docker/build-push-action#875</a></li>
<li>e2e: quay.io by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/799">docker/build-push-action#799</a> <a href="https://redirect.github.com/docker/build-push-action/pull/805">docker/build-push-action#805</a></li>
<li>e2e: local harbor and nexus by <a href="https://github.com/crazy-max"><code>@​crazy-max</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/800">docker/build-push-action#800</a></li>
<li>e2e: add artifactory container registry to test against by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/804">docker/build-push-action#804</a></li>
<li>e2e: add distribution tests by <a href="https://github.com/jedevc"><code>@​jedevc</code></a> in <a href="https://redirect.github.com/docker/build-push-action/pull/814">docker/build-push-action#814</a> <a href="https://redirect.github.com/docker/build-push-action/pull/815">docker/build-push-action#815</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/docker/build-push-action/compare/v4.0.0...v4.1.0">https://github.com/docker/build-push-action/compare/v4.0.0...v4.1.0</a></p>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/docker/build-push-action/commit/2cdde995de11925a030ce8070c3d77a52ffcf1c0"><code>2cdde99</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1080">#1080</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li><a href="https://github.com/docker/build-push-action/commit/008747aa03417139ec2995efe44e7f080b8323c3"><code>008747a</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/15807531260fa0e39af66835230d13071751862e"><code>1580753</code></a> chore(deps): Bump <code>@​docker/actions-toolkit</code> from 0.18.0 to 0.19.0</li>
<li><a href="https://github.com/docker/build-push-action/commit/2a7db1d68aab1a514ba647f39bcde60888a1753f"><code>2a7db1d</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1075">#1075</a> from crazy-max/ci-multi-output</li>
<li><a href="https://github.com/docker/build-push-action/commit/35e7dd592106dcd929ef8706706f6d54678d1f67"><code>35e7dd5</code></a> ci: test multi output</li>
<li><a href="https://github.com/docker/build-push-action/commit/af5a7ed5ba88268d5278f7203fb52cd833f66d6e"><code>af5a7ed</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1074">#1074</a> from crazy-max/build-cmd-debug</li>
<li><a href="https://github.com/docker/build-push-action/commit/2a85189a6c719593171342d3d43d4034e8c81513"><code>2a85189</code></a> chore: update generated content</li>
<li><a href="https://github.com/docker/build-push-action/commit/6c2079483ed8cd675d71b5a395b81fa9a19eddc8"><code>6c20794</code></a> disable quotes detection for &quot;outputs&quot; input</li>
<li><a href="https://github.com/docker/build-push-action/commit/afdf0c0a6772ea0bc8c6af61d5dc2df8823c85de"><code>afdf0c0</code></a> chore: debug build cmd and args</li>
<li><a href="https://github.com/docker/build-push-action/commit/00ae31ab6ef216583e63647d8865f52da6b99a13"><code>00ae31a</code></a> Merge pull request <a href="https://redirect.github.com/docker/build-push-action/issues/1070">#1070</a> from docker/dependabot/npm_and_yarn/docker/actions-t...</li>
<li>Additional commits viewable in <a href="https://github.com/docker/build-push-action/compare/v4...v5">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=docker/build-push-action&package-manager=github_actions&previous-version=4&new-version=5)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:27:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4436" class=".btn">#4436</a>
            </td>
            <td>
                <b>
                    Bump actions/setup-java from 3.13.0 to 4.2.1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/setup-java](https://github.com/actions/setup-java) from 3.13.0 to 4.2.1.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/setup-java/releases">actions/setup-java's releases</a>.</em></p>
<blockquote>
<h2>v4.2.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Patch for java version file to accept it from any path by <a href="https://github.com/mahabaleshwars"><code>@​mahabaleshwars</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/610">actions/setup-java#610</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v4...v4.2.1">https://github.com/actions/setup-java/compare/v4...v4.2.1</a></p>
<h2>v4.2.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Updated actions/httpclient version to 2.2.1 and other dependencies by <a href="https://github.com/HarithaVattikuti"><code>@​HarithaVattikuti</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/607">actions/setup-java#607</a></li>
<li>Added .tool-versions file support  along with .java-version file by <a href="https://github.com/mahabaleshwars"><code>@​mahabaleshwars</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/606">actions/setup-java#606</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/HarithaVattikuti"><code>@​HarithaVattikuti</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/607">actions/setup-java#607</a>
<strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v4...v4.2.0">https://github.com/actions/setup-java/compare/v4...v4.2.0</a></li>
</ul>
<h2>V4.1.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Added Windows Arm64 Support for Windows Arm64 Runners by <a href="https://github.com/mahabaleshwars"><code>@​mahabaleshwars</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/595">actions/setup-java#595</a></li>
<li>feat: bump actions/checkout and actions/setup-java to v4 by <a href="https://github.com/kbdharun"><code>@​kbdharun</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/533">actions/setup-java#533</a></li>
<li>Handle authorization when the token is undefined by <a href="https://github.com/peter-murray"><code>@​peter-murray</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/556">actions/setup-java#556</a></li>
<li>Documentation update of Java 21 by <a href="https://github.com/Okeanos"><code>@​Okeanos</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/566">actions/setup-java#566</a></li>
<li>Documentation update about maven-gpg-plugin version note by <a href="https://github.com/IvanZosimov"><code>@​IvanZosimov</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/570">actions/setup-java#570</a></li>
<li>Oracle JDK 21 support by <a href="https://github.com/jdubois"><code>@​jdubois</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/538">actions/setup-java#538</a></li>
<li>Fix typo in configuration example by <a href="https://github.com/Bananeweizen"><code>@​Bananeweizen</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/572">actions/setup-java#572</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/kbdharun"><code>@​kbdharun</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/533">actions/setup-java#533</a></li>
<li><a href="https://github.com/peter-murray"><code>@​peter-murray</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/556">actions/setup-java#556</a></li>
<li><a href="https://github.com/jdubois"><code>@​jdubois</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/538">actions/setup-java#538</a></li>
<li><a href="https://github.com/Bananeweizen"><code>@​Bananeweizen</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/572">actions/setup-java#572</a></li>
<li><a href="https://github.com/mahabaleshwars"><code>@​mahabaleshwars</code></a> made their first contribution in <a href="https://redirect.github.com/actions/setup-java/pull/595">actions/setup-java#595</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/setup-java/compare/v4...v4.1.0">https://github.com/actions/setup-java/compare/v4...v4.1.0</a></p>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<p>In the scope of this release, the version of the Node.js runtime was updated to 20. The majority of dependencies were updated to the latest versions. From now on, the code for the setup-java will run on Node.js 20 instead of Node.js 16.</p>
<h2>Breaking changes</h2>
<ul>
<li>Update Node.js runtime to version 20 by <a href="https://github.com/aparnajyothi-y"><code>@​aparnajyothi-y</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/558">actions/setup-java#558</a></li>
</ul>
<h2>Non-breaking changes</h2>
<ul>
<li>Adding support for microsoft openjdk 21.0.0 by <a href="https://github.com/ralfstuckert"><code>@​ralfstuckert</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/546">actions/setup-java#546</a></li>
<li>Update <code>@​actions/cache</code> dependency and documentation by <a href="https://github.com/IvanZosimov"><code>@​IvanZosimov</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/549">actions/setup-java#549</a></li>
<li>Implementation of the cache-dependency-path option to control caching dependency by <a href="https://github.com/itchyny"><code>@​itchyny</code></a> in <a href="https://redirect.github.com/actions/setup-java/pull/499">actions/setup-java#499</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/setup-java/commit/99b8673ff64fbf99d8d325f52d9a5bdedb8483e9"><code>99b8673</code></a> Patch for java version file (<a href="https://redirect.github.com/actions/setup-java/issues/610">#610</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/5896cecc08fd8a1fbdfaf517e29b571164b031f7"><code>5896cec</code></a> Added  .tool-versions file support (<a href="https://redirect.github.com/actions/setup-java/issues/606">#606</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/80ae3c2885b277a440ee4931b74570716d9a0e27"><code>80ae3c2</code></a> Update httpclient version and other dependencies (<a href="https://redirect.github.com/actions/setup-java/issues/607">#607</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/9704b39bf258b59bc04b50fa2dd55e9ed76b47a8"><code>9704b39</code></a> Added Windows Arm64 Support for Windows Arm64 Runners (<a href="https://redirect.github.com/actions/setup-java/issues/595">#595</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/7a445ee88d4e23b52c33fdc7601e40278616c7f8"><code>7a445ee</code></a> Fix typo in configuration example (<a href="https://redirect.github.com/actions/setup-java/issues/572">#572</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/3232623d9c428cc5f228a01a2ae8d2d70f79775e"><code>3232623</code></a> Oracle JDK 21 support (<a href="https://redirect.github.com/actions/setup-java/issues/538">#538</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/c0660d8edc6bc867c9d061fe281338039e3e0092"><code>c0660d8</code></a> docs: add note about maven-gpg-plugin version (<a href="https://redirect.github.com/actions/setup-java/issues/570">#570</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/2f7af1b9c5646dcf9105b2004b0c5d8f68026bad"><code>2f7af1b</code></a> make it clear that Java 21 is supported (<a href="https://redirect.github.com/actions/setup-java/issues/566">#566</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/16ef37f8dd292a31055a9ee0d26fa0a4efab58de"><code>16ef37f</code></a> HTTP errors when the token is undefined (<a href="https://redirect.github.com/actions/setup-java/issues/556">#556</a>)</li>
<li><a href="https://github.com/actions/setup-java/commit/a2374547dfdd276b7bd9e4ba2c6ba50647d9c8a7"><code>a237454</code></a> feat: bump actions/checkout and actions/setup-java to v4 (<a href="https://redirect.github.com/actions/setup-java/issues/533">#533</a>)</li>
<li>Additional commits viewable in <a href="https://github.com/actions/setup-java/compare/v3.13.0...v4.2.1">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/setup-java&package-manager=github_actions&previous-version=3.13.0&new-version=4.2.1)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:27:33 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4435" class=".btn">#4435</a>
            </td>
            <td>
                <b>
                    Bump actions/checkout from 3 to 4
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">dependencies</span><span class="chip">github_actions</span>
            </td>
            <td>
                Bumps [actions/checkout](https://github.com/actions/checkout) from 3 to 4.
<details>
<summary>Release notes</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/releases">actions/checkout's releases</a>.</em></p>
<blockquote>
<h2>v4.0.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Update default runtime to node20 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li>Support fetching without the --progress option by <a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
<li>Release 4.0.0 by <a href="https://github.com/takost"><code>@​takost</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1447">actions/checkout#1447</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/takost"><code>@​takost</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1436">actions/checkout#1436</a></li>
<li><a href="https://github.com/simonbaird"><code>@​simonbaird</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1067">actions/checkout#1067</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v4.0.0">https://github.com/actions/checkout/compare/v3...v4.0.0</a></p>
<h2>v3.6.0</h2>
<h2>What's Changed</h2>
<ul>
<li>Mark test scripts with Bash'isms to be run via Bash by <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1377">actions/checkout#1377</a></li>
<li>Add option to fetch tags even if fetch-depth &gt; 0 by <a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li>Release 3.6.0 by <a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/RobertWieczoreck"><code>@​RobertWieczoreck</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/579">actions/checkout#579</a></li>
<li><a href="https://github.com/luketomlinson"><code>@​luketomlinson</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1437">actions/checkout#1437</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.3...v3.6.0">https://github.com/actions/checkout/compare/v3.5.3...v3.6.0</a></p>
<h2>v3.5.3</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Checkout Issue in self hosted runner due to faulty submodule check-ins by <a href="https://github.com/megamanics"><code>@​megamanics</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li>Fix typos found by codespell by <a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li>Add support for sparse checkouts by <a href="https://github.com/dscho"><code>@​dscho</code></a> and <a href="https://github.com/dfdez"><code>@​dfdez</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
<li>Release v3.5.3 by <a href="https://github.com/TingluoHuang"><code>@​TingluoHuang</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1376">actions/checkout#1376</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/megamanics"><code>@​megamanics</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1196">actions/checkout#1196</a></li>
<li><a href="https://github.com/DimitriPapadopoulos"><code>@​DimitriPapadopoulos</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1287">actions/checkout#1287</a></li>
<li><a href="https://github.com/dfdez"><code>@​dfdez</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1369">actions/checkout#1369</a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3...v3.5.3">https://github.com/actions/checkout/compare/v3...v3.5.3</a></p>
<h2>v3.5.2</h2>
<h2>What's Changed</h2>
<ul>
<li>Fix: Use correct API url / endpoint in GHES by <a href="https://github.com/fhammerl"><code>@​fhammerl</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1289">actions/checkout#1289</a> based on <a href="https://redirect.github.com/actions/checkout/issues/1286">#1286</a> by <a href="https://github.com/1newsr"><code>@​1newsr</code></a></li>
</ul>
<p><strong>Full Changelog</strong>: <a href="https://github.com/actions/checkout/compare/v3.5.1...v3.5.2">https://github.com/actions/checkout/compare/v3.5.1...v3.5.2</a></p>
<h2>v3.5.1</h2>
<h2>What's Changed</h2>
<ul>
<li>Improve checkout performance on Windows runners by upgrading <code>@​actions/github</code> dependency by <a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<h2>New Contributors</h2>
<ul>
<li><a href="https://github.com/BrettDong"><code>@​BrettDong</code></a> made their first contribution in <a href="https://redirect.github.com/actions/checkout/pull/1246">actions/checkout#1246</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/actions/checkout/blob/main/CHANGELOG.md">actions/checkout's changelog</a>.</em></p>
<blockquote>
<h1>Changelog</h1>
<h2>v4.1.2</h2>
<ul>
<li>Fix: Disable sparse checkout whenever <code>sparse-checkout</code> option is not present <a href="https://github.com/dscho"><code>@​dscho</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1598">actions/checkout#1598</a></li>
</ul>
<h2>v4.1.1</h2>
<ul>
<li>Correct link to GitHub Docs by <a href="https://github.com/peterbe"><code>@​peterbe</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1511">actions/checkout#1511</a></li>
<li>Link to release page from what's new section by <a href="https://github.com/cory-miller"><code>@​cory-miller</code></a> in <a href="https://redirect.github.com/actions/checkout/pull/1514">actions/checkout#1514</a></li>
</ul>
<h2>v4.1.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1396">Add support for partial checkout filters</a></li>
</ul>
<h2>v4.0.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1067">Support fetching without the --progress option</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1436">Update to node20</a></li>
</ul>
<h2>v3.6.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1377">Fix: Mark test scripts with Bash'isms to be run via Bash</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/579">Add option to fetch tags even if fetch-depth &gt; 0</a></li>
</ul>
<h2>v3.5.3</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1196">Fix: Checkout fail in self-hosted runners when faulty submodule are checked-in</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1287">Fix typos found by codespell</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1369">Add support for sparse checkouts</a></li>
</ul>
<h2>v3.5.2</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1289">Fix api endpoint for GHES</a></li>
</ul>
<h2>v3.5.1</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1246">Fix slow checkout on Windows</a></li>
</ul>
<h2>v3.5.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1237">Add new public key for known_hosts</a></li>
</ul>
<h2>v3.4.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1209">Upgrade codeql actions to v2</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1210">Upgrade dependencies</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1225">Upgrade <code>@​actions/io</code></a></li>
</ul>
<h2>v3.3.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/1045">Implement branch list using callbacks from exec function</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1050">Add in explicit reference to private checkout options</a></li>
<li>[Fix comment typos (that got added in <a href="https://redirect.github.com/actions/checkout/issues/770">#770</a>)](<a href="https://redirect.github.com/actions/checkout/pull/1057">actions/checkout#1057</a>)</li>
</ul>
<h2>v3.2.0</h2>
<ul>
<li><a href="https://redirect.github.com/actions/checkout/pull/942">Add GitHub Action to perform release</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/967">Fix status badge</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1002">Replace datadog/squid with ubuntu/squid Docker image</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/964">Wrap pipeline commands for submoduleForeach in quotes</a></li>
<li><a href="https://redirect.github.com/actions/checkout/pull/1029">Update <code>@​actions/io</code> to 1.1.2</a></li>
</ul>
<!-- raw HTML omitted -->
</blockquote>
<p>... (truncated)</p>
</details>
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/actions/checkout/commit/b4ffde65f46336ab88eb53be808477a3936bae11"><code>b4ffde6</code></a> Link to release page from what's new section (<a href="https://redirect.github.com/actions/checkout/issues/1514">#1514</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8530928916aaef40f59e6f221989ccb31f5759e7"><code>8530928</code></a> Correct link to GitHub Docs (<a href="https://redirect.github.com/actions/checkout/issues/1511">#1511</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/7cdaf2fbc075e6f3b9ca94cfd6cec5adc8a75622"><code>7cdaf2f</code></a> Update CODEOWNERS to Launch team (<a href="https://redirect.github.com/actions/checkout/issues/1510">#1510</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8ade135a41bc03ea155e62e844d188df1ea18608"><code>8ade135</code></a> Prepare 4.1.0 release (<a href="https://redirect.github.com/actions/checkout/issues/1496">#1496</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/c533a0a4cfc4962971818edcfac47a2899e69799"><code>c533a0a</code></a> Add support for partial checkout filters (<a href="https://redirect.github.com/actions/checkout/issues/1396">#1396</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/72f2cec99f417b1a1c5e2e88945068983b7965f9"><code>72f2cec</code></a> Update README.md for V4 (<a href="https://redirect.github.com/actions/checkout/issues/1452">#1452</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/3df4ab11eba7bda6032a0b82a6bb43b11571feac"><code>3df4ab1</code></a> Release 4.0.0 (<a href="https://redirect.github.com/actions/checkout/issues/1447">#1447</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/8b5e8b768746b50394015010d25e690bfab9dfbc"><code>8b5e8b7</code></a> Support fetching without the --progress option (<a href="https://redirect.github.com/actions/checkout/issues/1067">#1067</a>)</li>
<li><a href="https://github.com/actions/checkout/commit/97a652b80035363df47baee5031ec8670b8878ac"><code>97a652b</code></a> Update default runtime to node20 (<a href="https://redirect.github.com/actions/checkout/issues/1436">#1436</a>)</li>
<li>See full diff in <a href="https://github.com/actions/checkout/compare/v3...v4">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=actions/checkout&package-manager=github_actions&previous-version=3&new-version=4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
        Created At 2024-04-16 08:27:30 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4434" class=".btn">#4434</a>
            </td>
            <td>
                <b>
                    [refactor] #4419: Deduplicate triggers with the same wasm code
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">Refactor</span><span class="chip">Optimization</span>
            </td>
            <td>
                ## Description

If trigger was already compiled reuse it.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4419 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

To demonstrate the difference 1000 identical triggers were registered. 

Examination of changes was done on apple silicon machine:

```bash
# might need to: cargo install cargo-instruments
cd client
cargo instruments -t Allocations --example register_1000_triggers --profile profiling
```

Allocation before the change:
![reg_trigger_before](https://github.com/hyperledger/iroha/assets/40040452/3ecd2816-1dc4-4911-959e-9149d5bc70ae)
[before_Launch_register_1000_triggers_2024-04-15_18.01.00_EAAEDBCC.trace.zip](https://github.com/hyperledger/iroha/files/14981280/before_Launch_register_1000_triggers_2024-04-15_18.01.00_EAAEDBCC.trace.zip)

Allocations after the change:
![reg_trigger_after](https://github.com/hyperledger/iroha/assets/40040452/b06e7b13-ab13-4fc5-be6d-cd393e1e0007)
[after_Launch_register_1000_triggers_2024-04-15_17.50.57_31C6FEB5.trace.zip](https://github.com/hyperledger/iroha/files/14981281/after_Launch_register_1000_triggers_2024-04-15_17.50.57_31C6FEB5.trace.zip)


<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 15:44:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4432" class=".btn">#4432</a>
            </td>
            <td>
                <b>
                    [chore]: Add @safinsaf to MAINTAINERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-15 09:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4431" class=".btn">#4431</a>
            </td>
            <td>
                <b>
                    [chore] Add @safinsaf to MAINTAINERS (Iroha 1)
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
        Created At 2024-04-15 09:06:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4430" class=".btn">#4430</a>
            </td>
            <td>
                <b>
                    [fix] #4429: Dont clear trigger execution queue (STABLE)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Check linked issue with description of the problem.

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4429 on the stable branch. <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 15:38:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4428" class=".btn">#4428</a>
            </td>
            <td>
                <b>
                    Feature/dops 3159/ci docker main
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 14:14:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4427" class=".btn">#4427</a>
            </td>
            <td>
                <b>
                    [fix] #4226: Prevent registering genesis Domain or Account
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Disallow registering `genesis` domain or `genesis@genesis` account

### Linked issue

Closes #4226

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [x] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 14:00:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4425" class=".btn">#4425</a>
            </td>
            <td>
                <b>
                    Try fix gcc-10 push
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [x] I've read `CONTRIBUTING.md`
- [x] I've used the standard signed-off commit format (or will squash just before merging)
- [x] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 09:06:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4424" class=".btn">#4424</a>
            </td>
            <td>
                <b>
                    Add gcc-10 to docker push
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">1.x</span>
            </td>
            <td>
                ## Description

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #{issue_number} <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-12 08:47:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4422" class=".btn">#4422</a>
            </td>
            <td>
                <b>
                    [chore] Add Nurzhan Sakén and Dmitry Murzin to MAINTAINERS
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
        Created At 2024-04-11 12:33:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4421" class=".btn">#4421</a>
            </td>
            <td>
                <b>
                    [chore]: Add Nurzhan Sakén to iroha2 MAINTAINERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 12:31:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4416" class=".btn">#4416</a>
            </td>
            <td>
                <b>
                    [chore]: add @dima74 to the CODEOWNERS
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span>
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-11 08:44:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4414" class=".btn">#4414</a>
            </td>
            <td>
                <b>
                    [ci]: Configure Sonarqube and Defectdojo in iroha2 CI
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha2</span><span class="chip">CI</span>
            </td>
            <td>
                ## Description
1. Substitute `llvm-cov` coverage tool by `grcov` (only `grcov` generates coverage reports that are compatible with Sonarqube).
2. Add jobs and steps into workflows to set up `lcov` and `clippy` reports uploading to Sonarqube and Defectdojo.
3. Bump `actions/checkout` somewhere.
4. Update `Dockerfiles.build`.

### Benefits
iroha2 dev code will be analyzed in Sonarqube and Defectdojo tools. Links to services URL will be provide in DM. It has access via corporate LDAP account.

### Note
It would be much better to send generared `clippy` and `lcov` reports from PR workflow where are they actually are generated. But we can't do it since GitHub actions security policies. So, we might try at least to upload them during pushing to dev branch. Hopefully, `dawidd6/action-download-artifact` has a magic to search for the latest uploaded artifact from the particular workflow.

### Checklist

- [ ] I've read `CONTRIBUTING.md`
- [ ] I've used the standard signed-off commit format (or will squash just before merging)
- [ ] All applicable CI checks pass (or I promised to make them pass later)
- [ ] (optional) I've written unit tests for the code changes
- [ ] I replied to all comments after code review, marking all implemented changes with thumbs up

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 13:41:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha/pull/4413" class=".btn">#4413</a>
            </td>
            <td>
                <b>
                    [fix] #4253: Check genesis pub key in genesis round
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">Bug</span><span class="chip">iroha2</span>
            </td>
            <td>
                ## Description

Verify that genesis transaction is indeed signed by genesis. 

<!-- Just describe what you did. -->

<!-- Skip if the title of the PR is self-explanatory -->

### Linked issue

<!-- Duplicate the main issue and add additional issues closed by this PR. -->

Closes #4253 <!-- Replace with an actual number,  -->

<!-- Link if e.g. JIRA issue or  from another repository -->

### Benefits

Not possible to submit wrong genesis.

<!-- EXAMPLE: users can't revoke their own right to revoke rights -->

<!-- HINT:  Add more points to checklist for large draft PRs-->

<!-- USEFUL LINKS 
 - https://www.secondstate.io/articles/dco
 - https://discord.gg/hyperledger (please ask us any questions)
 - https://t.me/hyperledgeriroha (if you prefer telegram)
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-10 12:58:40 +0000 UTC
    </div>
</div>

