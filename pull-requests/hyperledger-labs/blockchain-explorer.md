---
layout: default
title: blockchain-explorer
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-explorer
---

# blockchain-explorer <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-explorer){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-explorer/pull/463" class=".btn">#463</a>
            </td>
            <td>
                <b>
                    fixed packages vulnerability from backend
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <!--  Thanks for sending a pull request! 
-->


#### What this PR does / why we need it: update the vulnerable packages from backend explorer

#### Which issue(s) this PR fixes: packages vulnerabilities from backend application
<!--
*Automatically closes linked issue when PR is merged.
Usage: `Fixes #<issue number>`, or `Fixes (paste link of issue)`.
_If PR is about `failing-tests`, please post the related issues/tests in a comment and do not use `Fixes`_*
-->
Fixes #458 

#### Special notes for your reviewer:

#### Does this PR introduce a user-facing change: None
<!--
If no, just write "NONE" in the release-note block below.
If yes, a release note is required:
Enter your extended release note in the block below. If the PR requires additional action from users switching to the new release, include the string "action required".

-->
```release-note

```

#### Additional documentation, usage docs, etc.:
1. "ejs":"^2.5.6" ----> "^3.1.9", [critical]
2. "grpc": "^1.20.3" ----> "^1.24.11"
3. "jsonwebtoken":"^8.5.0", ----> "^9.0.2" [moderate] 

NOTE: jsonwebtoken's insecure implementation of key retrieval function could lead to Forgeable Public/Private Tokens from RSA to HMAC 
ref url: https://github.com/advisories/GHSA-hjrf-2m68-5959
jsonwebtoken vulnerable to signature validation bypass due to insecure default algorithm in jwt.verify() 
ref url: https://github.com/advisories/GHSA-qwph-4952-7xr6

4. "multer": "^1.3.0" ----> "^1.4.5-lts.1", ---> dicer[Severity: high], 
       busboy(Depends on vulnerable versions of dicer),
       multer(Depends on vulnerable versions of busboy)
 
NOTE- busboy---> dependency package of multer
      dicer----> dependency package of busboy

5. "passport": "^0.4.0", ----> "^0.6.0", ----> Severity: moderate

NOTE: Passport vulnerable to session regeneration when a users logs in or out - https://github.com/advisories/GHSA-v923-w3x8-wh69

6. "sequelize": "^6.12.2", ------> "^6.33.0", 

7. "mocha": "^8.2.1", ----> "^10.2.0",  ----> mocha  v5.1.0 - v9.2.1 Depends on vulnerable versions of "minimatch" and "nanoid"
 [minimatch <3.0.5 Severity: high]
 [nanoid  3.0.0 - 3.1.30 Severity: moderate]
<!--
This section can be blank if this pull request does not require a release note.

When adding links which point to resources within git repositories, like
supporting documentation, please reference a specific commit and avoid
linking directly to the master branch. This ensures that links reference a
specific point in time, rather than a document that may change over time.


-->
```docs

```

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-18 11:28:56 +0000 UTC
    </div>
</div>

