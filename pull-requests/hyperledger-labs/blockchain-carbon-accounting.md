---
layout: default
title: blockchain-carbon-accounting
parent: Hyperledger Labs
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger-labs/blockchain-carbon-accounting
---

# blockchain-carbon-accounting <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger-labs/blockchain-carbon-accounting){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/397" class=".btn">#397</a>
            </td>
            <td>
                <b>
                    feat(data loader): add script to load emissions data and identifiers into OrbitDB
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR adds a directory that contains a script to load emissions factors and identifiers from different XLSX and CSV files into OrbitDB. This is meant to be a drop-in replacement for the existing `egrid-data-loader.js` script. This is the first step towards migrating all the emissions records from CouchDB to OrbitDB. The following changes have been made:
- Imports data into OrbitDB instead of invoking the chaincode to add an emission factor/identifier
- Uses the IPFS HTTP API, so it can be connected to a public IPFS node that we run remotely
- Upgraded the code to TypeScript (some type definitions and interfaces will be added in later as the refactoring is done)
- Added in progress bars to improve the UX

Here are some instructions on how to test the data loader:
- Install `go-ipfs` on your computer [using these instructions](https://github.com/ipfs/go-ipfs#install-prebuilt-binaries)
- Initialize IPFS's config files by running `ipfs init`
- Start up an IPFS daemon with the following command
`ipfs daemon --enable-pubsub-experiment --writable`
- Ensure that you have Node >= v16 installed on your computer (the project will not work on a lower version of Node)
- Install `yarn` if you haven't already with `npm install -g yarn`
- Install `ts-node` globally with `npm install -g ts-node`
- Install the project's dependencies with
```sh
cd utility-emissions-channel/docker-compose-setup/data
yarn
```
- Download all the data files using the [instructions in the README](https://github.com/hyperledger-labs/blockchain-carbon-accounting/tree/main/utility-emissions-channel#seeding-the-fabric-database)
- For loading the files, simply replace `node egrid-data-loader.js` with `ts-node src/dataLoader.ts`. The other arguments can remain the same.

After loading the data, you may want to view all the inserted data. This can be done by running `ts-node src/getData.ts`.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-01-25 16:57:07 +0000 UTC
    </div>
</div>

