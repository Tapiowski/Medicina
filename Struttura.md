# Esami
```dataview
table without id file.link as esame, modulo, progresso, data
from "200/esami"
where !valutazione
```

# Studio
```dataview
task
group by file.link
```

# Moduli in corso
```dataview
table without id file.link as modulo, esame
from "Moduli"
where !superato
```

# Moduli superati
```dataview
table without id file.link as data, modulo, valutazione
from "200/esami"
where valutazione
```

# Orario
```dataview
table without id file.link as lezione, modulo, file.day - date("today") as "data"
from "200/lezioni"
where file.day > date("today")
```

# Lezioni
```dataview
table without id file.link as lezione, modulo, data
from "200/lezione"
where file.day < date("today")
limit 50
```

# Fonti
```dataview
table without id file.link as fonte, file.ctime as "Data"
from "Definizioni"
sort file.ctime desc
limit 50
```