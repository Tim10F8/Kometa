---
hide:
  - toc
---
{%
    include-markdown "./../../templates/defaults/country.md"
    replace='{
        "LIBRARY_TYPE": "Movie",
        "FULL_TYPE": "Movies",
        "SHORT_TYPE": "movie",
        "DYNAMIC_VALUE": "Countries"
    }'
    replace-tags='{"title-sub": "**[This file has a Show Library Counterpart.](./../../show/country)**"}'
    rewrite-relative-urls=false
%}

    === "Default `include`"
    
        {% include-markdown "../../templates/snippets/no-copy.md" rewrite-relative-urls=false %}
        include: 
    {%    
      include-markdown "../../../defaults/movie/country.yml" 
      comments=false
      start="include:\n"
      end="addons:"
    %}
        ```

    === "Default `addons`"
    
        {% include-markdown "../../templates/snippets/no-copy.md" rewrite-relative-urls=false %}
        addons: 
    {%    
      include-markdown "../../../defaults/movie/country.yml" 
      comments=false
      start="addons:\n"
    %}
        ```
