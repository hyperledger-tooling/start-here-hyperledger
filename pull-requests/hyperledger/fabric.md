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
                PR <a href="https://github.com/hyperledger/fabric/pull/4074" class=".btn">#4074</a>
            </td>
            <td>
                <b>
                    Release commit for v2.4.9.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Update docs and release notes for v2.4.9.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 21:10:58 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4073" class=".btn">#4073</a>
            </td>
            <td>
                <b>
                    Backport PR 4011 to release-2.4 (fix IsChannelMember)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I7205dbe264248c4ad534499955bb22710d07444d

#### Type of change

- Bug fix

#### Description
PR 4011 addressed a bug (#3998) in IsChannelMember that manifested itself in the test

`integration/raft/cft_test.go` use-case: "disregards certificate renewal if only the validity period changed"

after it was converted to run without the system channel.

Here we
- Backport the fix (in etcdraft/consenter.go)
- Add the same test case which runs without the system channel (w/o the fix this test case fails).
- Backport some test infrastructure that helps running tests without the system channel.


#### Related issues

#3998 the issue describing the bug
#4011 the PR fixing the bug on main
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 14:15:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4071" class=".btn">#4071</a>
            </td>
            <td>
                <b>
                    Backport PR 4011 to release-2.5 (fix IsChannelMember)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
Change-Id: I7205dbe264248c4ad534499955bb22710d07444d

#### Type of change

- Bug fix

#### Description

PR 4011 addressed a bug (#3998) in IsChannelMember that manifested itself in the test

`integration/raft/cft_test.go` use-case: "disregards certificate renewal if only the validity period changed"

after it was converted to run without the system channel.

Here we
- Backport the fix (in etcdraft/consenter.go)
- Add the same test case which runs without the system channel (w/o the fix this test case fails).
- Backport some test infrastructure that helps running tests without the system channel.

#### Related issues

#3998 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-01 12:00:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4069" class=".btn">#4069</a>
            </td>
            <td>
                <b>
                    Fix typo in documentation
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

This fix replaces the misspelled word "deployements" with the correct spelling "deployments". My motivation is creating my first pull request for the Hyperledger project and getting familiar with the contribution process.

#### Additional details


#### Related issues

https://github.com/hyperledger/fabric/issues/3271

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 21:33:10 +0000 UTC
    </div>
</div>

