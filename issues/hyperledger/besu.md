---
layout: default
title: besu
parent: Hyperledger
grand_parent: Issues
has_children: false
permalink: /issues/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2308" class=".btn">2308</a>
            </td>
            <td>
                <b>
                    Separate Listening and Discovery Ports in Node Configuration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span>
            </td>
            <td>
                ### Description
According to the documentation on [P2P Port](https://besu.hyperledger.org/en/stable/Reference/CLI/CLI-Syntax/#p2p-port) configuration, the `--p2p-port` options/`BESU_P2P_PORT` environment variable/`p2p-port` configuration file option can be used to configure the listening port for the node, which is used for both the TCP listening port and the UDP discovery port.

Strangely enough, there are sections in the documentation that describe a valid [Enode URL](https://besu.hyperledger.org/en/stable/Concepts/Node-Keys/#enode-url) that allows setting a different discovery port using a `discport` query parameter.

This brings the question of if those Enode URLs are supported, how can one configure a dedicated port for discovery, which has a different number than the listening port.

### Acceptance Criteria
Allow configuring the listening port and discovery port of the node separatly,

### Additional Information
It might seem like a small issue, but in scenarios that require exposing both ports, it creates limitations such as the cloud services that can be used to run nodes (at the time of opening this issue, both Azure ACI and AWS ECS do not support opening the same port number for both TCP and UDP at the same time).

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-20 14:08:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2190" class=".btn">2190</a>
            </td>
            <td>
                <b>
                    Unit tests fail if system language is not English
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">dev experience</span><span class="chip">good first issue</span>
            </td>
            <td>
                ### Description
The tests `BesuCommandTest.privEnclaveKeyFileDoesNotExist` and `NetworkingServiceLifecycleTest.startDiscoveryPortInUse` fail if the system language of the operating system is another language than English. In `BesuCommandTest.privEnclaveKeyFileDoesNotExist` the test looks like this:

```
@Test
public void privEnclaveKeyFileDoesNotExist() {
  parseCommand("--privacy-enabled=true", "--privacy-public-key-file", "/non/existent/file");

  assertThat(commandOutput.toString()).isEmpty();
  assertThat(commandErrorOutput.toString()).startsWith("Problem with privacy-public-key-file");
  assertThat(commandErrorOutput.toString()).contains("No such file");
}
```

The last assertion is the one that is failing. `No such file` is the error message coming directly from `IOException` when the file is not found. But the error messages of the exceptions thrown by the Java library are translated according to the system language. For example when the system language is set to Spanish the error looks like this:

```
Problem with privacy-public-key-file: /non/existent/file (No existe el archivo o el directorio)
```

In this case `No such file` is not part of the output string and the assertion fails.

 `NetworkingServiceLifecycleTest.startDiscoveryPortInUse`  fails for the same reason:
 
 ```
catch (final Exception e) {
          assertThat(e).hasCauseExactlyInstanceOf(PeerDiscoveryServiceException.class);
          assertThat(e)
              .hasMessageStartingWith(
                  "org.hyperledger.besu.ethereum.p2p.discovery."
                      + "PeerDiscoveryServiceException: Failed to bind Ethereum UDP discovery listener to 0.0.0.0:");

          assumeThat(System.getProperty("user.language")).isEqualTo("en");
          assertThat(e).hasMessageContaining("Address already in use");
        } 
```

Here again the last assertion fails, because it comes directly from an exception thrown by the Java library.

### Expected behavior
The tests should either be successful or be skipped.

### Possible solution
The tests could be skipped using [AssertJ Assume](https://assertj.github.io/doc/#assertj-core-assumptions) and testing if the system language is English or not. Like that they would not fail for developers with another system language. But they would still be executed in the CI / CD pipeline, to verify that the tested behavior has not been changed.

### Steps to Reproduce (Bug)
1. Checkout `master` branch
2. Change system language to any other than English
3. Execute `./gradlew build` 


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-04-26 11:24:46 +0000 UTC
    </div>
</div>

