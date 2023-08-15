---
layout: default
title: iroha-2-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/iroha-2-docs
---

# iroha-2-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/iroha-2-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/376" class=".btn">#376</a>
            </td>
            <td>
                <b>
                    [chore] Fix client config path (#358)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `cp ./configs/client_cli/config.json test_docker/` command won't work anymore; `cp ./configs/client/config.json test_docker/` would work in `iroha2-dev`, `dae3113496`.

I wonder if we need to do something about the Java and JavaScript articles, as `config.json` is mentioned there briefly, but Bash is the first thing to try. I think I will update those as well.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-15 06:57:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/374" class=".btn">#374</a>
            </td>
            <td>
                <b>
                    [docs] Introducing 'Security' section
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description
Introducing the "Security" section of the documentation. The original documentation—PR #332—has been split for the sake of granularity.

## Changes:
- Original PR #332 turned into the 'Security' section.
- Original topics restructured.
- Additional information added.

## Notes
- The "Password Security" topic is planned to be a part of the next PR.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-08-14 17:55:23 +0000 UTC
    </div>
</div>

