---
layout: default
title: pdo-contracts
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/pdo-contracts
---

# pdo-contracts <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/pdo-contracts){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/pdo-contracts/pull/29" class=".btn">#29</a>
            </td>
            <td>
                <b>
                    Jupyter upgrades for exchange and support functions
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">documentation</span>
            </td>
            <td>
                Major update of jupyter notebooks:

 *  Update for the new jupyter functions in the python module.  Issuer and token issuer should be fully functional. Other notebooks are work in progress.
    
* New notebooks for wallets and orders. Do not expect these to work at present. More than placeholders but less than fully functional.
    
* Split the exchange launch page into some additional documentation files and the operational links to the factories.    
  
* Add Jupyter files for the root notebook directory. Replace the empty index file with one that contains somewhat useful content. Move a lot of the getting started content into its own file. This should be replaced later by notebooks that allow for managing configurations.

Major update for the python functions that support Jupyter notebooks:

* Create a new jupyter module that can be used for multiple contract families; this will include context handling and ipython magic functions.
    
* Update the context creation for exchange family templates; this should make context creation a little more configurable
    
* Split out the the reusable components of the exchange jupyter python modue into a separate module. This is both functions that should be exposed to a jupyter notebook and support functions that are note exposed.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-03-06 23:54:25 +0000 UTC
    </div>
</div>

