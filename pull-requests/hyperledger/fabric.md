---
layout: default
title: fabric
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric
---

# fabric <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4161" class=".btn">#4161</a>
            </td>
            <td>
                <b>
                    chore(ci): try new builers
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
        Created At 2023-04-13 14:43:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4159" class=".btn">#4159</a>
            </td>
            <td>
                <b>
                    Fix failure in 'basic checks'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Bug fix

#### Description

This patch fixes failure during 'basic checks' in the CI. It is possibly caused by the update of Go to v1.20.

#### Additional details

During the "basic checks" job, the command references are compared with the generated ones. Since the Go version is updated to v1.20, the CI job generates slightly different documents from those in the repository, which were generated with the previous versions of Go.

#### Related issues

#4157
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 09:47:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4158" class=".btn">#4158</a>
            </td>
            <td>
                <b>
                    Fix typo regarding current LTS release
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

Fix typo regarding the current LTS release in README
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 09:39:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4157" class=".btn">#4157</a>
            </td>
            <td>
                <b>
                    Add docs for 'ledgerutil verify'
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

- Documentation update

#### Description

This is a backport of #4098 to release-2.5, fixing the failed automated backport #4153.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-04-13 05:27:01 +0000 UTC
    </div>
</div>

