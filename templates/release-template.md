---
layout: default
title: {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Releases
has_children: false
permalink: /releases/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}}

You can clone this repo on <span class="fs-3">[GitHub]({{.Repository.Link}}){: .btn .mr-4 }</span>

{{range .Releases}}
<div class="code-example" markdown="1">
    <table>
        <tr>
            <td colspan="2">
                {{.Name}}
            </td>
        </tr>
        <tr>
            <td>
                {{.TagName}}{: .label-grey }
            </td>
            <td>
                {{.Body}}
            </td>
        </tr>
    </table>
    [View on GitHub]({{.URL}}){: .btn }
    <span class="right-align">
        Created At {{.CreatedAt}}
    </span>
</div>
{{end}}
