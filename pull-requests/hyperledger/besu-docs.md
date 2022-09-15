---
layout: default
title: besu-docs
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu-docs
---

# besu-docs <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu-docs){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1171" class=".btn">#1171</a>
            </td>
            <td>
                <b>
                    Link from system requirements to jvm memory page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 21:21:21 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1170" class=".btn">#1170</a>
            </td>
            <td>
                <b>
                    Distribute troubleshooting content
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

The troubleshooting/FAQ page was removed in the Besu docs restructure (#1085). This PR distributes the content from that page across the site on the relevant pages.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1098 

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] Github Actions workflow
- [ ] Build and QA tools configuration (for example, lint rules or Vale style)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 20:36:42 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    use sha for weekly action
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Signed-off-by: Nicolas MASSART <nicolas.massart@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Use Sha for action version (and allow it in github config) as the @v1 not working on this action.
Using commit sha is more secure anyway.

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed


https://github.com/hyperledger/besu-docs/actions/runs/3052051159

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [x] Github Actions workflow
- [ ] Build and QA tools configuration (for example, lint rules or Vale style)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

NA

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 10:33:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1168" class=".btn">#1168</a>
            </td>
            <td>
                <b>
                    remove circle ci config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                Signed-off-by: Nicolas MASSART <nicolas.massart@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Remove the remains of Circle CI

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed

fixes #1146 

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [x] CircleCI workflow
- [ ] Build and QA tools (for example, lint or vale)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [x] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview


NA

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-14 10:06:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1166" class=".btn">#1166</a>
            </td>
            <td>
                <b>
                    Combine/remove old content
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

Combine/remove content from pages that were omitted in the restructure.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1099 
fixes #1100 

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] CircleCI workflow
- [ ] Build and QA tools (for example, lint or vale)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-12 07:00:59 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1165" class=".btn">#1165</a>
            </td>
            <td>
                <b>
                    add memory management docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: John Alon G <git@grasponcrypto.com>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [X] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [X] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [X] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

Adding documentation for how users can manage memory for the besu jvm.

## Issue fixed

Added missing documentation

## Impacted parts

manage-memory.md in both public and private network sections of documentation

For content changes:

- [X] Documentation content
- [x] Documentation page organization

For tool changes:

- [ ] CircleCI workflow
- [ ] Build and QA tools (for example, lint or vale)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

https://hyperledger-besu--1165.org.readthedocs.build/en/1165

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-11 18:51:06 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1164" class=".btn">#1164</a>
            </td>
            <td>
                <b>
                    add meta verification tag back
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">DocOps</span>
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

add meta verification tag back

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

## Issue fixed

Tag was removed as I thought it was only used once when you verify the site but it has to remain in the pages all the time otherwise you get unverified on Google search console...

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [ ] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] CircleCI workflow
- [ ] Build and QA tools (for example, lint or vale)
- [x] MkDocs templates
- [x] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [ ] You've fixed any issues raised by the tests.
- [ ] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 13:23:54 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/1163" class=".btn">#1163</a>
            </td>
            <td>
                <b>
                    Edit understand metrics page
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Alexandra Tran <alexandra.tran@consensys.net>

## Pull request checklist

Use the following list to make sure your PR fits the Besu documentation quality standard.

### Before creating the pull request

Make sure that:

- [x] [All commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] You've read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] You've [previewed your changes locally](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation).

## Describe the change

<!-- Add a clear and concise description of what your PR changes in the documentation. -->

Edit understand metrics page.

## Issue fixed

<!-- Link to the GitHub issue that your PR addresses.

Add "fixes #{your issue number}" to close the issue automatically when the PR is merged.

If your PR doesn't completely fix the issue, add "see #{your issue number}" to link to the issue
without automatically closing it. -->

fixes #1161 

## Impacted parts

<!-- Check the item from the following lists that your PR impacts. You can check multiple boxes. -->

For content changes:

- [x] Documentation content
- [ ] Documentation page organization

For tool changes:

- [ ] CircleCI workflow
- [ ] Build and QA tools (for example, lint or vale)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] Read the Docs configuration
- [ ] GitHub integration

## After creating your PR and tests have finished

Make sure that:

- [x] You've fixed any issues raised by the tests.
- [x] You've [previewed your changes on Read the Docs](https://wiki.hyperledger.org/display/BESU/Preview+the+documentation)
  and added a [preview link](#preview).

## Preview

<!-- Add the link to preview your changes on Read the Docs.

The link format is "https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/",
where {your PR number} is replaced by the number of this PR.
-->
https://hyperledger-besu--1163.org.readthedocs.build/en/1163/public-networks/how-to/monitor/understand-metrics/
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-09 06:17:35 +0000 UTC
    </div>
</div>

