Title:: {{title}}
URL: {{url}}
Zotero Link: {{pdfZoteroLink}}
Author: {{authors}}{{directors}}
Year:  {{date | format("YYYY")}}

{% for annotation in annotations -%} 
    {%- if annotation.annotatedText -%} 
    {{annotation.annotatedText}}”{% if annotation.color %} {{annotation.colorCategory}} {{annotation.type | capitalize}} {% else %} {{annotation.type | capitalize}} {% endif %}[Page {{annotation.page}}](zotero://open-pdf/library/items/{{annotation.attachment.itemKey}}?page={{annotation.page}}&annotation={{annotation.id}}) 
    {%- endif %} 
    {%- if annotation.imageRelativePath -%}
    ![[{{annotation.imageRelativePath}}]] {%- endif %} 
{% if annotation.comment %} 
{{annotation.comment}} 
{% endif %} 
{% endfor -%}