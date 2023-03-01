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

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4068" class=".btn">#4068</a>
            </td>
            <td>
                <b>
                    Home Button and Text of Side Navigation Menu (backport #4038)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is an automatic backport of pull request #4038 done by [Mergify](https://mergify.com).


---


<details>
<summary>Mergify commands and options</summary>

<br />

More conditions and actions can be found in the [documentation](https://docs.mergify.com/).

You can also trigger Mergify actions by commenting on this pull request:

- `@Mergifyio refresh` will re-evaluate the rules
- `@Mergifyio rebase` will rebase this PR on its base branch
- `@Mergifyio update` will merge the base branch into this PR
- `@Mergifyio backport <destination>` will backport this PR on `<destination>` branch

Additionally, on Mergify [dashboard](https://dashboard.mergify.com/) you can:

- look at your merge queues
- generate the Mergify configuration with the config editor.

Finally, you can contact us on https://mergify.com
</details>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-27 13:55:03 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric/pull/4064" class=".btn">#4064</a>
            </td>
            <td>
                <b>
                    BFT review comments: channelparticipation.Join
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Change-Id: I92a347a6105fbe99e934f8d4686378e58eb984ce


#### Type of change
- Improvement (improvement to code, performance, etc)

#### Description
Addressing review comments on the modification of channelparticipation.Join in the BFT commit.
This reverses the changes made to channelparticipation.Join in the BFT commit and fixes the respective tests accordingly.

Add retry to forwarding of the config-tx that causes a leader to abdicate, reducing the chances of integration test flakes.

#### Related issues
Raft IT flake #4066 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-02-23 14:17:35 +0000 UTC
    </div>
</div>

