---
layout: default
title: firefly-dataexchange-https
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-dataexchange-https
---

# firefly-dataexchange-https <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-dataexchange-https){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-dataexchange-https/pull/71" class=".btn">#71</a>
            </td>
            <td>
                <b>
                    Added delete blobs API for Issue 36
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Shweta Melton <shweta@shweta_s@hotmail.com>

- Added delete blobs API that would delete the blob file and the blob metadata file
- If any of the files for the blob do not exist, it will clean up whatever exists. 
- On success, returns Blob metadata if available or empty response (if the metadata file did not exist at the time of deletion)
- Added unit tests
- Updated Swagger documentation
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-09-17 02:40:13 +0000 UTC
    </div>
</div>

