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
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1858" class=".btn">#1858</a>
            </td>
            <td>
                <b>
                    Unit test fixes for python 3.9
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This partially implements the updates in #1717, for the specific tests that were failing under 3.9. There is some overlap with #1854.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-13 17:42:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-cloudagent-python/pull/1856" class=".btn">#1856</a>
            </td>
            <td>
                <b>
                    Githubaction publish docker image
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi, @swcurran mentioned in today's AcaPug call that you would be interested in a pipeline for building and publishing AcaPy Docker images automatically for every tagged commit.

The GitHub Action below should do this. It is triggered for every tagged commit and will build the docker image using the `docker/Dockerfile.run` file. The images are being published in the GitHub package registry of this repo.

Example: If a commit is tagged with `0.7.4-rc6` an image will automatically be built and published with the following two tags:
1. aries-cloudagent-python:latest
2. aries-cloudagent-python:0.7.4-rc6

You can also see the build image in my forked version of this repo: https://github.com/PaulWen/aries-cloudagent-python/pkgs/container/aries-cloudagent-python


Let me know if this is of any help or if I misunderstood the requirements. I am happy to iterate over it and appreciate any feedback!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-07-12 17:25:03 +0000 UTC
    </div>
</div>

