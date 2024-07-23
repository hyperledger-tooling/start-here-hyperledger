---
layout: default
title: aifaq
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/aifaq
---

# aifaq <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/aifaq){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Issue #20: Connect API to the frontend of the application
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description
This PR addresses Issue #20 . Users can now interact directly with the frontend, receiving their typed messages in the chatbox.

Due to hardware limitations, testing the connection between the frontend and backend hasn't been performed. The relevant code is written but currently commented out.

### Current Progress
The image below demonstrates the current progress
<img width="1499" alt="Screenshot 2024-07-23 at 9 32 51 PM" src="https://github.com/user-attachments/assets/3606e96f-202a-4c71-9244-1d6aecf10ed9">
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-21 14:34:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/28" class=".btn">#28</a>
            </td>
            <td>
                <b>
                    Configure formatting and continuous integration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">enhancement</span>
            </td>
            <td>
                This PR aims to improve the general repository structure with respect to CI workflows, formatting and linting and standard repository templates.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-21 07:10:35 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/27" class=".btn">#27</a>
            </td>
            <td>
                <b>
                    Automated the dowloading of ReadFromDocs procedure and Dockerized the current backend.
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Key changes:
- Added the file fetchAndOrganizeData.py. This file collects data from all the links provided in config.yaml. The collected data is then organized in a dedicated folder containing all the HTML files gathered.
- In ingest.py, we've added some debugging code to print the total number of chunks. Additionally, the creation of the chromadb folder is now automated.
- I've also included a Dockerfile and added usage commands for both Docker and non-Docker environments.

@gcapuzzi @swaptr Can you please review this?

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-20 19:07:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/24" class=".btn">#24</a>
            </td>
            <td>
                <b>
                    [ENH] : Collapsed Sidebar Feature for all Screen 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--- Until this PR is ready for review, you can include [WIP] in the title, or create a draft PR. -->


<!---
Below is a suggested pull request template. Feel free to add more details you feel are relevant/necessary.

For more info on the Hyperledger PR process and other contributing guidelines, see .
-->

<!-- 
Please indicate after the # which issue you're closing with this PR, if applicable.
If the PR closes multiple issues, include "closes" before each one is listed.
You can also link to other issues if necessary, e.g. "See also #1234".

https://help.github.com/articles/closing-issues-using-keywords
-->
- Closes #25 

<!-- 
You can link a pull request to an issue by using a supported keyword in the pull request's description or in a commit message. The pull request must be on the default branch.
EX: 
close
closes
closed
fix
fixes
fixed
resolve
resolves
resolved 

-->

<!-- 
Please give a brief overview of what has changed or been added in the PR.
This can include anything specific the maintainers should be looking for when they review the PR.
-->
Changes proposed in this pull request:

- The sidebar is collapsed by default in this pull request for all screen sizes (big, medium, and tiny).
- For a medium and small screen, it is collapsed; for a large screen, it is open. 


<!-- To be checked off by reviewers -->
## Checklist
_This section is for the PR reviewer_

- [x] PR has an interpretable title with a prefix (`[ENH]`, `[FIX]`, `[REF]`, `[TST]`, `[CI]`, `[MNT]`, `[INF]`, `[MODEL]`, `[DOC]`) (see our [Contributing Guidelines](/docs/pull_request_guidelines.md) for more info)

- [x] PR links to GitHub issue with mention `Closes #XXXX`


https://github.com/user-attachments/assets/46846a0a-b654-4dd7-95db-6d89ac83ded9



**Please advise if any modifications are required.**
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-18 17:15:32 +0000 UTC
    </div>
</div>

