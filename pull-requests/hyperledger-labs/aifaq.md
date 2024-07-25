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
                PR <a href="https://github.com/hyperledger-labs/aifaq/pull/30" class=".btn">#30</a>
            </td>
            <td>
                <b>
                    [ENH] : Containerize Frontend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Closes #26
**Changes proposed in this pull request:** 
-  Adds two Dockerfiles for development and production environments, and includes the installation of the sharp npm package for image optimization.

- Having separate Dockerfiles for development and production ensures that each environment has the appropriate configurations and dependencies.

- Using sharp for image optimization improves performance and quality of images used within the application.

- Ensuring sharp is installed in standalone mode is crucial for its correct operation in Docker containers.

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-07-24 17:44:06 +0000 UTC
    </div>
</div>

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

