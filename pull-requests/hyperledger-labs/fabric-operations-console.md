---
layout: default
title: fabric-operations-console
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/fabric-operations-console
---

# fabric-operations-console <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/fabric-operations-console){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/421" class=".btn">#421</a>
            </td>
            <td>
                <b>
                    reconnect to couchdb _changes api periodically ++
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
- lets athena safely periodically reconnect to the couchdb _changes api
   - it will now reconnect daily
- migration will now reconnect the _changes api when migration has started to ensure the api is alive and well
- ties into more request events to let the couchdb _changes api reconnect when things go wrong
  - previously only the events `error` and `end` where used to reconnect, we now use `error`, `end`, `timeout`, `abort`, `close`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-22 17:53:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/420" class=".btn">#420</a>
            </td>
            <td>
                <b>
                    tweak migration content text based on feedback
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Documentation update

#### Description
- Improved migration content text.
- also has npm audit changes (using better-npm-audit for athena)


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-17 17:22:47 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/fabric-operations-console/pull/419" class=".btn">#419</a>
            </td>
            <td>
                <b>
                    Prevent migration spin
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                #### Type of change

<!--- What type of change? Pick one option and delete the others. -->

- Bug fix

#### Description
Prevent migration status checking/monitoring from spinner in place forever.


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-03-15 20:50:04 +0000 UTC
    </div>
</div>

