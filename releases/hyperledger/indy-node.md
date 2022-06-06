---
layout: default
title: indy-node
parent: Hyperledger
grand_parent: Releases
has_children: false
permalink: /releases/hyperledger/indy-node
---

# indy-node <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/indy-node){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td colspan="2">
                <b>
                    v1.13.1-rc2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">
                    v1.13.1-rc2
                </span>
            </td>
            <td>
                [v1.13.1-rc2] 

## What's Changed
* adds GitHub Actions and build containers by @Toktar in https://github.com/hyperledger/indy-node/pull/1648
* chore: Add workflow trigger by @ryjones in https://github.com/hyperledger/indy-node/pull/1649
* UP-34: Add LEDGERS_FREEZE and GET_FROZEN_LEDGERS transactions by @Toktar in https://github.com/hyperledger/indy-node/pull/1641
* UP-37: Test for checking that removing keys doesn't break auth map mechanism by @Toktar in https://github.com/hyperledger/indy-node/pull/1640
* Add script for remove ledger by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1650
* Bump libindy v.1.15.0-1618, bump plenum by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1654
* Bump libindy version for python wrapper by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1655
* Pin pip version for CD by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1657
* Pin pip for cd by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1658
* Repair CD pipeline by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1660
* Bump test-automation version 0.8.43 by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1661
* Add settings file by @ryjones in https://github.com/hyperledger/indy-node/pull/1666
* Update CODEOWNERS by @askolesov in https://github.com/hyperledger/indy-node/pull/1664
* Add docs for freeze transactions by @adenishchenko in https://github.com/hyperledger/indy-node/pull/1656
* Allow test report publishing to fail by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1668
* Add support for publishing Debian packages by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1680
* Fix issue with nightly build. by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1685
* added building and publishing of python artifacts by @udosson in https://github.com/hyperledger/indy-node/pull/1690
* Ubuntu 20.04. CI/CD Pipeline as GitHub Action by @udosson in https://github.com/hyperledger/indy-node/pull/1697
* Support publishing off a development branch by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1698
* Ubuntu 20.04: bug fix: added missing env of distribution in publish_artifacts by @udosson in https://github.com/hyperledger/indy-node/pull/1699
* updated version of setup-jfrog-cli to v2 by @udosson in https://github.com/hyperledger/indy-node/pull/1709
* bump version of indy plenum and added pypi versio to 3rd party artifacts by @udosson in https://github.com/hyperledger/indy-node/pull/1713
* set dependencies for the Cannocical archive by @udosson in https://github.com/hyperledger/indy-node/pull/1714
* updated libsodium from v18 to v23 by @udosson in https://github.com/hyperledger/indy-node/pull/1715
* GHA optimiziation by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1721
* Remove duplicate Sovrin apt-key call by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1723
* Gitpod DevContainer by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1722
* VSCode Devcontainer by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1718
* Fix pytest-asyncio deprecation warnings which are causing the tests to fail. by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1730
* Fixes the Gitpod Link by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1731
* DevContainer documentation by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1732
* Gha Refactoring by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1738
* Fix crash in `indy-node-control` by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1741
* Remove Pip Imports for ubuntu20 by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1743
* did:indy by @dbluhm in https://github.com/hyperledger/indy-node/pull/1740
* Unpin pip by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1744
* Upgrade zmq by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1745
* Add warning filter by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1747
* New Release Workflow & Gha refactoring by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1749
* Pinned indy-shared-gha reference by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1754
* fix importlib-metadata dependency by @mgmgwi in https://github.com/hyperledger/indy-node/pull/1748
* Added Status Check for branch protection by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1756
* Gha release documentation & Removal of Jenkins files by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1752
* Adjust workflow triggers. by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1758
* consistent GHA variable substitution by @pSchlarb in https://github.com/hyperledger/indy-node/pull/1759
* Fix missing component in publish release workflow. by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1760
* Update indy-plenum version. by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1761
* Fix incorrect path filter in PR.yaml by @WadeBarnes in https://github.com/hyperledger/indy-node/pull/1763
* [v1.13.1-rc2] - Update Version Number for Release by @sovbot in https://github.com/hyperledger/indy-node/pull/1764

## New Contributors
* @dbluhm made their first contribution in https://github.com/hyperledger/indy-node/pull/1740
* @mgmgwi made their first contribution in https://github.com/hyperledger/indy-node/pull/1748

**Full Changelog**: https://github.com/hyperledger/indy-node/compare/v1.13.0-rc0...v1.13.1-rc2
            </td>
        </tr>
    </table>
    <a href="https://github.com/hyperledger/indy-node/releases/tag/v1.13.1-rc2" class=".btn">
        View on GitHub
    </a>
    <span class="right-align">
        Created At 2022-06-06 17:09:02 +0000 UTC
    </span>
</div>

