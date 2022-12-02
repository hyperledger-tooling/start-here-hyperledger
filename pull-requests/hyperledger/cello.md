---
layout: default
title: cello
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cello
---

# cello <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cello){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cello/pull/499" class=".btn">#499</a>
            </td>
            <td>
                <b>
                    Update docker-rest-agent Dep
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docker-rest-agent's dependency list by adding greenlet==1.1.3.

The gevent with a version lower than 20.9.0 will have difficulty working
with greenlet v2 or higher. If no greenlet version is specified, v2 or higher
will be installed automatically, which will crush gevent.

See [StackOverflow](https://stackoverflow.com/questions/34314222/gevent-not-valid-running-docker-registry) and [GitHub Issue](https://github.com/python-greenlet/greenlet/issues/178) for details.

Signed-off-by: xichen1 <xichen.pan@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-12-02 16:44:25 +0000 UTC
    </div>
</div>

