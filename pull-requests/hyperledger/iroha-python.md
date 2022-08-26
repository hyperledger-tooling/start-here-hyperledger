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
                PR <a href="https://github.com/hyperledger/iroha-python/pull/124" class=".btn">#124</a>
            </td>
            <td>
                <b>
                    Create pythonpublish.yml
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Ry Jones <ry@linux.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 15:56:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/iroha-python/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Added Dockerfile to test iroha-python (Iroha 1) in various distros
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">iroha1</span>
            </td>
            <td>
                Some time ago I added some features then created release: [1.4.0](https://github.com/hyperledger/iroha-python/releases/tag/1.4.0). Unfortunately despite working in my OS (Manjaro) it was not working in Ubuntu servers. So I repaired its: https://github.com/hyperledger/iroha-python/pull/104
But this time I wanted to make sure it will work in Manjaro and also in supported Ubuntu LTS, to make the task easier I've created Dockerfile.

The Dockerfile can be useful: 
------
1. When adding changes to protobufs in Iroha 1 (it will rather not happen, but maybe Iroha-Core maintainers would agree for internship project in next year)
2. The Dockerfile with some modifications can help in iroha-python development for Iroha 2.
___________________
Tests (checked if output as expected):
-----
```
docker build . --file Dockerfile_to_test_various_versions_of_library --build-arg 'SYSTEM=ubuntu' --build-arg 'SYSTEM_VERSION=20.04' --tag iroha-python-test:ubuntu_20.04
docker run --rm --network=host iroha-python-test:ubuntu_20.04

docker build . --file Dockerfile_to_test_various_versions_of_library --build-arg 'SYSTEM=ubuntu' --build-arg 'SYSTEM_VERSION=22.04' --tag iroha-python-test:ubuntu_22.04
docker run --rm --network=host iroha-python-test:ubuntu_22.04

docker build . --file Dockerfile_to_test_various_versions_of_library --build-arg 'SYSTEM=manjarolinux/base' --build-arg 'SYSTEM_VERSION=20220807' --tag iroha-python-test:manjaro_20220807
docker run --rm --network=host iroha-python-test:manjaro_20220807
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-08-25 03:09:53 +0000 UTC
    </div>
</div>

