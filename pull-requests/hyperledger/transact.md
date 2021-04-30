---
layout: default
title: transact
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/transact
---

# transact <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/transact){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/127" class=".btn">#127</a>
            </td>
            <td>
                <b>
                    Command family smart contract
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR updates the command family and adds a sabre compatible command smart contract.

The `make_command_transaction` method is moved behind a separate experimental feature to allow for the command smart contract to be compiled into wasm.

The command family transaction handler is updated to use namespaces and a method is added to generate the sha512 hash of "command".

The necessary information is added to the docker files to allow for the command smart contract scar file to be build and archived in Jenkins.

### **Testing:**

1. Checkout the branch in this PR which adds the CLI subcommands for interacting with the command family smart contract: https://github.com/hyperledger/transact/pull/126
2. Start two splinter nodes and create a circuit between them with scabbard services
3. Download the command family smart contract scar file found here: https://build.sawtooth.me/job/Transact-Hyperledger/job/transact/job/PR-127/1/artifact/build/scar/
4. Upload the command family smart contract to the circuit using the scabbard CLI
5. Create a namespace registry for the contract using the namespace "06abbc"
```
scabbard ns create 06abbc \
    --owners <public_key> \
    --key <path_to_private_key> \
    --url http://0.0.0.0:8080 \
    --service-id <circuit-id>::<scabbard-service-id>
```
6. Add read and write permissions for the contract
```
scabbard perm 06abbc command --read --write \
    --key <path_to_private_key> \
    --url http://0.0.0.0:8080 \
    --service-id <circuit-id>::<scabbard-service-id>
```
7. Start the transact CLI using the branch from step 1, if you are using a docker file for your splinter nodes you can add something similar to the following to your docker file: 
```
  transact-cli:
    image: transact-cli
    build:
      context: ../transact
      dockerfile: ./cli/Dockerfile
      args:
      - CARGO_ARGS=${CARGO_ARGS}
      - REPO_VERSION=0.4.1-dev
    container_name: transact-cli
    hostname: transact-cli
```
and then set the environment variable `CARGO_ARGS="-- --features=experimental"` and then run `docker-compose -f <docker-file-name>.yaml run transact-cli bash` in a new terminal window to start the transact CLI 
(alternatively the transact commands can be run from the transact/cli directory as `cargo run --features=experimental ...`)

8. Run a set-state command
```
transact command set-state \
  --key /alice.priv
  --target "http://0.0.0.0:8080/scabbard/<circuit-id>/<scabbard-service-id>"
  --state-entry 06abbcb16ed7d24b3ecbd4164dcdad374e08c0ab7518aa07f9d3683f34c2b3c67a1583:state-value
```
9. Check the splinterd logs to see if the transaction was successfully submitted
10. Run a show-state command
```
transact command show-state \
  --key /alice.priv
  --target "http://0.0.0.0:8080/scabbard/<circuit-id>/<scabbard-service-id>"
  --address 06abbcb16ed7d24b3ecbd4164dcdad374e08c0ab7518aa07f9d3683f34c2b3c67a1583
  --text
```
11. Check that the "state-value" is returned
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 00:24:34 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/126" class=".btn">#126</a>
            </td>
            <td>
                <b>
                    Command family cli subcommands
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Adds subcommands to the transact cli to interact with the command family smart contract. This is behind the experimental feature "command".

### **Testing:**

1. Checkout the branch in this PR which updates the command family and adds a command family smart contract: https://github.com/hyperledger/transact/pull/126
2. Start two splinter nodes and create a circuit between them with scabbard services
3. Download the command family smart contract scar file found here: https://build.sawtooth.me/job/Transact-Hyperledger/job/transact/job/PR-127/1/artifact/build/scar/
4. Upload the command family smart contract to the circuit using the scabbard CLI
5. Create a namespace registry for the contract using the namespace "06abbc"
```
scabbard ns create 06abbc \
    --owner <public_key> \
    --key <path_to_private_key> \
    --url http://0.0.0.0:8080 \
    --service-id <circuit-id>::<scabbard-service-id>
```
6. Add read and write permissions for the contract
```
scabbard perm 06abbc command --read --write \
    --key <path_to_private_key> \
    --url http://0.0.0.0:8080 \
    --service-id <circuit-id>::<scabbard-service-id>
```
7. Start the transact CLI using the branch from step 1, if you are using a docker file for your splinter nodes you can add something similar to the following to your docker file: 
```
  transact-cli:
    image: transact-cli
    build:
      context: ../transact
      dockerfile: ./cli/Dockerfile
      args:
      - CARGO_ARGS=${CARGO_ARGS}
      - REPO_VERSION=0.4.1-dev
    container_name: transact-cli
    hostname: transact-cli
```
and then set the environment variable `CARGO_ARGS="-- --features=experimental"` and then run `docker-compose -f <docker-file-name>.yaml run transact-cli bash` in a new terminal window to start the transact CLI 
(alternatively the transact commands can be run from the transact/cli directory as `cargo run --features=experimental ...`)

8. Run a set-state command
```
transact command set-state \
  --key /alice.priv
  --target "http://0.0.0.0:8080/scabbard/<circuit-id>/<scabbard-service-id>"
  --state-entry 06abbcb16ed7d24b3ecbd4164dcdad374e08c0ab7518aa07f9d3683f34c2b3c67a1583:state-value
```
9. Check the splinterd logs to see if the transaction was successfully submitted
10. Run a show-state command
```
transact command show-state \
  --key /alice.priv
  --target "http://0.0.0.0:8080/scabbard/<circuit-id>/<scabbard-service-id>"
  --address 06abbcb16ed7d24b3ecbd4164dcdad374e08c0ab7518aa07f9d3683f34c2b3c67a1583
  --text
```
11. Check that the "state-value" is returned
12. Run a get-state command 
```
transact command get-state \
  --key /alice.priv
  --target "http://0.0.0.0:8080/scabbard/<circuit-id>/<scabbard-service-id>"
  --address 06abbcb16ed7d24b3ecbd4164dcdad374e08c0ab7518aa07f9d3683f34c2b3c67a1583
```
13. Check the splinterd logs to see if the get state transaction was successfully submitted, the transact cli should not display anything after running this command.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-30 00:22:40 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/transact/pull/123" class=".btn">#123</a>
            </td>
            <td>
                <b>
                    Update dependencies
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Updates various dependencies, cleaning up the output of 'cargo outdated -R'.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-28 23:05:58 +0000 UTC
    </div>
</div>

