---
layout: default
title: fabric-ca
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-ca
---

# fabric-ca <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-ca){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/274" class=".btn">#274</a>
            </td>
            <td>
                <b>
                    Bump fvt mysql to 0.8.22-1 (backport #273)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">conflicts</span>
            </td>
            <td>
                This is an automatic backport of pull request #273 done by [Mergify](https://mergify.com).
Cherry-pick of bb858908d0356edb678ee2be1ca8345f24d641d0 has failed:
```
On branch mergify/bp/release-1.4/pr-273
Your branch is up to date with 'origin/release-1.4'.

You are currently cherry-picking commit bb858908.
  (fix conflicts and run "git cherry-pick --continue")
  (use "git cherry-pick --skip" to skip this patch)
  (use "git cherry-pick --abort" to cancel the cherry-pick operation)

Unmerged paths:
  (use "git add <file>..." to mark resolution)
	both modified:   images/fabric-ca-fvt/payload/mysql_setup.sh

no changes added to commit (use "git add" and/or "git commit -a")
```


To fix up this pull request, you can check it out locally. See documentation: https://docs.github.com/en/github/collaborating-with-pull-requests/reviewing-changes-in-pull-requests/checking-out-pull-requests-locally

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
        Created At 2022-03-18 22:08:51 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/273" class=".btn">#273</a>
            </td>
            <td>
                <b>
                    Bump fvt mysql to 0.8.22-1
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Bump fvt mysql to 0.8.22-1 to fix FVT docker image build.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 21:00:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-ca/pull/272" class=".btn">#272</a>
            </td>
            <td>
                <b>
                    Make server config.go and serverconfig.rst consistent
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The files got out of sync, they must be identical for builds to succeed.

Signed-off-by: David Enyeart <enyeart@us.ibm.com>

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-03-18 20:15:01 +0000 UTC
    </div>
</div>

