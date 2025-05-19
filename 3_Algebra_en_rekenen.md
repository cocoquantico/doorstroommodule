---
kernelspec:
  name: python3
  display_name: 'Python 3'
numbering:
  headings:
    enabled: true 
---

# Blok 1 Algebra en rekenen

```{note}
In dit blok gaan we rekenen met breuken en letters. Als je straks in de 11e zit, ga je merken dat je dit bij veel onderwerpen moet toepassen.
```

```{code-cell} ipython3
import ipywidgets as widgets
from IPython.display import display, clear_output

vraag = widgets.Text(
    value='',
    placeholder='Typ je antwoord',
    description='Antwoord:',
    disabled=False
)
uitvoer = widgets.Output()

def check_antwoord(change):
    with uitvoer:
        clear_output()
        if change['new'].strip() == "42":
            print("Goed gedaan!")
        elif change['new'] != "":
            print("Helaas, probeer het opnieuw.")

vraag.observe(check_antwoord, names='value')
display(vraag, uitvoer)
```
