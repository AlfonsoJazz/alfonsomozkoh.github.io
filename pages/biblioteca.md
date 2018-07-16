---
title: Biblioteca personal
permalink: "/biblioteca/"
layout: page
feature-img: assets/img/pexels/biblioteca.png
tags:
- Biblioteca
- PDF
- Recursos informáticos
- Libros gratis
---
<input type="text" id="search-input" placeholder="Palabras clave..." class="search-bar">
<br>
<br>
<ul id="results-container"></ul>

<section>
    <!-- Script pointing to jekyll-search.js -->
    <script src="{{ site.baseurl }}/assets/js/vendor/simple-jekyll-search.min.js" type="text/javascript"></script>

    <script type="text/javascript">
        SimpleJekyllSearch({
            searchInput: document.getElementById('search-input'),
            resultsContainer: document.getElementById('results-container'),
            json: '{{ site.baseurl }}/assets/data/search.json',
            searchResultTemplate: '<div class="search-title"><a href="{url}"><h3> {title}</h3></a><div class="meta">{date} <div class="right"><i class="fa fa-tag"></i> {tags}</div></div><p>{excerpt}</p></div><hr> ',
            noResultsText: 'No results found',
            limit: 10,
            fuzzy: false,
            exclude: []
        })
    </script>
</section>