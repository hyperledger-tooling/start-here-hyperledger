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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/2688" class=".btn">#2688</a>
            </td>
            <td>
                <b>
                    Add unit tests for anoncreds revocation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds unit testing for the anoncreds revocation module.

Tried to use the anoncred module as much as possible but when I was having too much trouble I mocked calls that loaded/created objects or converted forms. 

Mocked the database/wallet Entry responses a lot with basic classes. Couldn't find a better way to do this or an examples in the repo.

Coverage is 92%. I tried not to make the tests too brittle but wanted to have good coverage for my own understanding. I'm hoping this will help others trying to understand the code along with having a good testing layout for future refactoring or features.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-21 22:25:10 +0000 UTC
    </div>
</div>

