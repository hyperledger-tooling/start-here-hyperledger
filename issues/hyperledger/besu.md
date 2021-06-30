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

<div>
    <table>
        <tr>
            <td>
                Issue <a href="https://github.com/hyperledger/besu/issues/2069" class=".btn">2069</a>
            </td>
            <td>
                <b>
                    Make ignored dependent configuration warnings consistent between CLI options and TOML config
                </b>
            </td>
        </tr>
        <tr>
            <td>
                <span class="chip">good first issue</span><span class="chip">logging</span>
            </td>
            <td>
                <!-- Have you done the following? -->
<!--   * read the Code of Conduct? By filing an Issue, you are expected to -->  
<!--     comply with it, including treating everyone with respect: -->
<!--     https://github.com/hyperledger/besu/blob/master/CODE_OF_CONDUCT.md -->
<!--   * Reproduced the issue in the latest version of the software -->
<!--   * Read the debugging docs: https://besu.hyperledger.org/en/stable/HowTo/Monitor/Logging/ -->
<!--   * Duplicate Issue check:  https://github.com/search?q=+is%3Aissue+repo%3Ahyperledger/Besu -->
<!-- Note:  Not all sections will apply to all issue types. -->

### Description
Dependent options specified on the command line will trigger warnings, while the same options specified in a TOML file don't.

For example:
`WARN  | Besu | --min-gas-price has been ignored because --miner-enabled was not defined on the command line.`
^ This message is displayed when the CLI options are misconfigured, but not when the same configuration is used in a TOML file.

It likely affects CLI options being verified in CommandLineUtils, which may include:

- GraphQL options
- Metrics options
- Mining options
- P2P options
- PrivacyParameters
- Privacy TLS
- RPC options
- Sync options


### Acceptance Criteria
Warnings for ignored options will be displayed when using both CLI options and TOML configuration.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-03-24 01:29:30 +0000 UTC
    </div>
</div>

