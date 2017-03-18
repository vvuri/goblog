+++
Description = ""
menu = "main"
date = "2017-03-18T12:22:39+03:00"
title = "Map posts"
Categories = ["Development","GoLang"]
Tags = ["Development","golang"]

+++

{{ partial "header.html" . }}
	<main>
        {{ .Content }}
        {{ range .Paginator.Pages }}
			{{ partial "summary.html" . }}
		{{ end }}
		{{ partial "pagination.html" . }}
	</main>
{{ partial "sidebar.html" . }}
{{ partial "footer.html" . }}
