---
layout: default
title: firefly-common
parent: Hyperledger
grand_parent: Pull Requests
has_children: false
permalink: /pull-requests/hyperledger/firefly-common
---

# firefly-common <span class="fs-3 right-align">[GitHub](https://github.com/hyperledger/firefly-common){: .btn .mr-4 }</span>


<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/113" class=".btn">#113</a>
            </td>
            <td>
                <b>
                    Add JSON serialization of filters for building more complex queries
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                The URL query parameter spelling is designed to be convenient for simple cases, but it gets awkward with complex cases.

This PR proposes a JSON payload format and a utility to convert that into a runtime filter.

There are loads of ways this could be spelt (and many contrasting examples out there from other projects), with various compromises... the one I picked in this proposal was mainly for ease of implementation with our existing filtering code.

Some of the most significant choices/characteristics:

- Operators are the parent, values and modifiers are the children:
    - ... so `tag != 'abc'` is spelt `equal: [{not: true, field: "tag", value: "abc"}]`
- Field names are always in a `field` property - never a key name
- Operator -> array of matches semantics (makes it very easy to parse in Go strong typing)
- `AND` combination is the standard for all operator arrays, and when multiple operators used
- `OR` has to be specified explicitly, and the containing entries are all implicit `AND` (although singulars are optimized out)

### Example (from test)

```js
{
	"skip": 5,
	"limit": 10,
	"sort": [
		"tag",
		"-sequence"
	],
	"equal": [
		{
			"field": "tag",
			"value": "a"
		}
	],
	"greaterThan": [
		{
			"field": "sequence",
			"value": 10
		}
	],
	"or": [
		{
			"equal": [
				{
					"field": "masked",
					"value": true
				}
			],
			"in": [
				{
					"field": "tag",
					"values": [
						"a",
						"b",
						"c"
					]
				}
			]
		},
		{
			"equal": [
				{
					"field": "masked",
					"value": false
				}
			]
		}
	]
}
```

### The AND/OR this results in

```
(
  tag == 'a'
)
AND
(
  sequence >> 10
)
AND
(
  (
    (
      masked == true
    )
    AND
    (
      tag IN ['a','b','c']
    )
  )
  OR
  (
    masked == false
  )
)
sort=tag,-sequence skip=5 limit=10
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-12-03 05:27:48 +0000 UTC
    </div>
</div>

<div>
    <table>
        <tr>
            <td>
                PR <a href="https://github.com/hyperledger/firefly-common/pull/112" class=".btn">#112</a>
            </td>
            <td>
                <b>
                    Fix docs regression in parameter descriptions that changes swagger gen
                </b>
            </td>
        </tr>
        <tr>
            <td>
                
            </td>
            <td>
                We're incorrectly adding a `[0]` to these messages after #107:

```
description: 'The maximum number of records to return (max: [0])'
                                                            ^^^
```
            </td>
        </tr>
    </table>
    <div class="right-align">
        Created At 2023-11-29 16:26:32 +0000 UTC
    </div>
</div>

