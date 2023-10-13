---
limit: 100
mapWithTag: false
icon: alarm-clock
tagNames: 
excludes: 
extends: 
version: 1
---
class:: {"type":"Select","options":{"valuesList":{},"sourceType":"ValuesFromDVQuery","valuesListNotePath":"","valuesFromDVQuery":"dv.pages('\"100/classe\"').map(p => p.file.name)"}}
modulo:: {"type":"Select","options":{"valuesList":{},"sourceType":"ValuesFromDVQuery","valuesListNotePath":"","valuesFromDVQuery":"dv.pages('\"Moduli\"').map(p => p.file.name)"}}
progresso:: {"type":"Date","options":{"dateFormat":"DD/MM/YYYY","defaultInsertAsLink":"false","dateShiftInterval":"7 days"}}
data:: {"type":"Date","options":{"dateFormat":"HH:mm DD/MM/YYYY","defaultInsertAsLink":"false"}}

valutazione:: {"type":"Number","options":{"min":"0","max":"30"}}