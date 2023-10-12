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
                PR <a href="https://github.com/hyperledger/cacti/pull/2753" class=".btn">#2753</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add json-rpc proxy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add proxy endpoint handling. Requests sent to this endpoint will be passed directly to the ethereum node.
- Add test to verify that proxy is working.
- Update README of ethereum connector.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-09 12:21:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2751" class=".btn">#2751</a>
            </td>
            <td>
                <b>
                    style(cmd-api-server): fix any linter in getOrCreateWebServices()
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Description:
This pull request addresses issue #2676  by fixing an Unexpected any linter warning in the getOrCreateWebServices() method of the ApiServer class. The warning occurred due to a typecast using (app as any). 

### Changes:
Replaced (app as any) with (app as express.Express)[httpVerbPrometheus as keyof express.Express](httpPathPrometheus, prometheusExporterHandler);

### Importance of keyof:
The use of keyof here is crucial because it ensures that httpVerbPrometheus and httpVerb are treated as the valid key of the express.Express type. This is necessary because HTTP verbs, like GET, POST, PUT etc... should be treated as keys within the express.Express type. By casting httpVerbPrometheus as keyof express.Express, we enforce type safety and prevent potential runtime errors that could occur if an invalid HTTP verb is used. In essence, it ensures that only valid HTTP verbs are accepted, improving the robustness of the code. 

### Benefits:
This change enhances code readability and maintainability using appropriate types and expressions.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 19:26:56 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2750" class=".btn">#2750</a>
            </td>
            <td>
                <b>
                    feat(cactus-plugin-ledger-connector-ethereum): add signing utils
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Add methods for signing transactions to ethereum connector.
- Modify offline signing test to use this new method.
- Modify electricity trade sample to use new signing method.
- Add offline signature section to ethereum connector readme.

**Pull Request Requirements**
[ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
[ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
[ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information.

**Character Limit**
[ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
[ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-06 12:24:52 +0000 UTC
    </div>
</div>

