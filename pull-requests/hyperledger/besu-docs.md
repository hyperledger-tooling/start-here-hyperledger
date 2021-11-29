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
                PR <a href="https://github.com/hyperledger/besu-docs/pull/882" class=".btn">#882</a>
            </td>
            <td>
                <b>
                    update IBFT2.0 transitions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Roland Tyler <roland.tyler@consensys.net>

## Pull request checklist

## Describe the change
Edit transitions for IBFT2.0:
- update block period
- add block reward
<!-- A clear and concise description of what this PR changes in the documentation. -->

## Issue fixed
Fixes #843 
<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing
https://hyperledger-besu--882.org.readthedocs.build/en/882/HowTo/Configure/Consensus-Protocols/IBFT/
<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 16:58:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/881" class=".btn">#881</a>
            </td>
            <td>
                <b>
                    Updated link to point to GoQuorum genesis file
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I think I have updated the link correctly which is an improvement. However, if you use [this genesis file](https://docs.goquorum.consensys.net/en/stable/HowTo/Configure/Consensus-Protocols/IBFT/#genesis-file) as your basis, then I think further changes are be required in order to correctly add a besu node into a goquorum network. For example, the documentation just says 
> update the consensus protocol specified in the config property from istanbul to ibft.

However, I'm not sure all the properties within `istanbul` are relevant to `ibft` in besu (although perhaps they can be safely ignored when you're not a validator). 
Also, `"isQuorum": true` yields an error in besu, so it either wants removing or changing to false, which would be worth documenting.

```
      "istanbul": {
        "epoch": 30000,
        "policy": 0,
        "ceil2Nby3Block": 0
      },
      "txnSizeLimit": 64,
      "maxCodeSize": 0,
      "isQuorum": true
```

Tagging @jframe who may be able to help clarify.

## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [ ] you fixed all the issues raised by the tests, if any.
- [ ] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [x] Doc content
- [ ] Doc pages organisation

## Testing

Link on https://besu.hyperledger.org/en/stable/HowTo/Configure/Consensus-Protocols/QuorumIBFT/ should point to https://docs.goquorum.consensys.net/en/stable/HowTo/Configure/Consensus-Protocols/IBFT/#genesis-file
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 11:23:45 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu-docs/pull/880" class=".btn">#880</a>
            </td>
            <td>
                <b>
                    improve deploying contracts tutorial
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## Pull request checklist

Use the following list to make sure your PR fits the Besu doc quality standard.

### Before creating the pull request

Make sure that:

- [x] [all commits in this PR are signed off for the DCO](https://wiki.hyperledger.org/display/BESU/DCO).
- [x] you read the [contribution guidelines](https://wiki.hyperledger.org/display/BESU/Contributing+to+documentation).
- [x] you have [tested your changes locally](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewTheDocumentation) before submitting them to the community for review.

### After creating your pull request and tests finished

Make sure that:

- [ ] you fixed all the issues raised by the tests, if any.
- [ ] you verified the rendering of your changes on [ReadTheDocs.org PR preview](https://wiki.hyperledger.org/display/BESU/MkDocs+And+Markdown+Guide#MkDocsAndMarkdownGuide-PreviewwithReadTheDocs)
  and updated the testing link (see [Testing](#testing)).

## Describe the change

<!-- A clear and concise description of what this PR changes in the documentation. -->

Test and improve Deploying Contracts tutorial to add more detail based on user feedback.

## Issue fixed

<!-- Except for minor changes (typos, commas) it's required to have a Github issue linked to your
pull request.

Use the following to make Github close the issue automatically when merging the PR:
fixes #{your issue number}
If multiple issues are involved, use one line for each issue.

If you don't want to close the issue, use:
see #{your issue number} -->

fixes #760 

## Impacted parts <!-- check as many boxes as needed -->

### For content changes

- [ ] Doc content
- [ ] Doc pages organisation

### For tools changes

- [ ] CircleCI workflow
- [ ] Build and QA tools (lint, vale,…)
- [ ] MkDocs templates
- [ ] MkDocs configuration
- [ ] Python dependencies
- [ ] Node dependencies and JavaScript
- [ ] ReadTheDocs configuration
- [ ] GitHub integration

## Testing

<!-- Steps to follow to review and test your changes.
Add links to preview the pages changes here.
Link format is https://hyperledger-besu--{your PR number}.org.readthedocs.build/en/{your PR number}/
Where {your PR number} must be replaced by the number of this PR, for instance 123
-->

## Screenshots / recording

<!-- If it helps understanding your change,
don't hesitate to link an annotated screenshot or a small demo video. -->

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 08:13:24 +0000 UTC
    </div>
</div>

