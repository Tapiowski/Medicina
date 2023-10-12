---
limit: 100
mapWithTag: false
icon: alarm-minus
tagNames: 
excludes: 
extends: 
version: 3
---
class:: {"type":"Select","options":{"valuesList":{},"sourceType":"ValuesFromDVQuery","valuesListNotePath":"","valuesFromDVQuery":"dv.pages('\"100/classe\"').map(p => p.file.name)"}}
modulo:: {"type":"Select","options":{"valuesList":{},"sourceType":"ValuesFromDVQuery","valuesListNotePath":"","valuesFromDVQuery":"dv.pages('\"Moduli\"').map(p => p.file.name)"}}

data:: {"type":"Date","options":{"dateFormat":"HH:mm DD/MM/YYYY","defaultInsertAsLink":"false"}}

professore:: {"type":"Input","options":{}}