---
layout: default
title: cc-tools
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/cc-tools
---

# cc-tools <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/cc-tools){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/cc-tools/pull/44" class=".btn">#44</a>
            </td>
            <td>
                <b>
                    create package query-search
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This package provides a way to query a database, possibly using a CouchDB-like interface and defines several types, methods, and functions for querying. It facilitates the creation of queries without having to write queries in a raw form.

**Features**
- The Config struct contains the settings used for querying
- These settings include RemoveTags (a list of tags to be removed from the results)
- AssetName (the name of the asset being queried) used for create query
- PageSize (the number of results per page)
- BookMark (the bookmark for pagination)
- Resolve (a list of relations to be resolved)
- Sort (a list of fields to sort by)
- IndexDoc (a document containing the index design and name)
- NoRemoveTagsTransaction (a boolean indicating whether to remove tags during the transaction),
- CallBack (a function to be called after the query is executed)
- Date handling for searches
- Wraper to add fields to the search
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-05 17:00:17 +0000 UTC
    </div>
</div>

