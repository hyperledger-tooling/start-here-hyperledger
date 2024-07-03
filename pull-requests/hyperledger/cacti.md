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
                PR <a href="https://github.com/hyperledger/cacti/pull/3374" class=".btn">#3374</a>
            </td>
            <td>
                <b>
                    fix(plugin-persistence-ethereum): make created_at TIMESTAMPTZ in schema
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The problem was that the database schema was defined in a way that was
destroying timestamp information during insertion of records.
2. Updating the schema to hold the timestamp information made the test pass.

More information about why it's recommended to store datetime data with
the TIMESTAMPTZ column type is explained by the author of the node-postgres
library which is an important part of the problem (it assumes local time
for columns that do not store the timestamp time zone).

https://node-postgres.com/features/types#date--timestamp--timestamptz

Fixes #3373

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
        Created At 2024-07-02 19:41:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3372" class=".btn">#3372</a>
            </td>
            <td>
                <b>
                    chore(weaver): use docker compose v2
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                `Primary change:  Updates the weaver files
to use docker compose v2 syntax.  docker-compose
v1 will be dropped on the github runners
shortly.`

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
        Created At 2024-07-02 14:06:43 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3370" class=".btn">#3370</a>
            </td>
            <td>
                <b>
                    chore(cleanup): deleted deprecated files and folders
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Deleted 'docs-cactus' and 'weaver/docs' folders.
- Ensured that the latest contents in the above are reflected in the 'docs' folder.
- Updated MAINTAINERS.md file with contents from 'weaver/MAINTAINERS.md'.
- Deleted unnecessary 'MAINTAINERS.md' and 'CONTRIBUTING.md' in the 'weaver' folder.
- Fixed indentations and removed dead code in source files.

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-01 19:06:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3369" class=".btn">#3369</a>
            </td>
            <td>
                <b>
                    chore(cacti): use lerna 8.1 instead of lerna lite
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                First step of ci refactoring.
```

Please see ./epics/2024-06-ci-refactoring.md in
this commit for ci refactoring plan.

Primary Change:
 - switch from using lerna lite to lerna 8.1

 Secondary Changes:
 - add ci refactoring plan markdown file
 - lerna.json: remove useWorkspaces, which is not supported by lerna 8.1
 - introduce package.lock, a new file generated
 - package.json: increase memory used when building
 - yarn.lock: introduce lerna 8.1

```
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
        Created At 2024-06-28 16:06:12 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3368" class=".btn">#3368</a>
            </td>
            <td>
                <b>
                    Docs improvements
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR addresses several typographical errors across various files in the project. The changes improve readability and maintain the professional standard of the documentation and code comments.

Justification
Typographical errors, while minor, can detract from the overall quality of the project. Correcting these errors ensures clarity and professionalism, making the project more accessible and understandable for current and future contributors.

Hope it helps.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-06-28 06:42:23 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3367" class=".btn">#3367</a>
            </td>
            <td>
                <b>
                    fix(sync-ts-config): fix no such file or directory tsconfig.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### **Commit** to be reviewed
---
fix(sync-ts-config): fix no such file or directory tsconfig.json
```
Primary Changes
---------------

1. Fix issue with the object key
2. Temporarily added ignore paths for the missing tsconfig.json so the script will run successfully
```

Fixes: #3069 
Related to: #3366

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
        Created At 2024-06-28 03:54:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3365" class=".btn">#3365</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): shutdown hook was not waiting for promises
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The library we use for having async functions handle resource deallocation
was not being used correctly by the API server.
2. The library only supports callback style asynchronous code and the API
server assumed that it could return a promise from the shutdown hooks which
lead to the problem that our shutdown hooks were not being awaited for.

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
        Created At 2024-06-27 03:47:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3364" class=".btn">#3364</a>
            </td>
            <td>
                <b>
                    docs(examples/supply-chain-app): fix resource cleanup of shutdown logic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. Now you can run the supply chain app example locally and then hit CTRL+C
on the terminal and it will gracefully shut down all the containers hosting
the infrastructure and only after that the NodeJS process itself will exit.
2. Previously we had a bug where it wouldn't wait for the containers to wind
down and it left them running which was causing problems when people didn't
notice this behavior and their machines would get into this broken state where
the previous execution's containers were hanging around and one of them blocking
ports too.

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
        Created At 2024-06-27 03:35:41 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3363" class=".btn">#3363</a>
            </td>
            <td>
                <b>
                    docs(examples/supply-chain-app): print correct web host in the CLI logs 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The logs were showing the bound host which in our case was 0.0.0.0
but that is not accepted by web browsers when you are executing HTTP XHR
requests from Javascript.
2. This change makes it so that even though we bind to 0.0.0.0 the logs
to the person running the example application will show 127.0.0.1.
This might potentially cause further confusion in some people who'd think
that we are binding to 127.0.0.1 based on the logs, but this seems like an
acceptable trade-off for an example which has the number one priority of
being easily digestable.

Fixes #2390

Depends on #3362

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
        Created At 2024-06-27 01:56:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/3362" class=".btn">#3362</a>
            </td>
            <td>
                <b>
                    fix(cmd-api-server): stop changing LoggerProvider log level
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. The API server was mutating global shared state in it's own constructor
which was causing problems with other components (pretty much all of them)
2. I deleted the line that copies the API server's own log level to the
LoggerProvider so that the API server's log level can be it's own.
3. The way this bug came about is that in the supply chain app example
in the back-end the API server had to be muted (log level WARN) in order
for it to stop printing misleading logs due to us binding to the wildcard
host it would claim in its own logs that the WWW GUI is accessible on the
wildcard host in a web browser, but this was wrong and caused many people
a lot of confusion unfortunately.
4. The fix for the supply chain app is to set the API server's log level to
WARN and have the supply chain app itself log the correct URLs to the console.
5. The issue I ran into with that fix is that as soon as I set the log level
of the API server to WARN, everything else also stopped logging which resulted
in my fix making everything worse since now the users had absolutely no
idea what was happening or if the example application had even finished booting
up or not.
6. Upon further debugging I discovered that the API server was forcing its
own log level onto everybody else as the root cause.
7. A follow-up PR is about to drop with the supply chain app fixes which are
dependent on this one making it in first.

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
        Created At 2024-06-26 20:09:32 +0000 UTC
    </div>
</div>

