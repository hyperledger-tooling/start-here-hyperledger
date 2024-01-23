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
                PR <a href="https://github.com/hyperledger/cacti/pull/2979" class=".btn">#2979</a>
            </td>
            <td>
                <b>
                    refactor(cactus-core): catch block get-open-api-spec-v1-endpoint-base
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                    1. The GetOpenApiSpecV1EndpointBase<S, P> class now has the request
    handler migrated to the new error handling mechanism that automatically
    differentiates between HTTP statuses of 4xx and 5xx.
    2. The register-web-service-endpoint utility function uses the new error
    handling utilities as well, but on the lower level, e.g. it coerces unknown
    errors to RuntimeError instances to minimize the risk of information loss
    when re-throwing the inner exception with more context attached to it.
    3. The consensus-has-transaction-finality file was similarly migrated
    to the new error handling mechanisms.
    4. A dependency to the cactus-core package was added for the easier handling
    of HTTP specific errors. The http-errors-enhanced-cjs package contains
    useful shorthands for HTTP-aware error handling and can be used in common
    JS environments instead of being constrainted to ESM only like the original
    library.

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
        Created At 2024-01-16 16:19:22 +0000 UTC
    </div>
</div>

