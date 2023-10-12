# Esami
```dataview
table without id file.link as esame, modulo, progresso, data, voto
from "200/esami"
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
table without id file.link as modulo, esame
from "Moduli"
where superato
```

# Citazioni

# Appunti