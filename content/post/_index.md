+++
Categories = ["Development","GoLang"]
Tags = ["Development","golang"]
Description = ""
menu = "main"
date = "2017-03-17T23:27:56+03:00"
title = "Post"

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