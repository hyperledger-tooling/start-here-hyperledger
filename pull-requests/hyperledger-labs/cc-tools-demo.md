---
layout: default
title: cc-tools-demo
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/cc-tools-demo
---

# cc-tools-demo <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/cc-tools-demo){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools-demo/pull/53" class=".btn">#53</a>
            </td>
            <td>
                <b>
                    Remove binaries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Removed fabric binaries
- Added script to verify if binaries are already downloaded
    - If it's not, download it
    - If missing one or more binaries, download it 

I chose to always download and remove the `install-fabric.sh` script instead of having it hardcoded, since I didn't know if it was correct to do that
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-22 14:29:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools-demo/pull/52" class=".btn">#52</a>
            </td>
            <td>
                <b>
                    Automatic collection generation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Create script in the chaincode `main` package to generate the `collections.json` file
  - The script is only executed if the `-g` flag is used
  - The `--orgs/-o` can be used to pass a list of organizations to be considered when generating the policy
  - The scripts adds the collections according to asset types with readers and the number of orgs being deployed
- Removed collection files (and added it to gitignore)
- Added collection generation to startDev and upgradeCC scripts
- Created a `generateCollection.sh` script just to generate the collections.json file
  - The script can take multiple `-o` argumets to determinate the orgs to be considered on the generation
- Updated the `generateTar.sh` script to generate the collections.json file
   - The script can take multiple `-o` argumets to determinate the orgs to be considered on the generation 
- Unrelated to the collections, this PR also features a small fix to the `generateTar.sh` script so it includes hidden files (such as `.env`) when compressing the go ccapi
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-09-20 18:08:19 +0000 UTC
    </div>
</div>

