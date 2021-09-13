---
layout: default
title: iroha-python
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-python
---

# iroha-python <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-python){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/83" class=".btn">#83</a>
            </td>
            <td>
                <b>
                    Develop rebase with main branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                In iroha-python library many newest merges was being merged into `main` branch instead of develop, that is why many changes are not available on `develop`.
So I've made:
```
git cherry-pick 41a724b3f3f21921ad455d39fb959f45c98fe986
```
to fetch: https://github.com/hyperledger/iroha-python/commit/41a724b3f3f21921ad455d39fb959f45c98fe986

it will contain commits which change `iroha/iroha.py` file:

1. https://github.com/hyperledger/iroha-python/commit/41a724b3f3f21921ad455d39fb959f45c98fe986
2. https://github.com/hyperledger/iroha-python/commit/92d81772ab5c59b5521f0475300ebbc1e97f5974
3. https://github.com/hyperledger/iroha-python/commit/4d10eb0fb64bb033c950a8b6a63c6fae25fe4373
4. https://github.com/hyperledger/iroha-python/commit/3968c3903c1b7c1c2c1f2519699424416cbbe248

Rest of commits are not cherry-picked (connected with documentation, Jenkins, etc)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-09-13 11:17:41 +0000 UTC
    </div>
</div>

