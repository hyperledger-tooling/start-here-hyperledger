---
layout: default
title: hyperledger-community-management-tools
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/hyperledger-community-management-tools
---

# hyperledger-community-management-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/hyperledger-community-management-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/hyperledger-community-management-tools/pull/81" class=".btn">#81</a>
            </td>
            <td>
                <b>
                    Add CodeQL workflow for GitHub code scanning
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Hi `hyperledger-labs/hyperledger-community-management-tools`!

This is a one-off automatically generated pull request from LGTM.com :robot:. You might have heard that we’ve integrated LGTM’s underlying CodeQL analysis engine natively into GitHub. The result is [**GitHub code scanning**](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/about-code-scanning)!

With LGTM fully integrated into code scanning, we are focused on improving CodeQL within the native GitHub code scanning experience. In order to take advantage of current and future improvements to our analysis capabilities, we suggest you enable code scanning on your repository. Please take a look at our [blog post for more information](https://github.blog/2022-08-15-the-next-step-for-lgtm-com-github-code-scanning/).

This pull request enables code scanning by adding an auto-generated [`codeql.yml` workflow file for GitHub Actions](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/setting-up-code-scanning-for-a-repository#setting-up-code-scanning-manually) to your repository — take a look! We tested it before opening this pull request, so all should be working :heavy_check_mark:. In fact, you might already have seen some alerts appear on this pull request!

Where needed and if possible, we’ve adjusted the configuration to the needs of your particular repository. But of course, you should feel free to tweak it further! Check [this page](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#editing-a-code-scanning-workflow) for detailed documentation.

Questions? Check out the FAQ below!

### FAQ
<details>
<summary>Click here to expand the FAQ section</summary>

#### How often will the code scanning analysis run?
By default, code scanning will trigger a scan with the CodeQL engine on the following events:
* On every pull request — to flag up potential security problems for you to investigate before merging a PR.
* On every push to your default branch and other protected branches — this keeps the analysis results on your repository’s *Security* tab up to date.
* Once a week at a fixed time — to make sure you benefit from the latest updated security analysis even when no code was committed or PRs were opened.

#### What will this cost?
Nothing! The CodeQL engine will run inside GitHub Actions, making use of your [unlimited free compute minutes for public repositories](https://docs.github.com/en/actions/learn-github-actions/usage-limits-billing-and-administration#about-billing-for-github-actions).

#### What types of problems does CodeQL find?
The CodeQL engine that powers GitHub code scanning is the exact same engine that powers LGTM.com. The exact set of rules has been tweaked slightly, but you should see almost exactly the same types of alerts as you were used to on LGTM.com: we’ve enabled the [`security-and-quality` query suite](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/configuring-code-scanning#using-queries-in-ql-packs) for you.

#### How do I upgrade my CodeQL engine?
No need! New versions of the CodeQL analysis are constantly deployed on GitHub.com; your repository will automatically benefit from the most recently released version.

#### The analysis doesn’t seem to be working
If you get an error in GitHub Actions that indicates that CodeQL wasn’t able to analyze your code, please [follow the instructions here](https://docs.github.com/en/code-security/code-scanning/automatically-scanning-your-code-for-vulnerabilities-and-errors/troubleshooting-the-codeql-workflow) to debug the analysis.

#### How do I disable LGTM.com?
If you have LGTM’s automatic pull request analysis enabled, then you can [follow these steps to disable the LGTM pull request analysis](https://lgtm.com/help/lgtm/managing-automated-code-review#disabling-pr-integration). You don’t actually need to remove your repository from LGTM.com; it will automatically be removed in the next few months as part of the deprecation of LGTM.com ([more info here](https://github.blog/2022-08-15-the-next-step-for-lgtm-com-github-code-scanning/)).

#### Which source code hosting platforms does code scanning support?
GitHub code scanning is deeply integrated within GitHub itself. If you’d like to scan source code that is hosted elsewhere, we suggest that you create a mirror of that code on GitHub.

#### How do I know this PR is legitimate?
This PR is filed by the official LGTM.com GitHub App, in line with the [deprecation timeline that was announced on the official GitHub Blog](https://github.blog/2022-08-15-the-next-step-for-lgtm-com-github-code-scanning/). The proposed GitHub Action workflow uses the [official open source GitHub CodeQL Action](https://github.com/github/codeql-action/). If you have any other questions or concerns, please join the discussion [here](https://github.com/orgs/community/discussions/29534) in the official GitHub community!

#### I have another question / how do I get in touch?
Please join the discussion [here](https://github.com/orgs/community/discussions/29534) to ask further questions and send us suggestions!

</details> 

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-11-10 14:33:03 +0000 UTC
    </div>
</div>

