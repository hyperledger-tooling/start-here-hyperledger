---
layout: default
title: {{.Repository.Name}}
parent: {{.Organization.Name}}
grand_parent: Releases
has_children: false
permalink: /releases/{{.Organization.Github}}/{{.Repository.Name}}
---

# {{.Repository.Name}} <span class="fs-3 right-align">[GitHub]({{.Repository.Link}}){: .btn .mr-4 }</span>

{{range .Releases}}
<div markdown="1">
    <table>
        <tr>
            <td colspan="2">
                <b>
                    {{.Name}}
                </b>
            </td>
        </tr>
        <tr>
            <td>
{{.TagName}}
{: .label-grey }
            </td>
            <td>
                {{.Body}}
            </td>
        </tr>
    </table>
[View on GitHub]({{.HTMLURL}}){: .btn }
    <span class="right-align">
        Created At {{.CreatedAt}}
    </span>
</div>
{{end}}
