---
layout: default
title: aries-endorser-service
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/aries-endorser-service
---

# aries-endorser-service <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/aries-endorser-service){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/37" class=".btn">#37</a>
            </td>
            <td>
                <b>
                    Enhancement: Introduce Support for Uploading CSV-Based Configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This pull request resolves #38

This enhancement adds the capability to configure your application using CSV files. The configuration is structured around the following classes:

- AllowedPublicDid:
  - Used for managing the publish_did file.
  - Defines the registered_did attribute, which is a required string and serves as the primary key.
    
- AllowedSchema:
  - Intended for handling schema files.
  - Includes attributes like author_did, schema_name, and version, all of which are mandatory and cannot be null.

- AllowedCredentialDefinition:
  - Specifically designed for the credential_definition file.
  - Contains attributes such as issuer_did, author_did, schema_name, version, tag, rev_reg_def, and rev_reg_entry. All of these attributes are required and must have non-null values.

This enhancement enables you to upload CSV files associated with each
of these classes, using either the POST or PUT methods. The choice
between POST and PUT dictates how the uploaded data interacts with the
existing configuration:

POST: This method will replace the current configuration with the data from the uploaded CSV file.

PUT: In contrast, the PUT method appends the data from the CSV file to the existing configuration, preserving the current state.

This feature enhances the flexibility and ease of configuring your application by allowing you to manage your configuration using CSV files effortlessly.

![2023-10-16_15-22-15](https://github.com/hyperledger/aries-endorser-service/assets/34443260/bbc58cf1-6ebb-412d-812a-6d50f8cdc4ce)

These enhancements are designed to make your application's configuration management more user-friendly and efficient.


An example csv for the scheme file would be

```csv
author_did,schema_name,version
"3fa85f64-5717-4562-b3fc-2c963f66afa6","myschema","1.0"
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-16 22:30:10 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/aries-endorser-service/pull/36" class=".btn">#36</a>
            </td>
            <td>
                <b>
                    Update maintainers list
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Suggesting the following change (additions) to the maintainers list:

- @esune  (myself) as I have been designing the enhancements to the endorser service required to automate some/all of the endorsement operations with fine-grained control
- @Gavinok as he has been the hands-on implementer of the above changes (see #34)
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-10-13 18:18:51 +0000 UTC
    </div>
</div>

