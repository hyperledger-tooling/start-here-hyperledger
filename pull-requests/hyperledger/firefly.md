---
layout: default
title: firefly
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly
---

# firefly <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/774" class=".btn">#774</a>
            </td>
            <td>
                <b>
                    Add E2E test for contract APIs and fix postgres migration
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR fixes a PostgreSQL migration issue and adds an additional E2E test to cover that scenario
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-27 17:17:38 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/772" class=".btn">#772</a>
            </td>
            <td>
                <b>
                    Update manifest.json for v1.0.0
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Nicko Guyer <nicko.guyer@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 19:12:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/771" class=".btn">#771</a>
            </td>
            <td>
                <b>
                    [ui-v1.0.0] manifest
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: David Echelberger <eberger727@gmail.com>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 15:35:46 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/770" class=".btn">#770</a>
            </td>
            <td>
                <b>
                    Omit "connector" from token transfer/approval inputs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This should always be inferred from the token pool.

Fixes #768
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 14:39:44 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/769" class=".btn">#769</a>
            </td>
            <td>
                <b>
                    Add prefix for signer
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Signed-off-by: Peter Broadhurst <peter.broadhurst@kaleido.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-26 01:26:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/767" class=".btn">#767</a>
            </td>
            <td>
                <b>
                    Update architecture diagram to include OpenAPI generator and fix link
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                I noticed a dead link when you click the image before, because it was pointing at a branch.

Also tweaked the diagram to make the OpenAPI generator for custom smart contracts more visible.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 21:10:16 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/766" class=".btn">#766</a>
            </td>
            <td>
                <b>
                    "decimals" is not a valid input
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This is currently a read-only field.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 20:16:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/765" class=".btn">#765</a>
            </td>
            <td>
                <b>
                    add additional event enrichment
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                 - TokenPoolOpFailed
 - BlockchainInvokeOpSucceeded
 - BlockchainInvokeOpFailed

closes #736 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 20:13:11 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/764" class=".btn">#764</a>
            </td>
            <td>
                <b>
                    Add change events to operations, by adding namespace to ResolveOperation
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Supersedes #739
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:58:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/763" class=".btn">#763</a>
            </td>
            <td>
                <b>
                    Version Command
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Closes #132, resurrects #586. Uses new preferred way of versioning with module fields in the `cmd` package rather than an `internal` package, see https://github.com/hyperledger/firefly-cli/pull/164 for original implementation of this approach.

Example "default" usage:
```
make build
./firefly version
{
  "Version": "(devel)",
  "Date": "2022-04-25T19:52:28Z",
  "License": "Apache-2.0"
}

./firefly version -o yaml
Date: "2022-04-25T19:52:28Z"
License: Apache-2.0
Version: (devel)

./firefly version --short
(devel)

make docker
docker run -it --entrypoint /bin/sh hyperledger/firefly
/firefly # firefly version
{
  "Version": "(devel)",
  "Date": "2022-04-25T19:45:02Z",
  "License": "Apache-2.0"
}
/firefly # firefly version -o yaml
Date: "2022-04-25T19:45:02Z"
License: Apache-2.0
Version: (devel)

/firefly # firefly version --short
(devel)

```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:49:17 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/762" class=".btn">#762</a>
            </td>
            <td>
                <b>
                    Fill in blockchain TX ID for contract listener events
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #761
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:35:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/760" class=".btn">#760</a>
            </td>
            <td>
                <b>
                    remove rocketchat from docs
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ✂️ 

closes #757 
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:09:25 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/759" class=".btn">#759</a>
            </td>
            <td>
                <b>
                    Token approvals should return empty array instead of nil
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #758
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-25 19:01:04 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/755" class=".btn">#755</a>
            </td>
            <td>
                <b>
                    Firefly E2E Test updates
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                - Refactor tests to specify a Firefly namespace to run tests against 
- Create namespace test suite to use without identity tests 
- Fix string comparison in objectCheck
- Remove TestE2EContractEvents() test 
- Set pool name to random int instead of using len - len causes issues when completing more than 25 test runs on the same stack and will always make the poolname pool26
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-22 20:00:29 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/752" class=".btn">#752</a>
            </td>
            <td>
                <b>
                    Remove server-side HTML sanitization of error messages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Errors may be displayed or used in many contexts. If they are displayed in HTML,
it should be the responsibility of the HTML client to sanitize them. Doing the
sanitization server-side makes the messages less readable in all non-HTML
contexts.

I want to be conscious about XSS and security, but I'd say that doing
an HTML-escaping pass on these errors before writing them to the database
is putting the processing in the wrong place. Characters such as `<` and `"`
become much less readable when they're converted to HTML entities.

And arguably this encourages bad design on an HTML client - as the client page would have
to pipe the values into the HTML _without_ sanitizing them client-side, in order
to have the HTML entities render back into readable characters.

One good discussion of this (anti-)pattern:
https://security.stackexchange.com/questions/42498/which-is-the-best-way-to-sanitize-user-input-in-php/42521#42521

Also see https://github.com/hyperledger/firefly/issues/753
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 19:07:50 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/751" class=".btn">#751</a>
            </td>
            <td>
                <b>
                    Add first step of FireFly Transaction Manager support - separate URL for submit
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
        Created At 2022-04-21 18:59:19 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/750" class=".btn">#750</a>
            </td>
            <td>
                <b>
                    Rename docs pages for better hierarchy
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This PR renames some of the files in the subdirectories of the docs site. It improves the page hierarchy, but it does run the risk of breaking some existing links that we may have.

For example:
https://hyperledger.github.io/firefly/gettingstarted/gettingstarted.html
Becomes:
https://hyperledger.github.io/firefly/gettingstarted

This also fixes the links on the main page that are currently broken, because they used relative links to directories, and there was no index.html file in those directories previously.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 17:17:00 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/749" class=".btn">#749</a>
            </td>
            <td>
                <b>
                    Misc cleanup for contract listeners
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
        Created At 2022-04-21 14:56:39 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/748" class=".btn">#748</a>
            </td>
            <td>
                <b>
                    Format JSON errors from connectors
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                ```
Parse a JSON error of the form:
  {"error": "Bad Request", "message": "Field 'x' is required"}
into a message of the form:
  "Bad Request: Field 'x' is required"
```

See https://github.com/hyperledger/firefly/issues/753
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-21 01:04:57 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/747" class=".btn">#747</a>
            </td>
            <td>
                <b>
                    Add table name to debug on every SQL call
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Currently we take the first three words of the SQL to try and provide a debug statement that's useful, without printing the massive bundle of SQL. However, that is insufficient as for something like `SELECT` it just contains the first two fields from the select.

This PR introduces an explicit table name being passed on every call and put in the logs.

I did find what I think was one bug where `GetContractAPIs` was using the `contract_interfaces` table
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 21:44:55 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly/pull/746" class=".btn">#746</a>
            </td>
            <td>
                <b>
                    Resolve pool activation operations more cleanly
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Fixes #743
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2022-04-20 20:26:09 +0000 UTC
    </div>
</div>

