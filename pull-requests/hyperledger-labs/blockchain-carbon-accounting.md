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
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/371" class=".btn">#371</a>
            </td>
            <td>
                <b>
                    fix documentation on European emissions intensity data
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-23 17:48:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/368" class=".btn">#368</a>
            </td>
            <td>
                <b>
                    update web socket client app documentation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                <nil>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 18:48:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/367" class=".btn">#367</a>
            </td>
            <td>
                <b>
                    Configure Renovate
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                [![WhiteSource Renovate](https://app.renovatebot.com/images/banner.svg)](https://renovatebot.com)

Welcome to [Renovate](https://togithub.com/renovatebot/renovate)! This is an onboarding PR to help you understand and configure settings before regular Pull Requests begin.

🚦 To activate Renovate, merge this Pull Request. To disable Renovate, simply close this Pull Request unmerged.



---
### Detected Package Files

 * `utility-emissions-channel/docker-compose-setup/docker/application/docker-compose.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/docker-compose-blockchain-explorer.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/docker-compose-ca.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/docker-compose-carbonAccounting.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/docker-compose-couch.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-one/docker-compose-ca.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-one/docker-compose-carbonAccounting.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-one/docker-compose-chaincode.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-one/docker-compose-couch.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-two/docker-compose-ca.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-two/docker-compose-carbonAccounting.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-two/docker-compose-chaincode.yaml` (docker-compose)
 * `utility-emissions-channel/docker-compose-setup/docker/nodes/node-two/docker-compose-couch.yaml` (docker-compose)
 * `multi-cloud-deployment/chaincode/Dockerfile` (dockerfile)
 * `multi-cloud-deployment/deploy-aws/chaincode/Dockerfile` (dockerfile)
 * `secure-identities/vault-identity/Dockerfile` (dockerfile)
 * `secure-identities/ws-identity/Dockerfile` (dockerfile)
 * `secure-identities/ws-wallet/Dockerfile` (dockerfile)
 * `utility-emissions-channel/aws-kubernetes/Dockerfile` (dockerfile)
 * `utility-emissions-channel/chaincode/datalock/Dockerfile` (dockerfile)
 * `utility-emissions-channel/chaincode/node/Dockerfile` (dockerfile)
 * `utility-emissions-channel/chaincode/typescript/Dockerfile` (dockerfile)
 * `utility-emissions-channel/typescript_app/Dockerfile` (dockerfile)
 * `.github/workflows/ci.yml` (github-actions)
 * `.github/workflows/test-report.yml` (github-actions)
 * `multi-cloud-deployment/chaincode/go.mod` (gomod)
 * `multi-cloud-deployment/deploy-aws/chaincode/go.mod` (gomod)
 * `utility-emissions-channel/chaincode/datalock/go.mod` (gomod)
 * `utility-emissions-channel/chaincode/go/go.mod` (gomod)
 * `net-emissions-token-network/interface/package.json` (npm)
 * `net-emissions-token-network/interface/packages/contracts/package.json` (npm)
 * `net-emissions-token-network/interface/packages/react-app/package.json` (npm)
 * `net-emissions-token-network/interface/packages/subgraph/package.json` (npm)
 * `net-emissions-token-network/package.json` (npm)
 * `open-offsets-directory/node-server/package.json` (npm)
 * `open-offsets-directory/react/package.json` (npm)
 * `secure-identities/identity-ui/package.json` (npm)
 * `secure-identities/vault-identity/package.json` (npm)
 * `secure-identities/ws-identity-client/package.json` (npm)
 * `secure-identities/ws-identity/package.json` (npm)
 * `secure-identities/ws-wallet/package.json` (npm)
 * `utility-emissions-channel/chaincode/node/package.json` (npm)
 * `utility-emissions-channel/chaincode/typescript/package.json` (npm)
 * `utility-emissions-channel/docker-compose-setup/package.json` (npm)
 * `utility-emissions-channel/typescript_app/package.json` (npm)

### Configuration Summary

Based on the default config's presets, Renovate will:

  - Start dependency updates only once this onboarding PR is merged
  - Enable Renovate Dependency Dashboard creation
  - If semantic commits detected, use semantic commit type <code>fix</code> for dependencies and <code>chore</code> for all others
  - Ignore `node_modules`, `bower_components`, `vendor` and various test/tests directories
  - Autodetect whether to pin dependencies or maintain ranges
  - Rate limit PR creation to a maximum of two per hour
  - Limit to maximum 20 open PRs at any time
  - Group known monorepo packages together
  - Use curated list of recommended non-monorepo package groupings
  - Fix some problems with very old Maven commons versions
  - Ignore spring cloud 1.x releases
  - Ignore http4s digest-based 1.x milestones
  - Use node versioning for @types/node
  - Limit concurrent requests to reduce load on Repology servers until we can fix this properly, see issue 10133

🔡 Would you like to change the way Renovate is upgrading your dependencies? Simply edit the `renovate.json` in this branch with your custom config and the list of Pull Requests in the "What to Expect" section below will be updated the next time Renovate runs.

---

### What to Expect

With your current configuration, Renovate will create 111 Pull Requests:

<details>
<summary>chore(deps): roll back dependency ws-identity to ^1.0.12</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ws-identity-rollback`
  - Merge into: `main`
  - Upgrade [ws-identity](https://togithub.com/brioux/blockchain-carbon-accounting) to `^1.0.12`


</details>

<details>
<summary>chore(deps): update dependency ansi-regex to 5.0.1 [security]</summary>

  - Branch name: `renovate/npm-ansi-regex-vulnerability`
  - Merge into: `main`
  - Upgrade ansi-regex to `5.0.1`


</details>

<details>
<summary>chore(deps): update dependency grpc to 1.24.4 [security]</summary>

  - Branch name: `renovate/npm-grpc-vulnerability`
  - Merge into: `main`
  - Upgrade grpc to `1.24.4`


</details>

<details>
<summary>chore(deps): update dependency immer to 9.0.6 [security]</summary>

  - Branch name: `renovate/npm-immer-vulnerability`
  - Merge into: `main`
  - Upgrade immer to `9.0.6`


</details>

<details>
<summary>chore(deps): update dependency jsrsasign to 10.2.0 [security]</summary>

  - Branch name: `renovate/npm-jsrsasign-vulnerability`
  - Merge into: `main`
  - Upgrade jsrsasign to `10.2.0`


</details>

<details>
<summary>chore(deps): update dependency nth-check to 2.0.1 [security]</summary>

  - Branch name: `renovate/npm-nth-check-vulnerability`
  - Merge into: `main`
  - Upgrade nth-check to `2.0.1`


</details>

<details>
<summary>chore(deps): update dependency underscore to 1.12.1 [security]</summary>

  - Branch name: `renovate/npm-underscore-vulnerability`
  - Merge into: `main`
  - Upgrade underscore to `1.12.1`


</details>

<details>
<summary>chore(deps): update dependency validator to 13.7.0 [security]</summary>

  - Branch name: `renovate/npm-validator-vulnerability`
  - Merge into: `main`
  - Upgrade validator to `13.7.0`


</details>

<details>
<summary>fix(deps): update dependency axios to v0.21.2 [security]</summary>

  - Branch name: `renovate/npm-axios-vulnerability`
  - Merge into: `main`
  - Upgrade [axios](https://togithub.com/axios/axios) to `0.21.2`


</details>

<details>
<summary>fix(deps): pin dependencies</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/apollo-graphql-packages`
  - Merge into: `main`
  - Pin [@apollo/react-hooks](https://togithub.com/apollographql/react-apollo) to `3.1.5`
  - Pin [apollo-boost](https://togithub.com/apollographql/apollo-client) to `0.4.9`
  - Pin [apollo-client](https://togithub.com/apollographql/apollo-client) to `2.6.10`
  - Pin [apollo-utilities](https://togithub.com/apollographql/apollo-client) to `1.3.4`


</details>

<details>
<summary>fix(deps): pin dependencies</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/pin-dependencies`
  - Merge into: `main`
  - Pin [@ethersproject/contracts](https://togithub.com/ethers-io/ethers.js) to `5.0.12`
  - Pin [@ethersproject/providers](https://togithub.com/ethers-io/ethers.js) to `5.0.24`
  - Pin [@material-ui/core](https://togithub.com/mui-org/material-ui) to `4.11.4`
  - Pin [@material-ui/lab](https://togithub.com/mui-org/material-ui) to `4.0.0-alpha.58`
  - Pin [@nomiclabs/hardhat-ethers](https://togithub.com/nomiclabs/hardhat) to `2.0.1`
  - Pin [@nomiclabs/hardhat-etherscan](https://togithub.com/nomiclabs/hardhat) to `2.1.0`
  - Pin [@nomiclabs/hardhat-waffle](https://togithub.com/nomiclabs/hardhat) to `2.0.1`
  - Pin [@openzeppelin/hardhat-upgrades](https://togithub.com/OpenZeppelin/openzeppelin-upgrades) to `1.6.0`
  - Pin [@testing-library/dom](https://togithub.com/testing-library/dom-testing-library) to `6.16.0`
  - Pin [@testing-library/jest-dom](https://togithub.com/testing-library/jest-dom) to `4.2.4`
  - Pin [@testing-library/jest-dom](https://togithub.com/testing-library/jest-dom) to `5.14.1`
  - Pin [@testing-library/react](https://togithub.com/testing-library/react-testing-library) to `9.5.0`
  - Pin [@testing-library/react](https://togithub.com/testing-library/react-testing-library) to `12.0.0`
  - Pin [@testing-library/user-event](https://togithub.com/testing-library/user-event) to `7.2.1`
  - Pin [@testing-library/user-event](https://togithub.com/testing-library/user-event) to `13.1.9`
  - Pin [@types/chai](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.2.19`
  - Pin [@types/chai](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.2.22`
  - Pin [@types/chai-as-promised](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `7.1.4`
  - Pin [@types/crypto-js](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.0.2`
  - Pin [@types/express](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.17.8`
  - Pin [@types/express](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.17.13`
  - Pin [@types/mocha](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `8.2.2`
  - Pin [@types/mocha](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `8.2.3`
  - Pin [@types/mocha](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `9.0.0`
  - Pin [@types/multer](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `1.4.7`
  - Pin [@types/node](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `14.17.20`
  - Pin [@types/node](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `16.11.10`
  - Pin [@types/react](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `16.14.5`
  - Pin [@types/rewire](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `2.5.28`
  - Pin [@types/ssh2-streams](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `0.1.9`
  - Pin [@types/swagger-ui-express](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.1.2`
  - Pin [@types/uuid](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `8.3.1`
  - Pin [@typescript-eslint/eslint-plugin](https://togithub.com/typescript-eslint/typescript-eslint) to `4.33.0`
  - Pin [@typescript-eslint/parser](https://togithub.com/typescript-eslint/typescript-eslint) to `4.33.0`
  - Pin [@walletconnect/web3-provider](https://togithub.com/walletconnect/walletconnect-monorepo) to `1.3.6`
  - Pin [axios](https://togithub.com/axios/axios) to `0.19.2`
  - Pin [axios](https://togithub.com/axios/axios) to `0.21.2`
  - Pin [body-parser](https://togithub.com/expressjs/body-parser) to `1.19.0`
  - Pin [bootstrap](https://togithub.com/twbs/bootstrap) to `5.1.3`
  - Pin [bootstrap](https://togithub.com/twbs/bootstrap) to `5.0.2`
  - Pin [bootstrap](https://togithub.com/twbs/bootstrap) to `4.6.0`
  - Pin [chai](https://togithub.com/chaijs/chai) to `4.3.4`
  - Pin [chai](https://togithub.com/chaijs/chai) to `4.2.0`
  - Pin [chai-as-promised](https://togithub.com/domenic/chai-as-promised) to `7.1.1`
  - Pin [chai-http](https://togithub.com/chaijs/chai-http) to `4.3.0`
  - Pin [chalk](https://togithub.com/chalk/chalk) to `4.1.0`
  - Pin [cors](https://togithub.com/expressjs/cors) to `2.8.5`
  - Pin [cross-env](https://togithub.com/kentcdodds/cross-env) to `7.0.3`
  - Pin [crypto-js](https://togithub.com/brix/crypto-js) to `4.1.1`
  - Pin [dotenv](https://togithub.com/motdotla/dotenv) to `10.0.0`
  - Pin [eslint](https://togithub.com/eslint/eslint) to `7.32.0`
  - Pin [eslint](https://togithub.com/eslint/eslint) to `4.19.1`
  - Pin [eslint](https://togithub.com/eslint/eslint) to `6.8.0`
  - Pin [eslint-config-prettier](https://togithub.com/prettier/eslint-config-prettier) to `8.3.0`
  - Pin [eslint-config-standard](https://togithub.com/standard/eslint-config-standard) to `16.0.3`
  - Pin [eslint-plugin-flowtype](https://togithub.com/gajus/eslint-plugin-flowtype) to `4.7.0`
  - Pin [eslint-plugin-import](https://togithub.com/import-js/eslint-plugin-import) to `2.25.3`
  - Pin [eslint-plugin-node](https://togithub.com/mysticatea/eslint-plugin-node) to `11.1.0`
  - Pin [eslint-plugin-prettier](https://togithub.com/prettier/eslint-plugin-prettier) to `4.0.0`
  - Pin [eslint-plugin-promise](https://togithub.com/xjamundx/eslint-plugin-promise) to `5.1.1`
  - Pin [eslint-plugin-react](https://togithub.com/yannickcr/eslint-plugin-react) to `7.27.1`
  - Pin [ethereum-waffle](https://togithub.com/EthWorks/Waffle) to `3.2.1`
  - Pin [ethers](https://togithub.com/ethers-io/ethers.js) to `5.1.0`
  - Pin [express](https://togithub.com/expressjs/express) to `4.17.1`
  - Pin [express-recaptcha](https://togithub.com/pdupavillon/express-recaptcha) to `5.0.2`
  - Pin [express-validator](https://togithub.com/express-validator/express-validator) to `6.13.0`
  - Pin [graphql](https://togithub.com/graphql/graphql-js) to `14.7.0`
  - Pin [hardhat](https://togithub.com/nomiclabs/hardhat) to `2.1.2`
  - Pin [hardhat-deploy](https://togithub.com/wighawag/hardhat-deploy) to `0.7.0-beta.57`
  - Pin [hardhat-deploy-ethers](https://togithub.com/wighawag/hardhat-deploy-ethers) to `0.3.0-beta.7`
  - Pin [hardhat-gas-reporter](https://togithub.com/cgewecke/hardhat-gas-reporter) to `1.0.4`
  - Pin [ipfs-http-client](https://togithub.com/ipfs/js-ipfs) to `45.0.0`
  - Pin [mocha](https://togithub.com/mochajs/mocha) to `9.1.3`
  - Pin [mocha](https://togithub.com/mochajs/mocha) to `8.4.0`
  - Pin [mocha](https://togithub.com/mochajs/mocha) to `5.2.0`
  - Pin [moment](https://togithub.com/moment/moment) to `2.29.1`
  - Pin [node-fetch](https://togithub.com/node-fetch/node-fetch) to `2.6.1`
  - Pin [nodemon](https://togithub.com/remy/nodemon) to `2.0.15`
  - Pin [nodemon](https://togithub.com/remy/nodemon) to `2.0.12`
  - Pin [nyc](https://togithub.com/istanbuljs/nyc) to `15.1.0`
  - Pin [nyc](https://togithub.com/istanbuljs/nyc) to `12.0.2`
  - Pin [pg](https://togithub.com/brianc/node-postgres) to `8.6.0`
  - Pin [pg-hstore](https://togithub.com/scarney81/pg-hstore) to `2.3.4`
  - Pin [prettier](https://togithub.com/prettier/prettier) to `2.5.0`
  - Pin [prettier](https://togithub.com/prettier/prettier) to `2.2.1`
  - Pin [prettier-plugin-solidity](https://togithub.com/prettier-solidity/prettier-plugin-solidity) to `1.0.0-beta.2`
  - Pin [react](https://togithub.com/facebook/react) to `16.14.0`
  - Pin [react](https://togithub.com/facebook/react) to `17.0.2`
  - Pin [react-bootstrap](https://togithub.com/react-bootstrap/react-bootstrap) to `2.0.2`
  - Pin [react-bootstrap](https://togithub.com/react-bootstrap/react-bootstrap) to `1.5.1`
  - Pin [react-copy-to-clipboard](https://togithub.com/nkbt/react-copy-to-clipboard) to `5.0.3`
  - Pin [react-datetime](https://togithub.com/arqex/react-datetime) to `3.0.4`
  - Pin [react-dom](https://togithub.com/facebook/react) to `16.14.0`
  - Pin [react-dom](https://togithub.com/facebook/react) to `17.0.2`
  - Pin [react-google-recaptcha-v3](https://togithub.com/t49tran/react-google-recaptcha-v3) to `1.9.4`
  - Pin [react-icons](https://togithub.com/react-icons/react-icons) to `4.2.0`
  - Pin [react-linkify](https://togithub.com/tasti/react-linkify) to `1.0.0-alpha`
  - Pin [react-native](https://togithub.com/facebook/react-native) to `0.64.2`
  - Pin [react-native-web](https://togithub.com/necolas/react-native-web) to `0.17.1`
  - Pin [react-router-dom](https://togithub.com/remix-run/react-router) to `5.3.0`
  - Pin [react-router-dom](https://togithub.com/remix-run/react-router) to `5.2.0`
  - Pin [react-scripts](https://togithub.com/facebook/create-react-app) to `3.4.4`
  - Pin [react-scripts](https://togithub.com/facebook/create-react-app) to `4.0.3`
  - Pin [sequelize](https://togithub.com/sequelize/sequelize) to `6.6.5`
  - Pin [sinon](https://togithub.com/sinonjs/sinon) to `10.0.0`
  - Pin [sinon](https://togithub.com/sinonjs/sinon) to `6.3.5`
  - Pin [sinon-chai](https://togithub.com/domenic/sinon-chai) to `3.7.0`
  - Pin [solidity-coverage](https://togithub.com/sc-forks/solidity-coverage) to `0.7.13`
  - Pin [styled-components](https://togithub.com/styled-components/styled-components) to `5.2.1`
  - Pin [ts-node](https://togithub.com/TypeStrong/ts-node) to `10.0.0`
  - Pin [ts-node](https://togithub.com/TypeStrong/ts-node) to `9.1.1`
  - Pin [ts-node](https://togithub.com/TypeStrong/ts-node) to `10.4.0`
  - Pin [typescript](https://togithub.com/Microsoft/TypeScript) to `4.4.4`
  - Pin [typescript](https://togithub.com/Microsoft/TypeScript) to `4.4.3`
  - Pin [typescript](https://togithub.com/Microsoft/TypeScript) to `4.5.2`
  - Pin [web3modal](https://togithub.com/web3modal/web3modal) to `1.9.3`
  - Pin [wouter](https://togithub.com/molefrog/wouter) to `2.7.4`
  - Pin [ws-wallet](https://togithub.com/brioux/blockchain-carbon-accounting) to `1.1.5`


</details>

<details>
<summary>fix(deps): update github.com/hyperledger/fabric-chaincode-go commit hash to 38d29fa</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/github.com-hyperledger-fabric-chaincode-go-digest`
  - Merge into: `main`
  - Upgrade [github.com/hyperledger/fabric-chaincode-go](https://togithub.com/hyperledger/fabric-chaincode-go) to `38d29fabecb9916a8a1ecbd0facb72f2ac32d016`


</details>

<details>
<summary>fix(deps): update github.com/hyperledger/fabric-protos-go commit hash</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/github.com-hyperledger-fabric-protos-go-digest`
  - Merge into: `main`
  - Upgrade [github.com/hyperledger/fabric-protos-go](https://togithub.com/hyperledger/fabric-protos-go) to `23d738fc3553a5c804ae65575e5bfcf3bdabe53a`


</details>

<details>
<summary>chore(deps): update actions/upload-artifact action to v2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/actions-upload-artifact-2.x`
  - Merge into: `main`
  - Upgrade [actions/upload-artifact](https://togithub.com/actions/upload-artifact) to `v2`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;nomiclabs/hardhat-ethers to v2.0.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/nomiclabs-hardhat-ethers-2.x`
  - Merge into: `main`
  - Upgrade [@nomiclabs/hardhat-ethers](https://togithub.com/nomiclabs/hardhat) to `2.0.2`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;nomiclabs/hardhat-etherscan to v2.1.8</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/nomiclabs-hardhat-etherscan-2.x`
  - Merge into: `main`
  - Upgrade [@nomiclabs/hardhat-etherscan](https://togithub.com/nomiclabs/hardhat) to `2.1.8`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;types/express to v4.17.13</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/express-4.x`
  - Merge into: `main`
  - Upgrade [@types/express](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.17.13`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;types/mocha to v8.2.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/mocha-8.x`
  - Merge into: `main`
  - Upgrade [@types/mocha](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `8.2.3`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;types/node to v14.17.34</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/node-14.x`
  - Merge into: `main`
  - Upgrade [@types/node](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `14.17.34`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;types/uuid to v8.3.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/uuid-8.x`
  - Merge into: `main`
  - Upgrade [@types/uuid](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `8.3.3`


</details>

<details>
<summary>chore(deps): update dependency hardhat-deploy-ethers to v0.3.0-beta.11</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hardhat-deploy-ethers-0.x`
  - Merge into: `main`
  - Upgrade [hardhat-deploy-ethers](https://togithub.com/wighawag/hardhat-deploy-ethers) to `0.3.0-beta.11`


</details>

<details>
<summary>chore(deps): update dependency nodemon to v2.0.15</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/nodemon-2.x`
  - Merge into: `main`
  - Upgrade [nodemon](https://togithub.com/remy/nodemon) to `2.0.15`


</details>

<details>
<summary>chore(deps): update dependency prettier-plugin-solidity to v1.0.0-beta.19</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/prettier-plugin-solidity-1.x`
  - Merge into: `main`
  - Upgrade [prettier-plugin-solidity](https://togithub.com/prettier-solidity/prettier-plugin-solidity) to `1.0.0-beta.19`


</details>

<details>
<summary>chore(deps): update dependency solidity-coverage to v0.7.17</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/solidity-coverage-0.x`
  - Merge into: `main`
  - Upgrade [solidity-coverage](https://togithub.com/sc-forks/solidity-coverage) to `0.7.17`


</details>

<details>
<summary>chore(deps): update hyperledger/fabric-orderer docker tag to v2.3.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-fabric-orderer-2.x`
  - Merge into: `main`
  - Upgrade hyperledger/fabric-orderer to `2.3.3`


</details>

<details>
<summary>chore(deps): update hyperledger/fabric-peer docker tag to v2.3.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-fabric-peer-2.x`
  - Merge into: `main`
  - Upgrade hyperledger/fabric-peer to `2.3.3`


</details>

<details>
<summary>fix(deps): update dependency @eth-optimism/plugins to v0.0.20</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/eth-optimism-plugins-0.x`
  - Merge into: `main`
  - Upgrade @eth-optimism/plugins to `0.0.20`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;types/react to v16.14.21</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-16.x`
  - Merge into: `main`
  - Upgrade [@types/react](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `16.14.21`


</details>

<details>
<summary>fix(deps): update dependency bootstrap to v4.6.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/bootstrap-4.x`
  - Merge into: `main`
  - Upgrade [bootstrap](https://togithub.com/twbs/bootstrap) to `4.6.1`


</details>

<details>
<summary>fix(deps): update dependency chalk to v4.1.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/chalk-4.x`
  - Merge into: `main`
  - Upgrade [chalk](https://togithub.com/chalk/chalk) to `4.1.2`


</details>

<details>
<summary>fix(deps): update dependency fabric-shim to v2.2.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/fabric-shim-2.x`
  - Merge into: `main`
  - Upgrade [fabric-shim](https://togithub.com/hyperledger/fabric-chaincode-node) to `2.2.2`


</details>

<details>
<summary>fix(deps): update dependency node-fetch to v2.6.6</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/node-fetch-2.x`
  - Merge into: `main`
  - Upgrade [node-fetch](https://togithub.com/node-fetch/node-fetch) to `2.6.6`


</details>

<details>
<summary>fix(deps): update dependency react-copy-to-clipboard to v5.0.4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-copy-to-clipboard-5.x`
  - Merge into: `main`
  - Upgrade [react-copy-to-clipboard](https://togithub.com/nkbt/react-copy-to-clipboard) to `5.0.4`


</details>

<details>
<summary>fix(deps): update dependency react-google-recaptcha-v3 to v1.9.7</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-google-recaptcha-v3-1.x`
  - Merge into: `main`
  - Upgrade [react-google-recaptcha-v3](https://togithub.com/t49tran/react-google-recaptcha-v3) to `1.9.7`


</details>

<details>
<summary>fix(deps): update dependency react-native-web to v0.17.5</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-native-web-0.x`
  - Merge into: `main`
  - Upgrade [react-native-web](https://togithub.com/necolas/react-native-web) to `0.17.5`


</details>

<details>
<summary>fix(deps): update dependency react-scripts to v3.4.4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-scripts-3.x`
  - Merge into: `main`
  - Upgrade [react-scripts](https://togithub.com/facebook/create-react-app) to `3.4.4`


</details>

<details>
<summary>fix(deps): update dependency request-promise-native to v1.0.9</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/request-promise-native-1.x`
  - Merge into: `main`
  - Upgrade [request-promise-native](https://togithub.com/request/request-promise-native) to `1.0.9`


</details>

<details>
<summary>fix(deps): update dependency swagger-ui-express to v4.1.6</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/swagger-ui-express-4.x`
  - Merge into: `main`
  - Upgrade [swagger-ui-express](https://togithub.com/scottie1984/swagger-ui-express) to `4.1.6`
  - Upgrade [@types/swagger-ui-express](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.1.3`


</details>

<details>
<summary>fix(deps): update dependency web3modal to v1.9.4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/web3modal-1.x`
  - Merge into: `main`
  - Upgrade [web3modal](https://togithub.com/web3modal/web3modal) to `1.9.4`


</details>

<details>
<summary>fix(deps): update dependency wouter to v2.7.5</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/wouter-2.x`
  - Merge into: `main`
  - Upgrade [wouter](https://togithub.com/molefrog/wouter) to `2.7.5`


</details>

<details>
<summary>fix(deps): update module github.com/hyperledger/fabric to v1.4.12</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/github.com-hyperledger-fabric-1.x`
  - Merge into: `main`
  - Upgrade [github.com/hyperledger/fabric](https://togithub.com/hyperledger/fabric) to `v1.4.12`


</details>

<details>
<summary>chore(deps): update alpine docker tag to v3.15</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/alpine-3.x`
  - Merge into: `main`
  - Upgrade alpine to `3.15`


</details>

<details>
<summary>chore(deps): update couchdb docker tag to v3.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/couchdb-3.x`
  - Merge into: `main`
  - Upgrade couchdb to `3.2`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;openzeppelin/hardhat-upgrades to v1.12.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/openzeppelin-hardhat-upgrades-1.x`
  - Merge into: `main`
  - Upgrade [@openzeppelin/hardhat-upgrades](https://togithub.com/OpenZeppelin/openzeppelin-upgrades) to `1.12.0`


</details>

<details>
<summary>chore(deps): update dependency @typescript-eslint/eslint-plugin to v4.33.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/typescript-eslint-monorepo`
  - Merge into: `main`
  - Upgrade [@typescript-eslint/eslint-plugin](https://togithub.com/typescript-eslint/typescript-eslint) to `4.33.0`


</details>

<details>
<summary>chore(deps): update dependency chai to v4.3.4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/chai-4.x`
  - Merge into: `main`
  - Upgrade [chai](https://togithub.com/chaijs/chai) to `4.3.4`
  - Upgrade [@types/chai](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `4.2.22`


</details>

<details>
<summary>chore(deps): update dependency cspell to v5.13.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/cspell-5.x`
  - Merge into: `main`
  - Upgrade [cspell](https://togithub.com/streetsidesoftware/cspell) to `5.13.1`


</details>

<details>
<summary>chore(deps): update dependency ethereum-waffle to v3.4.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ethereum-waffle-3.x`
  - Merge into: `main`
  - Upgrade [ethereum-waffle](https://togithub.com/EthWorks/Waffle) to `3.4.0`


</details>

<details>
<summary>chore(deps): update dependency ethers to v5.5.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ethers-5.x`
  - Merge into: `main`
  - Upgrade [ethers](https://togithub.com/ethers-io/ethers.js) to `5.5.1`


</details>

<details>
<summary>chore(deps): update dependency hardhat to v2.7.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hardhat-2.x`
  - Merge into: `main`
  - Upgrade [hardhat](https://togithub.com/nomiclabs/hardhat) to `2.7.0`


</details>

<details>
<summary>chore(deps): update dependency hardhat-deploy to v0.9.12</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hardhat-deploy-0.x`
  - Merge into: `main`
  - Upgrade [hardhat-deploy](https://togithub.com/wighawag/hardhat-deploy) to `0.9.12`


</details>

<details>
<summary>chore(deps): update dependency prettier to v2.5.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/prettier-2.x`
  - Merge into: `main`
  - Upgrade [prettier](https://togithub.com/prettier/prettier) to `2.5.0`


</details>

<details>
<summary>chore(deps): update dependency typescript to v4.5.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/typescript-4.x`
  - Merge into: `main`
  - Upgrade [typescript](https://togithub.com/Microsoft/TypeScript) to `4.5.2`


</details>

<details>
<summary>chore(deps): update golang docker tag to v1.17.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/golang-1.x`
  - Merge into: `main`
  - Upgrade golang to `1.17.3-alpine3.14`
  - Upgrade golang to `1.17.3-alpine`


</details>

<details>
<summary>chore(deps): update hyperledger/explorer docker tag to v1.2.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-explorer-1.x`
  - Merge into: `main`
  - Upgrade hyperledger/explorer to `1.2.0`


</details>

<details>
<summary>chore(deps): update hyperledger/explorer-db docker tag to v1.2.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-explorer-db-1.x`
  - Merge into: `main`
  - Upgrade hyperledger/explorer-db to `1.2.0`


</details>

<details>
<summary>chore(deps): update hyperledger/fabric-ca docker tag to v1.5.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-fabric-ca-1.x`
  - Merge into: `main`
  - Upgrade hyperledger/fabric-ca to `1.5.2`


</details>

<details>
<summary>chore(deps): update localstack/localstack docker tag to v0.13.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/localstack-localstack-0.x`
  - Merge into: `main`
  - Upgrade localstack/localstack to `0.13.0`


</details>

<details>
<summary>chore(deps): update node.js to v12.22.7</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/node-12.x`
  - Merge into: `main`
  - Upgrade [node](https://togithub.com/nodejs/node) to `12.22.7-alpine`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;ethersproject/contracts to v5.5.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ethersproject-contracts-5.x`
  - Merge into: `main`
  - Upgrade [@ethersproject/contracts](https://togithub.com/ethers-io/ethers.js) to `5.5.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;ethersproject/providers to v5.5.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ethersproject-providers-5.x`
  - Merge into: `main`
  - Upgrade [@ethersproject/providers](https://togithub.com/ethers-io/ethers.js) to `5.5.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;graphprotocol/graph-cli to v0.24.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/graphprotocol-graph-cli-0.x`
  - Merge into: `main`
  - Upgrade @&#8203;graphprotocol/graph-cli to `0.24.1`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;graphprotocol/graph-ts to v0.24.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/graphprotocol-graph-ts-0.x`
  - Merge into: `main`
  - Upgrade @&#8203;graphprotocol/graph-ts to `0.24.1`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;hyperledger/cactus-common to v0.10.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-cactus-common-0.x`
  - Merge into: `main`
  - Upgrade [@hyperledger/cactus-common](https://togithub.com/hyperledger/cactus) to `0.10.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;hyperledger/cactus-plugin-ledger-connector-fabric to v0.10.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/hyperledger-cactus-plugin-ledger-connector-fabric-0.x`
  - Merge into: `main`
  - Upgrade [@hyperledger/cactus-plugin-ledger-connector-fabric](https://togithub.com/hyperledger/cactus) to `0.10.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;walletconnect/web3-provider to v1.6.6</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/walletconnect-web3-provider-1.x`
  - Merge into: `main`
  - Upgrade [@walletconnect/web3-provider](https://togithub.com/walletconnect/walletconnect-monorepo) to `1.6.6`


</details>

<details>
<summary>fix(deps): update dependency axios to v0.24.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/axios-0.x`
  - Merge into: `main`
  - Upgrade [axios](https://togithub.com/axios/axios) to `0.24.0`


</details>

<details>
<summary>fix(deps): update dependency debug to v3.2.7</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/debug-3.x`
  - Merge into: `main`
  - Upgrade [debug](https://togithub.com/visionmedia/debug) to `3.2.7`


</details>

<details>
<summary>fix(deps): update dependency express-validator to v6.13.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/express-validator-6.x`
  - Merge into: `main`
  - Upgrade [express-validator](https://togithub.com/express-validator/express-validator) to `6.13.0`


</details>

<details>
<summary>fix(deps): update dependency jsrsasign to v10.5.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/jsrsasign-10.x`
  - Merge into: `main`
  - Upgrade [jsrsasign](https://togithub.com/kjur/jsrsasign) to `10.5.0`


</details>

<details>
<summary>fix(deps): update dependency pg to v8.7.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/pg-8.x`
  - Merge into: `main`
  - Upgrade [pg](https://togithub.com/brianc/node-postgres) to `8.7.1`


</details>

<details>
<summary>fix(deps): update dependency react-bootstrap to v1.6.4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-bootstrap-1.x`
  - Merge into: `main`
  - Upgrade [react-bootstrap](https://togithub.com/react-bootstrap/react-bootstrap) to `1.6.4`


</details>

<details>
<summary>fix(deps): update dependency react-datetime to v3.1.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-datetime-3.x`
  - Merge into: `main`
  - Upgrade [react-datetime](https://togithub.com/arqex/react-datetime) to `3.1.1`


</details>

<details>
<summary>fix(deps): update dependency react-icons to v4.3.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-icons-4.x`
  - Merge into: `main`
  - Upgrade [react-icons](https://togithub.com/react-icons/react-icons) to `4.3.1`


</details>

<details>
<summary>fix(deps): update dependency react-native to v0.66.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-monorepo`
  - Merge into: `main`
  - Upgrade [react-native](https://togithub.com/facebook/react-native) to `0.66.3`


</details>

<details>
<summary>fix(deps): update dependency react-router-dom to v5.3.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-router-monorepo`
  - Merge into: `main`
  - Upgrade [react-router-dom](https://togithub.com/remix-run/react-router) to `5.3.0`


</details>

<details>
<summary>fix(deps): update dependency sequelize to v6.11.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/sequelize-6.x`
  - Merge into: `main`
  - Upgrade [sequelize](https://togithub.com/sequelize/sequelize) to `6.11.0`


</details>

<details>
<summary>fix(deps): update dependency styled-components to v5.3.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/styled-components-5.x`
  - Merge into: `main`
  - Upgrade [styled-components](https://togithub.com/styled-components/styled-components) to `5.3.3`


</details>

<details>
<summary>fix(deps): update dependency web3 to v1.6.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/web3-1.x`
  - Merge into: `main`
  - Upgrade [web3](https://togithub.com/ethereum/web3.js) to `1.6.1`


</details>

<details>
<summary>fix(deps): update material-ui monorepo</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/material-ui-monorepo`
  - Merge into: `main`
  - Upgrade [@material-ui/core](https://togithub.com/mui-org/material-ui) to `4.12.3`
  - Upgrade [@material-ui/lab](https://togithub.com/mui-org/material-ui) to `4.0.0-alpha.60`


</details>

<details>
<summary>fix(deps): update module github.com/stretchr/testify to v1.7.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/github.com-stretchr-testify-1.x`
  - Merge into: `main`
  - Upgrade [github.com/stretchr/testify](https://togithub.com/stretchr/testify) to `v1.7.0`


</details>

<details>
<summary>chore(deps): update alpine docker tag to v20210804</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/alpine-20210804.x`
  - Merge into: `main`
  - Upgrade alpine to `20210804`


</details>

<details>
<summary>chore(deps): update dependency @&#8203;types/node to v16.11.10</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/node-16.x`
  - Merge into: `main`
  - Upgrade [@types/node](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `16.11.10`


</details>

<details>
<summary>chore(deps): update dependency eslint to v8</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/eslint-8.x`
  - Merge into: `main`
  - Upgrade [eslint](https://togithub.com/eslint/eslint) to `8.3.0`


</details>

<details>
<summary>chore(deps): update dependency mocha to v9</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/mocha-9.x`
  - Merge into: `main`
  - Upgrade [mocha](https://togithub.com/mochajs/mocha) to `9.1.3`
  - Upgrade [@types/mocha](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `9.0.0`


</details>

<details>
<summary>chore(deps): update dependency nyc to v15</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/nyc-15.x`
  - Merge into: `main`
  - Upgrade [nyc](https://togithub.com/istanbuljs/nyc) to `15.1.0`


</details>

<details>
<summary>chore(deps): update dependency sinon to v12</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/sinon-12.x`
  - Merge into: `main`
  - Upgrade [sinon](https://togithub.com/sinonjs/sinon) to `12.0.1`


</details>

<details>
<summary>chore(deps): update dependency ts-node to v10.4.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ts-node-10.x`
  - Merge into: `main`
  - Upgrade [ts-node](https://togithub.com/TypeStrong/ts-node) to `10.4.0`


</details>

<details>
<summary>chore(deps): update node.js</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/node-17.x`
  - Merge into: `main`
  - Upgrade [node](https://togithub.com/nodejs/node) to `17.1.0-alpine`
  - Upgrade [node](https://togithub.com/nodejs/node) to `17-alpine`


</details>

<details>
<summary>chore(deps): update typescript-eslint monorepo to v5 (major)</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/major-typescript-eslint-monorepo`
  - Merge into: `main`
  - Upgrade [@typescript-eslint/eslint-plugin](https://togithub.com/typescript-eslint/typescript-eslint) to `5.4.0`
  - Upgrade [@typescript-eslint/parser](https://togithub.com/typescript-eslint/typescript-eslint) to `5.4.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;apollo/react-hooks to v4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/major-apollo-graphql-packages`
  - Merge into: `main`
  - Upgrade [@apollo/react-hooks](https://togithub.com/apollographql/react-apollo) to `4.0.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;openzeppelin/contracts to v4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/openzeppelin-contracts-4.x`
  - Merge into: `main`
  - Upgrade [@openzeppelin/contracts](https://togithub.com/OpenZeppelin/openzeppelin-contracts) to `^4.0.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;openzeppelin/contracts-upgradeable to v4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/openzeppelin-contracts-upgradeable-4.x`
  - Merge into: `main`
  - Upgrade [@openzeppelin/contracts-upgradeable](https://togithub.com/OpenZeppelin/openzeppelin-contracts-upgradeable) to `^4.0.0`


</details>

<details>
<summary>fix(deps): update dependency @testing-library/dom to v8</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/testing-library-dom-8.x`
  - Merge into: `main`
  - Upgrade [@testing-library/dom](https://togithub.com/testing-library/dom-testing-library) to `8.11.1`


</details>

<details>
<summary>fix(deps): update dependency @testing-library/jest-dom to v5.15.1</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/testing-library-jest-dom-5.x`
  - Merge into: `main`
  - Upgrade [@testing-library/jest-dom](https://togithub.com/testing-library/jest-dom) to `5.15.1`


</details>

<details>
<summary>fix(deps): update dependency @testing-library/react to v12.1.2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/testing-library-react-12.x`
  - Merge into: `main`
  - Upgrade [@testing-library/react](https://togithub.com/testing-library/react-testing-library) to `12.1.2`


</details>

<details>
<summary>fix(deps): update dependency @testing-library/user-event to v13.5.0</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/testing-library-user-event-13.x`
  - Merge into: `main`
  - Upgrade [@testing-library/user-event](https://togithub.com/testing-library/user-event) to `13.5.0`


</details>

<details>
<summary>fix(deps): update dependency @&#8203;types/react to v17</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-17.x`
  - Merge into: `main`
  - Upgrade [@types/react](https://togithub.com/DefinitelyTyped/DefinitelyTyped) to `17.0.37`


</details>

<details>
<summary>fix(deps): update dependency bootstrap to v5.1.3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/bootstrap-5.x`
  - Merge into: `main`
  - Upgrade [bootstrap](https://togithub.com/twbs/bootstrap) to `5.1.3`


</details>

<details>
<summary>fix(deps): update dependency chalk to v5</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/chalk-5.x`
  - Merge into: `main`
  - Upgrade [chalk](https://togithub.com/chalk/chalk) to `5.0.0`


</details>

<details>
<summary>fix(deps): update dependency debug to v4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/debug-4.x`
  - Merge into: `main`
  - Upgrade [debug](https://togithub.com/visionmedia/debug) to `4.3.3`


</details>

<details>
<summary>fix(deps): update dependency dotenv to v10</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/dotenv-10.x`
  - Merge into: `main`
  - Upgrade [dotenv](https://togithub.com/motdotla/dotenv) to `^10.0.0`


</details>

<details>
<summary>fix(deps): update dependency eslint-plugin-flowtype to v8</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/eslint-plugin-flowtype-8.x`
  - Merge into: `main`
  - Upgrade [eslint-plugin-flowtype](https://togithub.com/gajus/eslint-plugin-flowtype) to `8.0.3`


</details>

<details>
<summary>fix(deps): update dependency graphql to v16</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/graphql-16.x`
  - Merge into: `main`
  - Upgrade [graphql](https://togithub.com/graphql/graphql-js) to `16.0.1`


</details>

<details>
<summary>fix(deps): update dependency ipfs-http-client to v54</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/ipfs-http-client-54.x`
  - Merge into: `main`
  - Upgrade [ipfs-http-client](https://togithub.com/ipfs/js-ipfs) to `54.0.2`


</details>

<details>
<summary>fix(deps): update dependency node-fetch to v3</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/node-fetch-3.x`
  - Merge into: `main`
  - Upgrade [node-fetch](https://togithub.com/node-fetch/node-fetch) to `3.1.0`


</details>

<details>
<summary>fix(deps): update dependency react-bootstrap to v2</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-bootstrap-2.x`
  - Merge into: `main`
  - Upgrade [react-bootstrap](https://togithub.com/react-bootstrap/react-bootstrap) to `2.0.2`


</details>

<details>
<summary>fix(deps): update dependency react-router-dom to v6</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/major-react-router-monorepo`
  - Merge into: `main`
  - Upgrade [react-router-dom](https://togithub.com/remix-run/react-router) to `6.0.2`


</details>

<details>
<summary>fix(deps): update dependency react-scripts to v4</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/react-scripts-4.x`
  - Merge into: `main`
  - Upgrade [react-scripts](https://togithub.com/facebook/create-react-app) to `4.0.3`


</details>

<details>
<summary>fix(deps): update dependency yargs to v17</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/yargs-17.x`
  - Merge into: `main`
  - Upgrade [yargs](https://togithub.com/yargs/yargs) to `^17.0.0`


</details>

<details>
<summary>fix(deps): update react monorepo to v17 (major)</summary>

  - Schedule: ["at any time"]
  - Branch name: `renovate/major-react-monorepo`
  - Merge into: `main`
  - Upgrade [react](https://togithub.com/facebook/react) to `17.0.2`
  - Upgrade [react-dom](https://togithub.com/facebook/react) to `17.0.2`


</details>

<br />

🚸 Branch creation will be limited to maximum 2 per hour, so it doesn't swamp any CI resources or spam the project. See docs for `prhourlylimit` for details.


---

❓ Got questions? Check out Renovate's [Docs](https://docs.renovatebot.com/), particularly the Getting Started section.
If you need any further assistance then you can also [request help here](https://togithub.com/renovatebot/renovate/discussions).


---

This PR has been generated by [WhiteSource Renovate](https://renovate.whitesourcesoftware.com). View repository job log [here](https://app.renovatebot.com/dashboard#{{platform}}/{{repository}}).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 17:44:22 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger-labs/blockchain-carbon-accounting/pull/365" class=".btn">#365</a>
            </td>
            <td>
                <b>
                    feat (test): Test if emission factors for the correct year are used
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR modifies the test setup script to use the real utility data present in the eGRID 2018 and 2019 datasets (Los Angeles Department of Water and Power), to insert 2 data records.  Then, 2 emissions are recorded, one in the year 2018 and one in the year 2019. Then we assert the following conditions:
- The emissions amounts of both years must not be equal
- The emissions amounts of each year should match the value calculated as per the eGRID data of that year

The emissions data is fetched from the CouchDB database using the [HTTP /db/_find API](https://docs.couchdb.org/en/latest/api/database/find.html). Then, the emissions factors are calculated and checked against the values stored on the ledger.

Closes #302 and #316.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-11-22 16:15:30 +0000 UTC
    </div>
</div>

