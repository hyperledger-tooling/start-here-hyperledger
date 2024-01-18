---
layout: default
title: fabric-samples
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/fabric-samples
---

# fabric-samples <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/fabric-samples){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1173" class=".btn">#1173</a>
            </td>
            <td>
                <b>
                    	new file:   LandContract/application-typescript/package.json
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                	new file:   LandContract/application-typescript/src/Admin.js
	new file:   LandContract/application-typescript/src/app.ts
	new file:   LandContract/application-typescript/src/registerEnrollUser.js
	new file:   LandContract/application-typescript/src/utils/AppUtil.ts
	new file:   LandContract/application-typescript/src/utils/CAUtil.ts
	new file:   LandContract/application-typescript/tsconfig.json
	new file:   LandContract/application-typescript/tslint.json
	new file:   chaincode-typescript/Dockerfile
	new file:   chaincode-typescript/dist/Contract/landAsset.d.ts
	new file:   chaincode-typescript/dist/Contract/landAsset.js
	new file:   chaincode-typescript/dist/Contract/landAsset.js.map
	new file:   chaincode-typescript/dist/Contract/landTransaction.d.ts
	new file:   chaincode-typescript/dist/Contract/landTransaction.js
	new file:   chaincode-typescript/dist/Contract/landTransaction.js.map
	new file:   chaincode-typescript/dist/asset.d.ts
	new file:   chaincode-typescript/dist/asset.js
	new file:   chaincode-typescript/dist/asset.js.map
	new file:   chaincode-typescript/dist/assetTransfer.d.ts
	new file:   chaincode-typescript/dist/assetTransfer.js
	new file:   chaincode-typescript/dist/assetTransfer.js.map
	new file:   chaincode-typescript/dist/index.d.ts
	new file:   chaincode-typescript/dist/index.js
	new file:   chaincode-typescript/dist/index.js.map
	new file:   chaincode-typescript/docker/docker-entrypoint.sh
	new file:   chaincode-typescript/npm-shrinkwrap.json
	new file:   chaincode-typescript/package.json
	new file:   chaincode-typescript/src/Contract/Admin.js
	new file:   chaincode-typescript/src/Contract/landAsset.ts
	new file:   chaincode-typescript/src/Contract/landTransaction.ts
	new file:   chaincode-typescript/src/Contract/registerEnrollUser.js
	new file:   chaincode-typescript/src/Contract/userRequest.ts
	new file:   chaincode-typescript/src/Contract/wallet/admin.id
	new file:   chaincode-typescript/src/Contract/wallet/user123.id
	new file:   chaincode-typescript/src/asset.ts
	new file:   chaincode-typescript/src/assetTransfer.ts
	new file:   chaincode-typescript/src/index.ts
	new file:   chaincode-typescript/tsconfig.json
	new file:   chaincode-typescript/tslint.json
	modified:   test-network/compose/compose-ca.yaml
	modified:   test-network/compose/compose-test-net.yaml
	modified:   test-network/compose/docker/docker-compose-bft-test-net.yaml
	modified:   test-network/compose/docker/docker-compose-test-net.yaml
	modified:   test-network/configtx/configtx.yaml
	modified:   test-network/network.sh
	modified:   test-network/organizations/ccp-generate.sh
	modified:   test-network/organizations/cryptogen/crypto-config-org2.yaml
	new file:   test-network/organizations/cryptogen/crypto-config-org3.yaml
	new file:   test-network/organizations/cryptogen/crypto-config-org4.yaml
	modified:   test-network/organizations/fabric-ca/registerEnroll.sh
	new file:   test-network_org4.zip
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-17 11:31:14 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/fabric-samples/pull/1169" class=".btn">#1169</a>
            </td>
            <td>
                <b>
                    Fix certPath in assetTransfer.go
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Following the latest tutorial, the current version of network.sh does not generate `cert.pem` as filename under `msp/signcerts` but instead created `User1@org1.example.com-cert.pem`. I have edited the application file to reflect such difference.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-01-15 01:32:59 +0000 UTC
    </div>
</div>

