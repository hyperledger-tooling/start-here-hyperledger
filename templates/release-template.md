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
<div>
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
<span class="chip">
{{.TagName}}
</span>
            </td>
            <td>
                {{.Body}}
            </td>
        </tr>
    </table>
<a href="{{.HTMLURL}}" class=".btn">
View on GitHub
</a>
    <span class="right-align">
        Created At {{.CreatedAt}}
    </span>
</div>
{{end}}
