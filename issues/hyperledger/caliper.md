---
layout: default
title: caliper
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/caliper
---

# caliper <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/caliper){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/caliper/issues/1516" class=".btn">1516</a>
            </td>
            <td>
                <b>
                    Benchmarking Ethereum Network (Error: Nonce undefined)
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">help wanted</span>
            </td>
            <td>
                ### Which Caliper version are you using?

v0.5.0

### Which Node.JS version are you using?

v18.15.0

### Which operating system are you using?

Windows 11 Pro

### Please provide some context for your error. For example, when did the error occur? What were you trying to achieve, and how?

I am using hyperledger-caliper to benchmark the Ethereum local network (Ganache). The contract is a simple storage contract, nothing fancy. I can deploy the contract. 

### What was the observed incorrect behavior?

But unable to send a request to the deployed contract.   I believe I am making some mistake or error in establishing the connection.

### Please provide the error logs and their surroundings.

```
Here is the error:

2024.02.22-13:27:41.180 error [caliper] [ethereum-connector]    Failed tx on sample calling method retrieve nonce undefined
2024.02.22-13:27:41.180 error [caliper] [ethereum-connector]    TypeError: Found non-callable @@iterator
```

Here is the response to the submit transaction command `await this.sutAdapter.sendRequests(connectorRequest)`
```
TxStatus {  
  status: {  
    id: undefined,  
    status: 'failed',  
    time_create: 1708626461180,  
    time_final: 1708626461180,  
    result: null,  
    verified: false,  
    flags: 0,  
    error_messages: [],  
    custom_data: Map(0) {}  
  }  
}  
```


### Please provide your benchmark configuration file content, if possible.

```
caliper:
  blockchain: ethereum
  ethereum:
    url: ws://127.0.0.1:7545
    gas: 40712388
    from: "0x618......d9"
    accounts:
      - privateKey: "0xe8.......d936"
        balance: "1000000000000000000000"  # Initial balance in Wei
test:
  name: basic-contract-benchmark
  description: A test benchmark
  workers:
    type: local
    number: 1
  rounds:
    - label: callFunction
      description: Call function benchmark
      txNumber: 1
      rateControl:
        type: "fixed-rate"
        opts:
          tps: 1
      workload:
        module: path/to/sample.js
      readOnly: true
```


### Please provide your network configuration file content, if possible.

```
{
    "caliper": {
        "blockchain": "ethereum"
    },
    "ethereum": {
        "url": "ws://127.0.0.1:7545",
        "contractDeployerAddress": "0x618.................d9",
        "contractDeployerAddressPassword": "",
        "contractDeployerAddressPrivateKey": "0xe.............36",
        "fromAddress": "0x61.....d9",
        "fromAddressPassword": "",
        "transactionConfirmationBlocks": 12,
        "contracts": {
            "sample": {
                "path": "path/to/sample.json"
            }
        }
    }
}
```

Here is the contract file: 
```
{
    "name": "sample",
    "abi": [{"inputs":[],"name":"retrieve","outputs":[{"internalType":"uint256","name":"","type":"uint256"}],"stateMutability":"view","type":"function","constant":true,"signature":"0x2e64cec1"},{"inputs":[{"internalType":"uint256","name":"num","type":"uint256"}],"name":"store","outputs":[],"stateMutability":"nonpayable","type":"function","signature":"0x6057361d"}],
    "bytecode": "608060405234801561001057600080fd5b5061012f806100206000396000f3fe6080604052348015600f57600080fd5b506004361060325760003560e01c80632e64cec11460375780636057361d146051575b600080fd5b603d6069565b6040516048919060c2565b60405180910390f35b6067600480360381019060639190608f565b6072565b005b60008054905090565b8060008190555050565b60008135905060898160e5565b92915050565b60006020828403121560a057600080fd5b600060ac84828501607c565b91505092915050565b60bc8160db565b82525050565b600060208201905060d5600083018460b5565b92915050565b6000819050919050565b60ec8160db565b811460f657600080fd5b5056fea2646970667358221220a919f081cdd0953c3eb15dd85fdd23cb57fcbc15f2675dfe59cc99fa69e9423864736f6c63430008000033",
    "gas": 1000000
}
```


### Please provide your workload module content, if possible.

```
const { WorkloadModuleBase, ConfigUtil } = require('@hyperledger/caliper-core');
//const web3 = new Web3('ws://127.0.0.1:7545');
const SupportedConnectors = ['ethereum'];
class MyWorkload extends WorkloadModuleBase {
    constructor() {
        super();
        //this.workerIndex = -1;
        //this.totalWorkers = -1;
        //this.roundIndex = -1;
        //this.roundArguments = undefined;
        //this.sutAdapter = undefined;
        //this.sutContext = undefined;
    }
        /**
    * Initialize the workload module with the given parameters.
    * @param {number} workerIndex The 0-based index of the worker instantiating the workload module.
    * @param {number} totalWorkers The total number of workers participating in the round.
    * @param {number} roundIndex The 0-based index of the currently executing round.
    * @param {Object} roundArguments The user-provided arguments for the round from the benchmark configuration file.
    * @param {ConnectorBase} sutAdapter The adapter of the underlying SUT.
    * @param {Object} sutContext The custom context object provided by the SUT adapter.
    * @async
    */
    async initializeWorkloadModule(workerIndex, totalWorkers, roundIndex, roundArguments, sutAdapter, sutContext) {
        await super.initializeWorkloadModule(workerIndex, totalWorkers, roundIndex, roundArguments, sutAdapter, sutContext);
        this.connectorType = this.sutAdapter.getType();
        //this.workerIndex = workerIndex;
        //this.totalWorkers = totalWorkers;
        //this.roundIndex = roundIndex;
        //this.roundArguments = roundArguments;
        //this.sutAdapter = sutAdapter;
        //this.sutContext = sutContext;
    }
      /**
     * Assemble a Ethereum-specific request from the business parameters.
     * @param {string} operation The name of the operation to invoke.
     * @param {object} args The object containing the arguments.
     * @return {object} The Ethereum-specific request.
     * @private
     */
      _createEthereumConnectorRequest(operation, args) {
        return {
            contract: 'sample',
            verb: operation,
            args: args,
            readOnly: false
        };
    }
    createConnectorRequest(operation, args) {
        switch (this.connectorType) {
            case 'ethereum':
                return this._createEthereumConnectorRequest(operation, args);
            default:
                // this shouldn't happen
                throw new Error(`Connector type ${this.connectorType} is not supported by the benchmark`);
        }
    }
    async getNextNonce(address) {
        //console.log(await this.sutAdapter.web3.eth.getTransactionCount(address));
        return await this.sutAdapter.web3.eth.getTransactionCount(address);
    }
    async submitTransaction() {
        try {
            let txArgs = {
                // Provide any required arguments for the function
            };
            const connectorRequest = this.createConnectorRequest("retrieve", txArgs);
            console.log('Connector Request:', connectorRequest);
            // Invoke smart contract
            const tx_status = await this.sutAdapter.sendRequests(connectorRequest);
            console.log(tx_status)
            // Log successful invocation
            console.log('Smart contract invoked successfully');
        } catch (error) {
            console.error('Error invoking smart contract:', error);
        }
    }
}
function createWorkloadModule() {
    return new MyWorkload();
}
module.exports.createWorkloadModule = createWorkloadModule;
```


### Please provide any additional information you deem relevant to the error.

Please advise if you need any additional information. Thank you!
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-02-22 20:07:01 +0000 UTC
    </div>
</div>

