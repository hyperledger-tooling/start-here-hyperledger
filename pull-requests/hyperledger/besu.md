---
layout: default
title: besu
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/besu
---

# besu <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/besu){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/besu/pull/6988" class=".btn">#6988</a>
            </td>
            <td>
                <b>
                    Fix "CORS Rejected - Invalid origin" issue when origin header is empty
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ## PR description
Fix "CORS Rejected - Invalid origin" issue when the origin allowed hosts is set to * and actual origin is empty (not null, but empty).

The regex may appear a bit weird at first glance, but this change is more related to the change in Vertx implementation between 4.3.5 and 4.5.4. This new regex will make sure that Vertx CorsHandler will try to match origin values to that regex. 

Vertx 4.3.5 (old regex in Besu is `.*`)
```
public CorsHandlerImpl(String allowedOriginPattern) {
    Objects.requireNonNull(allowedOriginPattern);
    if ("*".equals(allowedOriginPattern)) {
      allowedOrigin = null;
    } else {
      allowedOrigin = Pattern.compile(allowedOriginPattern);
    }
    allowedOrigins = null;
  }
```

Vertx 4.5.4 (regex in Besu is `.*://.*`)
```
  public CorsHandler addRelativeOrigin(String origin) {
    Objects.requireNonNull(origin, "'origin' cannot be null");

    if (relativeOrigins == null) {
      if (origin.equals(".*")) {
        // we signal any as null
        return this;
      }
      relativeOrigins = new LinkedHashSet<>();
    } else {
      if (origin.equals(".*")) {
        // we signal any as null
        throw new IllegalStateException("Cannot mix '/.*/' with relative origins");
      }
    }
    relativeOrigins.add(Pattern.compile(origin));
    return this;
  }
```


## Fixed Issue(s)
https://github.com/hyperledger/besu/issues/6983
<!-- Please link to fixed issue(s) here using format: fixes #<issue number> -->
<!-- Example: "fixes #2" -->


### Thanks for sending a pull request! Have you done the following?

- [x] Checked out our [contribution guidelines](https://github.com/hyperledger/besu/blob/main/CONTRIBUTING.md)?
- [x] Considered documentation and added the `doc-change-required` label to this PR [if updates are required](https://wiki.hyperledger.org/display/BESU/Documentation).
- [x] Considered the changelog and included an [update if required](https://wiki.hyperledger.org/display/BESU/Changelog).
- [x] For database changes (e.g. KeyValueSegmentIdentifier) considered compatibility and performed forwards and backwards compatibility tests

### Locally, you can run these tests to catch failures early:

- [x] unit tests: `./gradlew build`
- [ ] acceptance tests: `./gradlew acceptanceTest`
- [ ] integration tests: `./gradlew integrationTest`
- [ ] reference tests: `./gradlew ethereum:referenceTests:referenceTests`


            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2024-04-23 16:44:47 +0000 UTC
    </div>
</div>

