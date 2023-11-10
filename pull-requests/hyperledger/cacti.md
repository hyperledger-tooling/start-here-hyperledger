---
layout: default
title: cacti
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/cacti
---

# cacti <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/cacti){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2869" class=".btn">#2869</a>
            </td>
            <td>
                <b>
                    fix(connector-besu): error handling of DeployContractSolidityBytecodeEndpoint
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                1. Uses the new utility function from the core package in the catch block
so that HTTP statusCode is matching the intent of the thrower (e.g.
correctly differentiates between user-error and developer error)
2. Updates the deployContract method of the besu connector so that it
correctly specifies the intent of the errors thrown as either user error
or developer error via setting the statusCode property of the HTTP errors
to either 4xx or 5xx depending on the cause.
3. Provides a template for future similar changes (of which we'll need
dozens to update all the REST API endpoints)

Depends on #2868

Related to but does not conclude: https://github.com/hyperledger/cacti/issues/1747

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 21:33:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2868" class=".btn">#2868</a>
            </td>
            <td>
                <b>
                    feat(cactus-core): add handleRestEndpointException utility to public API
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                1. This is a function that is designed to be called by all the REST API
endpoint implementations to (more) correctly handle errors.
2. The problem right now is that we do not differentiate between invalid
request errors (e.g. expected exceptions) vs.
legitimate crashes (e.g. unexpected exceptions)
What the above means is that a lot of our endpoints will crash with an
HTTP 500 error code returned to the client even if the problem as user-
error (such as a missing parameter that is mandatory).
3. With the new utility function the REST endpoint code can easily
apply the decision logic at runtime in their own catch blocks' and
set the HTTP response status code based on the information (context)
provided by the callee (most often the connector plugin's underlying
method that was called)

An example usage of this utility method can be described as:
1. Add the necessary dependencies to your plugin (`http-errors`, `@types/http-errors`)
2. `yarn install` (which will update the lock file)
3. Choose the endpoint you wish to update to be using the new handleRestEndpointException
function internally when handling HTTP requests that involve the plugin.
For example this file:
```
packages/cactus-plugin-ledger-connector-besu/src/main/typescript/
web-services/deploy-contract-solidity-bytecode-endpoint.ts
```
4. Update the `catch() { ... }` block of the `handleRequest` method to
invoke the handleRestEndpointException method:

```typescript
public async handleRequest(req: Request, res: Response): Promise<void> {
const fnTag = `${this.className}#handleRequest()`;
const reqTag = `${this.getVerbLowerCase()} - ${this.getPath()}`;
this.log.debug(reqTag);
const reqBody: DeployContractSolidityBytecodeV1Request = req.body;
try {
    const resBody = await this.options.connector.deployContract(reqBody);
    res.json(resBody);
} catch (ex) {
    const errorMsg = `${reqTag} ${fnTag} Failed to deploy contract:`;
    handleRestEndpointException({ errorMsg, log: this.log, error: ex, res });
}
}
```

Then proceed to also update the implementation of the method that is  being
called by the REST endpoint request handler such that it uses the HTTP
errors according to their intended status codes, e.g. 400 is user error
and 5xx is something that is a developer error (e.g. indicating that
a bug is in the code of the plugin and should be fixed)

```typescript
import createHttpError from "http-errors";

export class SomePluginImplementration {

  public async deployContract(
    req: DeployContractSolidityBytecodeV1Request,
  ): Promise<DeployContractSolidityBytecodeV1Response> {
    const fnTag = `${this.className}#deployContract()`;
    Checks.truthy(req, `${fnTag} req`);
    if (isWeb3SigningCredentialNone(req.web3SigningCredential)) {
      throw createHttpError[400](
        `${fnTag} Cannot deploy contract with pre-signed TX`,
      );
    }
    const { keychainId, contractName } = req;
    if (!keychainId || !req.contractName) {
      const errorMessage = `${fnTag} Cannot deploy contract without keychainId and the contractName.`;
      throw createHttpError[400](errorMessage);
    }

    const keychainPlugin = this.pluginRegistry.findOneByKeychainId(keychainId);

    if (!keychainPlugin) {
      const errorMessage =
        `${fnTag} The plugin registry does not contain` +
        ` a keychain plugin for ID:"${req.keychainId}"`;
      throw createHttpError[400](errorMessage);
    }

    if (!keychainPlugin.has(contractName)) {
      const errorMessage =
        `${fnTag} Cannot create an instance of the contract instance because` +
        `the contractName in the request does not exist on the keychain`;
      throw new createHttpError[400](errorMessage);
    }
    // rest of the implementation goes here
}
```

[skip ci]

Related to, but does NOT conclude: https://github.com/hyperledger/cacti/issues/1747

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 21:26:01 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2867" class=".btn">#2867</a>
            </td>
            <td>
                <b>
                    build(dev-container): add git auto-completion via .bashrc
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #2215

Signed-off-by: Peter Somogyvari <peter.somogyvari@accenture.com>

**Pull Request Requirements**
- [x] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [x] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [x] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [x] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [x] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-09 20:05:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/cacti/pull/2861" class=".btn">#2861</a>
            </td>
            <td>
                <b>
                    feat(indy-sdk): replace indy SDK with AFJ
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dependent</span>
            </td>
            <td>
                - Refactor test ledger `indy-testnet` into `indy-all-in-one`. New package uses
    the latest indy version, has healtcheck script, updated startup / cleanup
    scripts.
- Remove `indy-sdk-cli` image since it's not used anymore.
- Refactor `cactus-example-discounted-asset-trade` to use own aries agent
    instead of indy connector. This way it doesn't need to use indy-sdk anymore,
    and python indy connector can be safely removed / upgraded.
- Update sample app readme to explain current workflow.
- Remove client scripts since `cactus-example-discounted-asset-trade-client`
    can now be used to interact with the sample app.
- Add `cactus-example-discounted-asset-trade-client`. It contains script for
    setting up test credentials on the ledger, script with interactive menu for
    interacting with `cactus-example-discounted-asset-trade` sample app,
    and bunch of helper functions used for writing these apps.

Depends on #2859
Depends on #2860

Signed-off-by: Michal Bajer <michal.bajer@fujitsu.com>

**Pull Request Requirements**
- [ ] Rebased onto `upstream/main` branch and squashed into single commit to help maintainers review it more efficient and to avoid spaghetti git commit graphs that obfuscate which commit did exactly what change, when and, why.
- [ ] Have git sign off at the end of commit message to avoid being marked red. You can add `-s` flag when using `git commit` command. You may refer to this [link](https://docs.github.com/en/authentication/managing-commit-signature-verification/signing-commits) for more information.
- [ ] Follow the Commit Linting specification. You may refer to this [link](https://www.conventionalcommits.org/en/v1.0.0-beta.4/#specification) for more information. 

**Character Limit**
- [ ] Pull Request Title and Commit Subject must not exceed 72 characters (including spaces and special characters).
- [ ] Commit Message per line must not exceed 80 characters (including spaces and special characters).

**A Must Read for Beginners**
For rebasing and squashing, here's a [must read guide](https://github.com/servo/servo/wiki/Beginner's-guide-to-rebasing-and-squashing) for beginners.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-03 20:30:05 +0000 UTC
    </div>
</div>

