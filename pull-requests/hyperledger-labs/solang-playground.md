---
layout: default
title: solang-playground
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/solang-playground
---

# solang-playground <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/solang-playground){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/solang-playground/pull/11" class=".btn">#11</a>
            </td>
            <td>
                <b>
                    Implement Backend Service and Compile Button 
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ### Description
This pull request adds the Solang Playground backend service and updates the frontend with a "Compile" button that compiles the code with Solang and downloads the result contract with a single click.

### Changes
- **New Rust Crates in `crates/`**:
    - `backend`: Actix Web server for the frontend.
    - `generate_bindings`: Generates TypeScript bindings for API endpoints.
- **Frontend Update**:
    - Added a "Compile" button and implemented a TypeScript function to interact with the backend.
- **Docker Setup**:
    - Created a Dockerfile and set up the Docker image to use `sysbox` for Docker-in-Docker functionality.
- **CI Workflow**:
    - Added a CI workflow to build the project, run the Docker image, and test compiling a sample contract.
- **README Update**:
    - Updated the README file with the project's progress.
### Testing
- Added two TypeScript tests to ensure the frontend is served and can compile a sample contract.
- These tests are integrated into the CI as end-to-end (e2e) tests.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-05-23 14:52:53 +0000 UTC
    </div>
</div>

