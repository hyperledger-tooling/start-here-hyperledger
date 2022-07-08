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
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/80" class=".btn">#80</a>
            </td>
            <td>
                <b>
                    Fix docker-compose command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                While working on https://github.com/hyperledger/iroha/issues/1466, I've noted a "docker compose command". I don't think [Compose](https://docs.docker.com/compose/) is a part of default Docker distribution.

If I will try to run it with just `docker` command, I'll see this:

```bash
$ docker compose up
docker: 'compose' is not a docker command.
See 'docker --help'
```

Versions:

```
Docker version 20.10.16, build aa7e414fdc
docker-compose version 1.29.2, build 5becea4c
```

Signed-off-by: 6r1d <vic.6r1d@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-08 15:26:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-2-docs/pull/77" class=".btn">#77</a>
            </td>
            <td>
                <b>
                    #73, #60: Update info about roles, mark statements about the future
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span><span class="chip">iroha2</span>
            </td>
            <td>
                Signed-off-by: Ekaterina Mekhnetsova <mekkatya@gmail.com>

Closes #73 minor adjustments about role registration and role granting
Closes #60 (`<!-- Check: a reference about future releases or work in progress -->` marks all statements that have to be checked regularly as they mention WIP or a future release)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-05 07:55:53 +0000 UTC
    </div>
</div>

