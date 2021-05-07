---
layout: default
title: grid
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/grid
---

# grid <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/grid){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/680" class=".btn">#680</a>
            </td>
            <td>
                <b>
                    Fix clippy lint introduced in rust 1.52
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-07 16:36:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/679" class=".btn">#679</a>
            </td>
            <td>
                <b>
                    Remove deprecated form components
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes deprecated form components for adding, editing, and deleting products. These components will be updated in the near future to match the new grid styles. The Product sapling will be released with read-only features for Grid v0.2. This depends on PR #649
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 17:42:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/678" class=".btn">#678</a>
            </td>
            <td>
                <b>
                    Improve validation error reporting
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The rust-libxml bindings library did not handle validation errors properly. Instead of reporting all of the validation errors for a file, the library would return the correct number of errors but all of the error messages would be the same. This issue seems to be due to the implementation of the StructuredError handler in the rust-libxml bindings library.

This PR removes the bindings library and just implements bindings for the specific libxml2 functions needed for validation.

This PR also moves the validation step to after the XML files have been parsed so that parsing errors can be reported before validation.

Example output:

```
$ grid product create --owner crgl --file .myfiles/valid_example.xml --file .myfiles/invalid_example.xml 
Entity: line 10: Schemas validity error : Element 'isTradeItemAnInvoiceUnit': 'ERROR' is not a valid value of the atomic type 'xs:boolean'.
Entity: line 11: Schemas validity error : Element 'isTradeItemAnOrderableUnit': 'ERROR' is not a valid value of the atomic type 'xs:boolean'.
Error: File fails to validate (.myfiles/invalid_example.xml)
```

Implementation was inspired by [FranklinChen/validate-xml-rust](https://github.com/FranklinChen/validate-xml-rust) and [xmllint](https://github.com/GNOME/libxml2/blob/master/xmllint.c)

            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-06 03:32:52 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/660" class=".btn">#660</a>
            </td>
            <td>
                <b>
                    Remove unsupported Memory Store impls
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This removes now-unsupported MemoryStore implementations for the
commits and schemas stores. The memory store implementations were
deprecated in favor of an in-memory sqlite implementation but it looks
like a couple of the modules' implementations didn't get cleaned up.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:36:13 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/659" class=".btn">#659</a>
            </td>
            <td>
                <b>
                    Replace specific store errors with standard ones
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This replaces the StoreFactoryCreationError and ParseConnectionUriErrors
with the standard Grid InternalError type. This is more in line with the
approach used across the rest of the SDK.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:29:31 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/658" class=".btn">#658</a>
            </td>
            <td>
                <b>
                    Make all operations atomic
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This makes all operations atomic. Previously, this was done in a sort of
piecemeal fashion. This just cleans this up and makes sure all
operations are wrapped in the generic diesel transaction. This is
available for all Diesel backends that implement Diesel::Connection.
This depends on PR #656.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:27:49 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/657" class=".btn">#657</a>
            </td>
            <td>
                <b>
                    Update PurchaseOrderStore feature guard
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This updates the DieselPurchaseOrderStore feature to be guarded by the
`diesel` feature rather than the `postgres` feature. This brings the
module in line with the other Grid data stores. This is part of stabilizing the
postgres and sqlite features.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:23:32 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/656" class=".btn">#656</a>
            </td>
            <td>
                <b>
                    Rename `fetch_` operations to `get_`
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                This renames the `fetch_` operations to `get_` operations. This brings
the Grid data store operation in line with the naming conventions used
in Splinter. This is part of stabilizing the postgres and sqlite features.

Signed-off-by: Davey Newhall <newhall@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-03 16:19:31 +0000 UTC
    </div>
</div>

