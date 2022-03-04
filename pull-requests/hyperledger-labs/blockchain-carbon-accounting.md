---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/487" class=".btn">#487</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency solidity-coverage to v0.7.20 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [solidity-coverage](https://togithub.com/sc-forks/solidity-coverage) | [`^0.7.13` -> `0.7.20`](https://renovatebot.com/diffs/npm/solidity-coverage/0.7.13/0.7.20) | [![age](https://badges.renovateapi.com/packages/npm/solidity-coverage/0.7.20/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/solidity-coverage/0.7.20/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/solidity-coverage/0.7.20/compatibility-slim/0.7.13)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/solidity-coverage/0.7.20/confidence-slim/0.7.13)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>sc-forks/solidity-coverage</summary>

### [`v0.7.20`](https://togithub.com/sc-forks/solidity-coverage/blob/HEAD/CHANGELOG.md#&#8203;0720--2022-02-15)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/6136b1025fee2285c082bda6cb42ed4630a510b2...6b0dab0ff57720943acc76bc0c6528d888c28d3b)

\===================

-   Remove early V7 Truffle patches  ([https://github.com/sc-forks/solidity-coverage/issues/693](https://togithub.com/sc-forks/solidity-coverage/issues/693))

### [`v0.7.19`](https://togithub.com/sc-forks/solidity-coverage/blob/HEAD/CHANGELOG.md#&#8203;0719--2022-02-09)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/d9d8ecd27b48c55feaf9d14246e2fba0cf27e86c...6136b1025fee2285c082bda6cb42ed4630a510b2)

\===================

-   Update solidity-parser/parser to 0.14.0 - supports solidity user-defined types ([https://github.com/sc-forks/solidity-coverage/issues/689](https://togithub.com/sc-forks/solidity-coverage/issues/689))

### [`v0.7.18`](https://togithub.com/sc-forks/solidity-coverage/blob/HEAD/CHANGELOG.md#&#8203;0718-2022-01-17)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/d2f65c59213c894c90c6f4a60201c7eb32deac6f...d9d8ecd27b48c55feaf9d14246e2fba0cf27e86c)

\=================

-   Add solcOptimizerDetails option to help workaround "stack too deep" errors ([https://github.com/sc-forks/solidity-coverage/issues/683](https://togithub.com/sc-forks/solidity-coverage/issues/683))
-   Add \__SOLIDITY_COVERAGE_RUNNING variable on global HH env for identifying solidity-coverage task from other tasks [https://github.com/sc-forks/solidity-coverage/issues/682](https://togithub.com/sc-forks/solidity-coverage/issues/682)2)
-   Fix hardhat_reset ([https://github.com/sc-forks/solidity-coverage/issues/667](https://togithub.com/sc-forks/solidity-coverage/issues/667))
-   Add new hook and make temporary contracts directory configurable ([https://github.com/sc-forks/solidity-coverage/issues/664](https://togithub.com/sc-forks/solidity-coverage/issues/664))
-   Use internal visibility for fn level hash method defs ([https://github.com/sc-forks/solidity-coverage/issues/660](https://togithub.com/sc-forks/solidity-coverage/issues/660))

### [`v0.7.17`](https://togithub.com/sc-forks/solidity-coverage/compare/71bc199ad5a7dc6d28925f624b32c6b8b02f4a68...d2f65c59213c894c90c6f4a60201c7eb32deac6f)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/71bc199ad5a7dc6d28925f624b32c6b8b02f4a68...d2f65c59213c894c90c6f4a60201c7eb32deac6f)

### [`v0.7.16`](https://togithub.com/sc-forks/solidity-coverage/blob/HEAD/CHANGELOG.md#&#8203;0716--2021-03-04)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/72d6e4198447ce9437ca995d979d516e16b8bb95...71bc199ad5a7dc6d28925f624b32c6b8b02f4a68)

\===================

-   Update [@&#8203;solidity-parser/parser](https://togithub.com/solidity-parser/parser) to ^0.12.0 (and support Panic keyword in catch clauses) ([https://github.com/sc-forks/solidity-coverage/issues/621](https://togithub.com/sc-forks/solidity-coverage/issues/621))

### [`v0.7.15`](https://togithub.com/sc-forks/solidity-coverage/blob/HEAD/CHANGELOG.md#&#8203;0715--2021-02-16)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/abc0aa2977269124227990030bd2f79ef77381a6...72d6e4198447ce9437ca995d979d516e16b8bb95)

\===================

-   Fix ctrl-c not exiting on Hardhat ([https://github.com/sc-forks/solidity-coverage/issues/616](https://togithub.com/sc-forks/solidity-coverage/issues/616))
-   Fix bug instrumentation bug w/ "pragma abicoder v2" ([https://github.com/sc-forks/solidity-coverage/issues/615](https://togithub.com/sc-forks/solidity-coverage/issues/615))
-   Update changelog: v0.7.14

### [`v0.7.14`](https://togithub.com/sc-forks/solidity-coverage/blob/HEAD/CHANGELOG.md#&#8203;0714--2021-01-14)

[Compare Source](https://togithub.com/sc-forks/solidity-coverage/compare/0f47eb6c9755e40d11bce6118910fc94390d919a...abc0aa2977269124227990030bd2f79ef77381a6)

\===================

-   Support file scoped function definitions for solc >= 0.7.4
-   Upgrade [@&#8203;solidity-parser/parser](https://togithub.com/solidity-parser/parser) to v0.11.0

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 23:31:27 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/486" class=".btn">#486</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency prettier-plugin-solidity to v1.0.0-beta.19 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [prettier-plugin-solidity](https://togithub.com/prettier-solidity/prettier-plugin-solidity) | [`^1.0.0-beta.2` -> `1.0.0-beta.19`](https://renovatebot.com/diffs/npm/prettier-plugin-solidity/1.0.0-beta.2/1.0.0-beta.19) | [![age](https://badges.renovateapi.com/packages/npm/prettier-plugin-solidity/1.0.0-beta.19/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/prettier-plugin-solidity/1.0.0-beta.19/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/prettier-plugin-solidity/1.0.0-beta.19/compatibility-slim/1.0.0-beta.2)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/prettier-plugin-solidity/1.0.0-beta.19/confidence-slim/1.0.0-beta.2)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>prettier-solidity/prettier-plugin-solidity</summary>

### [`v1.0.0-beta.19`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.19)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.18...v1.0.0-beta.19)

Changes in this version:

-   🔧  node 12 is no longer supported. [#&#8203;598](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/598) thanks [@&#8203;mattiaerre](https://togithub.com/mattiaerre)
-   🐛  fixed bug for pragma statements containing multiple versions. [#&#8203;583](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/583) thanks [@&#8203;fvictorio](https://togithub.com/fvictorio)
-   ✨ added support for user defined types. [#&#8203;607](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/607) thanks [@&#8203;zemse](https://togithub.com/zemse)

### [`v1.0.0-beta.18`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.18)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.17...v1.0.0-beta.18)

### Description

-   [#&#8203;565](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/565)
-   [#&#8203;570](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/570)
-   [#&#8203;575](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/575)

### [`v1.0.0-beta.17`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.17)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.16...v1.0.0-beta.17)

This release contains 2 main improvements:

-   indentation in chained elements:

```Solidity
// v1.0.0-beta.16
uint foo = someLongFunction(
    foo,
    bar,
    baz
)
.someOtherFunctionA(
    foo,
    bar,
    baz
)
.someOtherFunctionB(
    foo,
    bar,
    baz
)

// v1.0.0-beta.17
uint foo = someLongFunction(
    foo,
    bar,
    baz
)
    .someOtherFunctionA(
        foo,
        bar,
        baz
    )
    .someOtherFunctionB(
        foo,
        bar,
        baz
    )
```

-   Bug fix for long variable declarations

```Solidity
// input
function isAuthorized(
    bytes32 serviceId,
    address client
) external view override returns (bool) {
    WhitelistStatus storage whitelistStatus = serviceIdToClientToWhitelistStatus[serviceId][client];
    return true;
}

// v1.0.0-beta.16
function isAuthorized(bytes32 serviceId, address client)
    external
    view
    override
    returns (bool)
{

        WhitelistStatus storage whitelistStatus
     = serviceIdToClientToWhitelistStatus[serviceId][client];
    return true;
}

// v1.0.0-beta.17
function isAuthorized(bytes32 serviceId, address client)
    external
    view
    override
    returns (bool)
{
    WhitelistStatus
        storage whitelistStatus = serviceIdToClientToWhitelistStatus[
            serviceId
        ][client];
    return true;
}
```

Special thanks to [@&#8203;acenolaza](https://togithub.com/acenolaza) ([#&#8203;564](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/564)) and [@&#8203;passabilities](https://togithub.com/passabilities) ([#&#8203;562](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/562)) for their help.

### [`v1.0.0-beta.16`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.16)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.15...v1.0.0-beta.16)

This release contains a bug fix and an improvement in our opinionated standardised code.

-   ([#&#8203;557](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/557)) We fixed a problem in our indentation in `MemberAccess` chains.

```Solidity
// input
int256 amount = SafeCast.toInt256(amount.mul(10**(18 - underlyingAssetDecimals))).neg();

// v1.0.0-beta.15
int256 amount = SafeCast
.toInt256(amount.mul(10**(18 - underlyingAssetDecimals)))
.neg();

// v1.0.0-beta.16
int256 amount = SafeCast
    .toInt256(amount.mul(10**(18 - underlyingAssetDecimals)))
    .neg();
```

-   ([#&#8203;555](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/555)) We also made the decision to enforce parentheses in `ModifierDeclaration`s without parameters,

```Solidity
// input
modifier onlyOwner {
    require(owner() == _msgSender(), "Ownable: caller is not the owner");
    _;
}

// v1.0.0-beta.15
modifier onlyOwner {
    require(owner() == _msgSender(), "Ownable: caller is not the owner");
    _;
}

// v1.0.0-beta.16
modifier onlyOwner() {
    require(owner() == _msgSender(), "Ownable: caller is not the owner");
    _;
}
```

and remove them from `ModifierInvocation`s without arguments.

```Solidity
// input
function renounceOwnership() public virtual onlyOwner() {
    _setOwner(address(0));
}

// v1.0.0-beta.15
function renounceOwnership() public virtual onlyOwner() {
    _setOwner(address(0));
}

// v1.0.0-beta.16
function renounceOwnership() public virtual onlyOwner {
    _setOwner(address(0));
}
```

### [`v1.0.0-beta.15`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.15)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.14...v1.0.0-beta.15)

This release adds a runtime security check for Prettier's version.
The printing process will throw if Prettier's version does not satisfy the range `>=2.3.0`

### [`v1.0.0-beta.14`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.14)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.13...v1.0.0-beta.14)

Release `v1.0.0-beta.14` comes with a new [option](https://togithub.com/prettier-solidity/prettier-plugin-solidity#compiler-experimental) for the configuration file. You can use the `compiler` option to help `prettier-plugin-solidity` choose a appropriate formats.

along this mayor change the release includes these other minor changes:

-   internal changes [#&#8203;531](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/531), [#&#8203;532](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/532), [#&#8203;539](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/539), [#&#8203;540](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/540)
-   improvements in the documentation [#&#8203;537](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/537), [#&#8203;548](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/548)

### [`v1.0.0-beta.13`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.13)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.12...v1.0.0-beta.13)

### Description

In v1.0.0-beta.12 we used a new feature provided by `prettier 2.3.0` that allowed us to simplify our codebase drastically. However Prettier was declared as a dependency, thus nom did not enforce the installation of `prettier v2.3.0` in existing projects. By declaring it as a peerDependency we hope to warn developers of the new requirement.

### [`v1.0.0-beta.12`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.12)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.11...v1.0.0-beta.12)

### Description

-   [#&#8203;513](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/513)

-   [#&#8203;514](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/514)

-   [#&#8203;515](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/515)

-   [#&#8203;516](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/516)

-   [#&#8203;517](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/517)

-   [#&#8203;518](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/518)

-   [#&#8203;519](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/519)

-   [#&#8203;520](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/520)

-   [#&#8203;524](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/524)

-   [#&#8203;527](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/527)

Wow, huge release; thanks [@&#8203;Janther](https://togithub.com/Janther) and [@&#8203;fvictorio](https://togithub.com/fvictorio)

### [`v1.0.0-beta.11`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.11)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.10...v1.0.0-beta.11)

### Description

-   [#&#8203;502](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/502)

-   [#&#8203;499](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/499)

### [`v1.0.0-beta.10`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.10)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.9...v1.0.0-beta.10)

### Description

-   [#&#8203;478](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/478)

-   [#&#8203;480](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/480)

### [`v1.0.0-beta.9`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.9)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.8...v1.0.0-beta.9)

### Description

-   [#&#8203;461](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/461)

-   [#&#8203;473](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/473)

### [`v1.0.0-beta.8`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.8)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.7...v1.0.0-beta.8)

### Description

-   [#&#8203;462](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/462)

-   [#&#8203;466](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/466)

-   [#&#8203;468](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/468)

-   [#&#8203;470](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/470)

### [`v1.0.0-beta.7`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.7)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.6...v1.0.0-beta.7)

### Description

-   [#&#8203;447](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/447)

-   [#&#8203;448](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/448)

-   [#&#8203;452](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/452)

-   [#&#8203;456](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/456)

-   [#&#8203;459](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/459)

shout out to [@&#8203;Janther](https://togithub.com/Janther) for this one 🎉

### [`v1.0.0-beta.6`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.6)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.5...v1.0.0-beta.6)

### Description

-   [#&#8203;444](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/444)

### [`v1.0.0-beta.5`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.5)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.4...v1.0.0-beta.5)

### Description

-   [#&#8203;433](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/433)

-   [#&#8203;435](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/435)

### [`v1.0.0-beta.4`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.4)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.3...v1.0.0-beta.4)

### Description

-   [#&#8203;428](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/428)

### [`v1.0.0-beta.3`](https://togithub.com/prettier-solidity/prettier-plugin-solidity/releases/v1.0.0-beta.3)

[Compare Source](https://togithub.com/prettier-solidity/prettier-plugin-solidity/compare/v1.0.0-beta.2...v1.0.0-beta.3)

### Description

-   [#&#8203;416](https://togithub.com/prettier-solidity/prettier-plugin-solidity/issues/416)

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 23:10:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/485" class=".btn">#485</a>
            </td>
            <td>
                <b>
                    feat(OrbitDBService): Calculate emissions using scope-wise emissions factors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds functions to allow the OrbitDB service to
* Query emissions factors by scope
* Query emissions factors by activity
* Calculate activity emissions based on scope-wise emission data
Special UOMs such as tonne.km and passenger.km have also been accounted for in these functions.

A sample activity and calculation has also been given in the `getData.ts` file.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-03 09:13:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/484" class=".btn">#484</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency nodemon to v2.0.15 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [nodemon](https://nodemon.io) ([source](https://togithub.com/remy/nodemon)) | [`^2.0.12` -> `2.0.15`](https://renovatebot.com/diffs/npm/nodemon/2.0.12/2.0.15) | [![age](https://badges.renovateapi.com/packages/npm/nodemon/2.0.15/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/nodemon/2.0.15/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/nodemon/2.0.15/compatibility-slim/2.0.12)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/nodemon/2.0.15/confidence-slim/2.0.12)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>remy/nodemon</summary>

### [`v2.0.15`](https://togithub.com/remy/nodemon/releases/v2.0.15)

[Compare Source](https://togithub.com/remy/nodemon/compare/v2.0.14...v2.0.15)

##### Bug Fixes

-   bump prod dep versions ([54784ab](https://togithub.com/remy/nodemon/commit/54784ab842a220777958cf590a49c5d9721f9834))

### [`v2.0.14`](https://togithub.com/remy/nodemon/releases/v2.0.14)

[Compare Source](https://togithub.com/remy/nodemon/compare/v2.0.13...v2.0.14)

##### Bug Fixes

-   add windows signals SIGUSR2 & SIGUSR1 to terminate the process ([#&#8203;1938](https://togithub.com/remy/nodemon/issues/1938)) ([61e7abd](https://togithub.com/remy/nodemon/commit/61e7abd730839979c3ec099830d4af7030a6ce3f)), closes [#&#8203;1903](https://togithub.com/remy/nodemon/issues/1903) [#&#8203;1915](https://togithub.com/remy/nodemon/issues/1915) [#&#8203;1936](https://togithub.com/remy/nodemon/issues/1936) [#&#8203;1937](https://togithub.com/remy/nodemon/issues/1937) [#&#8203;1882](https://togithub.com/remy/nodemon/issues/1882) [#&#8203;1893](https://togithub.com/remy/nodemon/issues/1893)

### [`v2.0.13`](https://togithub.com/remy/nodemon/releases/v2.0.13)

[Compare Source](https://togithub.com/remy/nodemon/compare/v2.0.12...v2.0.13)

##### Bug Fixes

-   bump update-notifier ([90e7a3e](https://togithub.com/remy/nodemon/commit/90e7a3e1e2426098f0a849558ac9086fb4e75710)), closes [#&#8203;1919](https://togithub.com/remy/nodemon/issues/1919)
-   release process on main ([9f82a48](https://togithub.com/remy/nodemon/commit/9f82a48ff4f18a7bf0ce3f398ef5fd2be143d57d))

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 17:17:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/483" class=".btn">#483</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency hardhat-gas-reporter to v1.0.8 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [hardhat-gas-reporter](https://togithub.com/cgewecke/hardhat-gas-reporter) | [`^1.0.4` -> `1.0.8`](https://renovatebot.com/diffs/npm/hardhat-gas-reporter/1.0.4/1.0.8) | [![age](https://badges.renovateapi.com/packages/npm/hardhat-gas-reporter/1.0.8/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/hardhat-gas-reporter/1.0.8/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/hardhat-gas-reporter/1.0.8/compatibility-slim/1.0.4)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/hardhat-gas-reporter/1.0.8/confidence-slim/1.0.4)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>cgewecke/hardhat-gas-reporter</summary>

### [`v1.0.8`](https://togithub.com/cgewecke/hardhat-gas-reporter/blob/HEAD/CHANGELOG.md#&#8203;108--2022-02-15)

[Compare Source](https://togithub.com/cgewecke/hardhat-gas-reporter/compare/v1.0.7...v1.0.8)

-   Skip gas reporting when --parallel flag detected ([https://github.com/cgewecke/hardhat-gas-reporter/issues/101](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/101))

### [`v1.0.7`](https://togithub.com/cgewecke/hardhat-gas-reporter/blob/HEAD/CHANGELOG.md#&#8203;107--2022-01-09)

[Compare Source](https://togithub.com/cgewecke/hardhat-gas-reporter/compare/v1.0.6...v1.0.7)

-   Pin colors.js to 1.4.0

### [`v1.0.6`](https://togithub.com/cgewecke/hardhat-gas-reporter/blob/HEAD/CHANGELOG.md#&#8203;106--2021-11-29)

[Compare Source](https://togithub.com/cgewecke/hardhat-gas-reporter/compare/v1.0.5...v1.0.6)

-   Add missing config TS types for multi chain gas prices ([https://github.com/cgewecke/hardhat-gas-reporter/issues/81](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/81))

### [`v1.0.5`](https://togithub.com/cgewecke/hardhat-gas-reporter/blob/HEAD/CHANGELOG.md#&#8203;105--2021-11-29)

[Compare Source](https://togithub.com/cgewecke/hardhat-gas-reporter/compare/v1.0.4...v1.0.5)

-   Fix remote data fetching race condition ([https://github.com/cgewecke/hardhat-gas-reporter/issues/80](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/80))
    -   Update eth-gas-reporter to 0.2.23 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/80](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/80))
    -   Add gas reporter merge task ([https://github.com/cgewecke/hardhat-gas-reporter/issues/75](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/75))
    -   Bump y18n from 3.2.1 to 3.2.2 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/61](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/61))
    -   Bump hosted-git-info from 2.8.8 to 2.8.9 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/64](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/64))
    -   Bump normalize-url from 4.5.0 to 4.5.1 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/66](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/66))
    -   Bump glob-parent from 5.1.1 to 5.1.2 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/67](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/67))
    -   Bump tar from 4.4.13 to 4.4.15 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/70](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/70))
    -   Bump path-parse from 1.0.6 to 1.0.7 ([https://github.com/cgewecke/hardhat-gas-reporter/issues/71](https://togithub.com/cgewecke/hardhat-gas-reporter/issues/71))
        dependabot

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 17:00:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/482" class=".btn">#482</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency hardhat-deploy-ethers to v0.3.0-beta.13 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [hardhat-deploy-ethers](https://togithub.com/wighawag/hardhat-deploy-ethers) | [`^0.3.0-beta.7` -> `0.3.0-beta.13`](https://renovatebot.com/diffs/npm/hardhat-deploy-ethers/0.3.0-beta.7/0.3.0-beta.13) | [![age](https://badges.renovateapi.com/packages/npm/hardhat-deploy-ethers/0.3.0-beta.13/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/hardhat-deploy-ethers/0.3.0-beta.13/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/hardhat-deploy-ethers/0.3.0-beta.13/compatibility-slim/0.3.0-beta.7)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/hardhat-deploy-ethers/0.3.0-beta.13/confidence-slim/0.3.0-beta.7)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>wighawag/hardhat-deploy-ethers</summary>

### [`v0.3.0-beta.13`](https://togithub.com/wighawag/hardhat-deploy-ethers/blob/HEAD/CHANGELOG.md#&#8203;030-beta13)

[Compare Source](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/v0.3.0-beta.12...v0.3.0-beta.13)

##### Patch Changes

-   follow hardhat-ethers compilation output setup

### [`v0.3.0-beta.12`](https://togithub.com/wighawag/hardhat-deploy-ethers/blob/HEAD/CHANGELOG.md#&#8203;030-beta12)

[Compare Source](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/dc87dcab772f7bbd3399ad4393801fb7f629845e...v0.3.0-beta.12)

##### Patch Changes

-   support waffle build with missing linkReferences field

### [`v0.3.0-beta.11`](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/v0.3.0-beta.10...dc87dcab772f7bbd3399ad4393801fb7f629845e)

[Compare Source](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/v0.3.0-beta.10...dc87dcab772f7bbd3399ad4393801fb7f629845e)

### [`v0.3.0-beta.10`](https://togithub.com/wighawag/hardhat-deploy-ethers/blob/HEAD/CHANGELOG.md#&#8203;030-beta10)

[Compare Source](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/v0.3.0-beta.9...v0.3.0-beta.10)

##### Patch Changes

-   remove unecessary file

### [`v0.3.0-beta.9`](https://togithub.com/wighawag/hardhat-deploy-ethers/blob/HEAD/CHANGELOG.md#&#8203;030-beta9)

[Compare Source](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/v0.3.0-beta.8...v0.3.0-beta.9)

##### Patch Changes

-   update from latest hardhat-ethers + fix compatibility issue with typechain

### [`v0.3.0-beta.8`](https://togithub.com/wighawag/hardhat-deploy-ethers/blob/HEAD/CHANGELOG.md#&#8203;030-beta8)

[Compare Source](https://togithub.com/wighawag/hardhat-deploy-ethers/compare/v0.3.0-beta.7...v0.3.0-beta.8)

##### Patch Changes

-   typing on getContract etc..

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 16:59:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/481" class=".btn">#481</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency chai to v4.3.6 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [chai](http://chaijs.com) ([source](https://togithub.com/chaijs/chai)) | [`^4.3.4` -> `4.3.6`](https://renovatebot.com/diffs/npm/chai/4.3.4/4.3.6) | [![age](https://badges.renovateapi.com/packages/npm/chai/4.3.6/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/chai/4.3.6/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/chai/4.3.6/compatibility-slim/4.3.4)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/chai/4.3.6/confidence-slim/4.3.4)](https://docs.renovatebot.com/merge-confidence/) |
| [@types/chai](https://togithub.com/DefinitelyTyped/DefinitelyTyped) | [`^4.2.18` -> `4.3.0`](https://renovatebot.com/diffs/npm/@types%2fchai/4.2.19/4.3.0) | [![age](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/compatibility-slim/4.2.19)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/confidence-slim/4.2.19)](https://docs.renovatebot.com/merge-confidence/) |
| [@types/chai](https://togithub.com/DefinitelyTyped/DefinitelyTyped) | [`^4.2.16` -> `4.3.0`](https://renovatebot.com/diffs/npm/@types%2fchai/4.2.22/4.3.0) | [![age](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/compatibility-slim/4.2.22)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/@types%2fchai/4.3.0/confidence-slim/4.2.22)](https://docs.renovatebot.com/merge-confidence/) |
| [chai](http://chaijs.com) ([source](https://togithub.com/chaijs/chai)) | [`^4.2.0` -> `4.3.6`](https://renovatebot.com/diffs/npm/chai/4.2.0/4.3.6) | [![age](https://badges.renovateapi.com/packages/npm/chai/4.3.6/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/chai/4.3.6/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/chai/4.3.6/compatibility-slim/4.2.0)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/chai/4.3.6/confidence-slim/4.2.0)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>chaijs/chai</summary>

### [`v4.3.6`](https://togithub.com/chaijs/chai/releases/v4.3.6)

[Compare Source](https://togithub.com/chaijs/chai/compare/v4.3.5...v4.3.6)

Update loupe to 2.3.1

### [`v4.3.5`](https://togithub.com/chaijs/chai/releases/v4.3.5)

[Compare Source](https://togithub.com/chaijs/chai/compare/v4.3.4...v4.3.5)

-   build chaijs  [`fca5bb1`](https://togithub.com/chaijs/chai/commit/fca5bb1)
-   build(deps-dev): bump codecov from 3.1.0 to 3.7.1 ([#&#8203;1446](https://togithub.com/chaijs/chai/issues/1446))  [`747eb4e`](https://togithub.com/chaijs/chai/commit/747eb4e)
-   fix package.json exports  [`022c2fa`](https://togithub.com/chaijs/chai/commit/022c2fa)
-   fix: package.json - deprecation warning on exports field ([#&#8203;1400](https://togithub.com/chaijs/chai/issues/1400))  [`5276af6`](https://togithub.com/chaijs/chai/commit/5276af6)
-   feat: use chaijs/loupe for inspection ([#&#8203;1401](https://togithub.com/chaijs/chai/issues/1401)) ([#&#8203;1407](https://togithub.com/chaijs/chai/issues/1407))  [`c8a4e00`](https://togithub.com/chaijs/chai/commit/c8a4e00)

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about these updates again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 15:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/480" class=".btn">#480</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency @types/uuid to v8.3.4 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [@types/uuid](https://togithub.com/DefinitelyTyped/DefinitelyTyped) | [`^8.3.1` -> `8.3.4`](https://renovatebot.com/diffs/npm/@types%2fuuid/8.3.1/8.3.4) | [![age](https://badges.renovateapi.com/packages/npm/@types%2fuuid/8.3.4/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/@types%2fuuid/8.3.4/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/@types%2fuuid/8.3.4/compatibility-slim/8.3.1)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/@types%2fuuid/8.3.4/confidence-slim/8.3.1)](https://docs.renovatebot.com/merge-confidence/) |

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 15:42:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/479" class=".btn">#479</a>
            </td>
            <td>
                <b>
                    build(deps): bump plist from 3.0.2 to 3.0.4 in /open-offsets-directory/react
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [plist](https://github.com/TooTallNate/node-plist) from 3.0.2 to 3.0.4.
<details>
<summary>Changelog</summary>
<p><em>Sourced from <a href="https://github.com/TooTallNate/plist.js/blob/master/History.md">plist's changelog</a>.</em></p>
<blockquote>
<h1>3.0.4 / 2021-08-27</h1>
<ul>
<li>inline xmldom@0.6.0 to eliminate security warning false positive (Mike Reinstein)</li>
</ul>
<h1>3.0.3 / 2021-08-04</h1>
<ul>
<li>update xmldom to 0.6.0 to patch critical vulnerability (Mike Reinstein)</li>
<li>remove flaky saucelabs teseting badge (Mike Reinstein)</li>
</ul>
</blockquote>
</details>
<details>
<summary>Commits</summary>
<ul>
<li>See full diff in <a href="https://github.com/TooTallNate/node-plist/commits">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=plist&package-manager=npm_and_yarn&previous-version=3.0.2&new-version=3.0.4)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 02:42:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/478" class=".btn">#478</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency plist to 3.0.4 [security]
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change |
|---|---|
| plist | [`3.0.2` -> `3.0.4`](https://renovatebot.com/diffs/npm/plist/3.0.2/3.0.4) |

### GitHub Vulnerability Alerts

#### [CVE-2022-22912](https://nvd.nist.gov/vuln/detail/CVE-2022-22912)

Prototype pollution vulnerability via .parse() in Plist before v3.0.4 allows attackers to cause a Denial of Service (DoS) and may lead to remote code execution.

---

### Configuration

📅 **Schedule**: "" (UTC).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-02 02:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/477" class=".btn">#477</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency @types/mocha to v8.2.3 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [@types/mocha](https://togithub.com/DefinitelyTyped/DefinitelyTyped) | [`^8.2.2` -> `8.2.3`](https://renovatebot.com/diffs/npm/@types%2fmocha/8.2.2/8.2.3) | [![age](https://badges.renovateapi.com/packages/npm/@types%2fmocha/8.2.3/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/@types%2fmocha/8.2.3/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/@types%2fmocha/8.2.3/compatibility-slim/8.2.2)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/@types%2fmocha/8.2.3/confidence-slim/8.2.2)](https://docs.renovatebot.com/merge-confidence/) |

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [x] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 23:25:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/476" class=".btn">#476</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency @types/chai-as-promised to v7.1.5 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [@types/chai-as-promised](https://togithub.com/DefinitelyTyped/DefinitelyTyped) | [`^7.1.4` -> `7.1.5`](https://renovatebot.com/diffs/npm/@types%2fchai-as-promised/7.1.4/7.1.5) | [![age](https://badges.renovateapi.com/packages/npm/@types%2fchai-as-promised/7.1.5/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/@types%2fchai-as-promised/7.1.5/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/@types%2fchai-as-promised/7.1.5/compatibility-slim/7.1.4)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/@types%2fchai-as-promised/7.1.5/confidence-slim/7.1.4)](https://docs.renovatebot.com/merge-confidence/) |

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [x] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-01 22:08:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/473" class=".btn">#473</a>
            </td>
            <td>
                <b>
                    build(deps): bump url-parse from 1.5.7 to 1.5.10 in /net-emissions-token-network/interface
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependencies</span><span class="chip">javascript</span>
            </td>
            <td>
                Bumps [url-parse](https://github.com/unshiftio/url-parse) from 1.5.7 to 1.5.10.
<details>
<summary>Commits</summary>
<ul>
<li><a href="https://github.com/unshiftio/url-parse/commit/8cd4c6c6435c1ea32243ec20c9cfe535251ec524"><code>8cd4c6c</code></a> 1.5.10</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ce7a01f2e10738b17812f57c7b6b5de4ea4c0298"><code>ce7a01f</code></a> [fix] Improve handling of empty port</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/00714900ea1e8ba0a1f87b9f8399001e47f060ec"><code>0071490</code></a> [doc] Update JSDoc comment</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/a7044e3e8bb2308ac0f74264d01951aeaca0d66f"><code>a7044e3</code></a> [minor] Use more descriptive variable name</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d547792414a414b2f341a805141beafee728addf"><code>d547792</code></a> [security] Add credits for CVE-2022-0691</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/ad23357ad5fd9a6b011d049466e9ecff723e52b8"><code>ad23357</code></a> 1.5.9</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/0e3fb542d60ddbf6933f22eb9b1e06e25eaa5b63"><code>0e3fb54</code></a> [fix] Strip all control characters from the beginning of the URL</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/61864a8eccff714a45d23db85a814e3c6ee0baba"><code>61864a8</code></a> [security] Add credits for CVE-2022-0686</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/bb0104d6439cf7c2662afbd9411e0772a9639664"><code>bb0104d</code></a> 1.5.8</li>
<li><a href="https://github.com/unshiftio/url-parse/commit/d5c64791ef496ca5459ae7f2176a31ea53b127e5"><code>d5c6479</code></a> [fix] Handle the case where the port is specified but empty</li>
<li>Additional commits viewable in <a href="https://github.com/unshiftio/url-parse/compare/1.5.7...1.5.10">compare view</a></li>
</ul>
</details>
<br />


[![Dependabot compatibility score](https://dependabot-badges.githubapp.com/badges/compatibility_score?dependency-name=url-parse&package-manager=npm_and_yarn&previous-version=1.5.7&new-version=1.5.10)](https://docs.github.com/en/github/managing-security-vulnerabilities/about-dependabot-security-updates#about-compatibility-scores)

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
- `@dependabot ignore this major version` will close this PR and stop Dependabot creating any more for this major version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this minor version` will close this PR and stop Dependabot creating any more for this minor version (unless you reopen the PR or upgrade to it yourself)
- `@dependabot ignore this dependency` will close this PR and stop Dependabot creating any more for this dependency (unless you reopen the PR or upgrade to it yourself)
- `@dependabot use these labels` will set the current labels as the default for future PRs for this repo and language
- `@dependabot use these reviewers` will set the current reviewers as the default for future PRs for this repo and language
- `@dependabot use these assignees` will set the current assignees as the default for future PRs for this repo and language
- `@dependabot use this milestone` will set the current milestone as the default for future PRs for this repo and language

You can disable automated security fix PRs for this repo from the [Security Alerts page](https://github.com/hyperledger-labs/blockchain-carbon-accounting/network/alerts).

</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-28 04:44:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/472" class=".btn">#472</a>
            </td>
            <td>
                <b>
                    chore(deps): update dependency @nomiclabs/hardhat-waffle to v2.0.3 signed-off-by: renovate bot <bot@example.com>
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

This PR contains the following updates:

| Package | Change | Age | Adoption | Passing | Confidence |
|---|---|---|---|---|---|
| [@nomiclabs/hardhat-waffle](https://togithub.com/nomiclabs/hardhat) | [`^2.0.1` -> `2.0.3`](https://renovatebot.com/diffs/npm/@nomiclabs%2fhardhat-waffle/2.0.1/2.0.3) | [![age](https://badges.renovateapi.com/packages/npm/@nomiclabs%2fhardhat-waffle/2.0.3/age-slim)](https://docs.renovatebot.com/merge-confidence/) | [![adoption](https://badges.renovateapi.com/packages/npm/@nomiclabs%2fhardhat-waffle/2.0.3/adoption-slim)](https://docs.renovatebot.com/merge-confidence/) | [![passing](https://badges.renovateapi.com/packages/npm/@nomiclabs%2fhardhat-waffle/2.0.3/compatibility-slim/2.0.1)](https://docs.renovatebot.com/merge-confidence/) | [![confidence](https://badges.renovateapi.com/packages/npm/@nomiclabs%2fhardhat-waffle/2.0.3/confidence-slim/2.0.1)](https://docs.renovatebot.com/merge-confidence/) |

---

### Release Notes

<details>
<summary>nomiclabs/hardhat</summary>

### [`v2.0.3`](https://togithub.com/nomiclabs/hardhat/releases/@&#8203;nomiclabs/hardhat-waffle@2.0.3)

[Compare Source](https://togithub.com/nomiclabs/hardhat/compare/@nomiclabs/hardhat-waffle@2.0.2...@nomiclabs/hardhat-waffle@2.0.3)

This is a small patch release that improves how some errors are created.

#### Changelog

-   Improve how errors are created in the hardhat-waffle plugin ([#&#8203;2307](https://togithub.com/nomiclabs/hardhat/issues/2307))

### [`v2.0.2`](https://togithub.com/nomiclabs/hardhat/releases/@&#8203;nomiclabs/hardhat-waffle@2.0.2)

Add support for the hexEqual matcher ([#&#8203;2200](https://togithub.com/nomiclabs/hardhat/issues/2200))

</details>

---

### Configuration

📅 **Schedule**: At any time (no schedule defined).

🚦 **Automerge**: Disabled by config. Please merge this manually once you are satisfied.

♻ **Rebasing**: Whenever PR becomes conflicted, or you tick the rebase/retry checkbox.

🔕 **Ignore**: Close this PR and you won't be reminded about this update again.

---

 - [ ] <!-- rebase-check -->If you want to rebase/retry this PR, click this checkbox.

---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#github/hyperledger-labs/blockchain-carbon-accounting).
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 01:28:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/471" class=".btn">#471</a>
            </td>
            <td>
                <b>
                    finish refactor ups.js to general purpose emissions.js #452
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Finish #452
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-02-25 01:27:42 +0000 UTC
    </div>
</div>

