---
layout: default
title: identus-edge-agent-sdk-ts
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/identus-edge-agent-sdk-ts
---

# identus-edge-agent-sdk-ts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/identus-edge-agent-sdk-ts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/259" class=".btn">#259</a>
            </td>
            <td>
                <b>
                    docs: add commit signing notes to CONTRIBUTING
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                fixes : https://github.com/hyperledger/identus-edge-agent-sdk-ts/issues/251

Problem: signing + sign-off are not common for many open-source projects. Barrier to entry
Solution: document it to make it easier to get started

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-22 00:19:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/258" class=".btn">#258</a>
            </td>
            <td>
                <b>
                    fix: next generation building tools and testing framework
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
This PR is part of our technical debt reduction strategy. 

Our previous build was too complex, for several reasons:

1. Having to bundle wasms for both browser and nodejs (when in reality they are or should be the same as we don't use native env functionality like FS, or Window for browser)
2. Lots of workarounds to get all our wasm files working, with some hacky techniques which required to use and stick with older versions of rollup.
3. Rollup is slower than more modern bundling tools like esbuild, swc, etc.
4. Jest is very problematic and has always caused issues when testing complex wasm scenarios, its hard to integrate.


Improvements:
1. Single build for nodejs and browser all use the same functionality
2. No need to bundle both wasm files (x3, didcomm, JWE and anoncreds)
3. We removed all the rollup configurations and replaced them with esbuild, which requires fewer configuration, we just needed the bare minimum.
4. Esbuild first bundles to esm and then to modern cjs
5. We removed JEST and all its heavy configuration and replaced it with vitest and 20 lines of configuration.
6. Build now runs like 2 o 3 times faster, less than 2 seconds
7. Tests run in a browser environment and nodejs environment without any issues
8. Vitest exposes literally all the same dependencies that we used for jest, sinon, etc but in a single package
9. Vitest runs the unitary tests in 4seconds now

Have validated that the browser demo works flawlessly, the nextjs one.

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-20 20:44:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/257" class=".btn">#257</a>
            </td>
            <td>
                <b>
                    fix: improve didcomm error handling through Mercury and edge agent he…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
### Description: 
Improves error handling for didcomm messages when the mediator url is invalid.

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-20 20:19:15 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/255" class=".btn">#255</a>
            </td>
            <td>
                <b>
                    fix: generate docs after releasing as we cannot access a package that…
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                

### Description: 
generate docs after releasing as we cannot access a package that does not exist yet

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 14:08:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/254" class=".btn">#254</a>
            </td>
            <td>
                <b>
                    fix: remove typo in release pipeline
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
typo 

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 13:49:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/253" class=".btn">#253</a>
            </td>
            <td>
                <b>
                    fix: releasing to HL
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
Release to HL

### Checklist: 
- [ ] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [ ] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [ ] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [ ] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 13:18:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/252" class=".btn">#252</a>
            </td>
            <td>
                <b>
                    docs: fix links in README
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                this atalaprism / hyperledger / identus migration has been a bit of a mess.

Here's a little help :heart: :gift: 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 02:24:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/identus-edge-agent-sdk-ts/pull/250" class=".btn">#250</a>
            </td>
            <td>
                <b>
                    docs: link pluto-encrypted as reference implementation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description: 
The current README gives very little info on what's needed for a Pluto implementation

Changes:
- mentioned that it's Pluto.Store you need to implement (not Pluto any more)
- started a "community implementations" section, and linked `pluto-encrypted` work

### Checklist: 
- [x] My PR follows the [contribution guidelines](https://github.com/input-output-hk/atala-prism-wallet-sdk-ts/blob/master/CONTRIBUTING.md) of this project
- [x] My PR is free of third-party dependencies that don't comply with the [Allowlist](https://toc.hyperledger.org/governing-documents/allowed-third-party-license-policy.html#approved-licenses-for-allowlist)
- [ ] I have commented my code, particularly in hard-to-understand areas
- [x] I have made corresponding changes to the documentation
- [ ] I have added tests that prove my fix is effective or that my feature works
- [x] I have checked the PR title to follow the [conventional commit specification](https://www.conventionalcommits.org/en/v1.0.0/)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-19 01:09:13 +0000 UTC
    </div>
</div>

