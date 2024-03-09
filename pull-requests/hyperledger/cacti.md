---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3049" class=".btn">#3049</a>
            </td>
            <td>
                <b>
                    build: upgrade Yarn from v3.6.0 to v4.1.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                **IMPORTANT**: The lock file format has been updated yet again so you
need to run a `yarn install` after pulling this update on the main branch.

This is not technically a breaking change in the software's APIs but it
is in terms of breaking developer's workflows unless a specific set of
instructions (see above) are performed in order to do the migration.

1. Upgraded Yarn to v4. Hopefully I didn't miss any of the places where
the version was/is declared/documented/etc.
2. Also added a new dependency vulnerability audit script which uses
npm's own audit script/mechanism under the hood. Previously this was
broken if you were using Yarn (e.g. pre-v4 releases of Yarn) but now
we can have the dependency auditing done locally which is a great resource
because we no longer have to depend only on GitHub's dependabot to tell
us when a dependency has some vulnerabilities associated with it.

Point 2 is also the motivation behind the upgrade apart from the usual
reason for trying to keep us on the latest and greatest when it comes
to dependencies so that we don't paint ourselves in a corner when old
dependencies start to have hard to fix vulnerabilities.

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-03 04:43:03 +0000 UTC
    </div>
</div>

