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
                PR <a href="https://github.com/hyperledger/grid/pull/684" class=".btn">#684</a>
            </td>
            <td>
                <b>
                    Update product man pages
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                Add explaination of `--xml` option for `grid product create` man page

Remove `--owner` option from `grid product update` man page

Signed-off-by: Ryan Banks <rbanks@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 17:27:36 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/683" class=".btn">#683</a>
            </td>
            <td>
                <b>
                    Fix Rust 1.52 lints
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
        Created At 2021-05-10 16:37:18 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/682" class=".btn">#682</a>
            </td>
            <td>
                <b>
                    Fix lint and dependency
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The Batch Processor constructor was merged after this lint was fixed elsewhere in Grid. Also updates saplingjs to get the dependency from the proper branch.
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 16:14:09 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/grid/pull/681" class=".btn">#681</a>
            </td>
            <td>
                <b>
                    Update Saplingjs dependency to correct branch
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The default branch was recently changed to main.

Signed-off-by: Ryan Beck-Buysse <rbuysse@bitwise.io>
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2021-05-10 14:40:14 +0000 UTC
    </div>
</div>

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

