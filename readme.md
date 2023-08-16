
# pokemon-py

pokemon-py is a Python wrapper for PokeAPI (https://pokeapi.co)



## Installation

Install my-project with pip

```bash
  pip install pokemon-py
```
    
## Setup

Using Pokemon-Py is simple, we start by importing the modules we want
```python
from pokepy import Pokemon
from pokepy import Move
from pokepy import Ability
```

Then we create an instance of the Pokemon class
```python
p = Pokemon()
m = Move()
a = Ability()
```

From now on we can use those instances to call the functions



## Examples

**get_sprites**
```python
p.get_sprites(1)
```
This returns a dictionary with the sprites of the Pokemon.
```python

"back_default": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/back/1.png",
"back_female": None,
"back_shiny": "https://raw.githubusercontent.com/PokeAPI/sprites/master/sprites/pokemon/back/shiny/1.png",
"back_shiny_female": None,
...
```

**get_battle_info**
```python
print(m.get_battle_info(4))
```

This returns a dictionary with important battle information

```python
{
    "name": "fire-punch",
    "accuracy": 100,
    "power": 75,
    "pp": 15,
    "priority": 0,
    "type": "fire",
    "damage_class": "physical",
    "effect_chance": 10,
    "effect_entry": "Has a $effect_chance% chance to burn the target.",
}
```

**get_pokemon_can_have_ability**
```python
print(a.get_pokemon_can_have_ability(1))
```

This returns a list with all the pokemon that can have that ability

```python
['gloom', 'grimer', 'muk', 'koffing', 'weezing', 'stunky', 'skuntank', 'trubbish', 'garbodor', 'garbodor-gmax']
```



## Packages

```python
requests
```



## Contact
**E-mail**: rick89@gmail.com

**Github**: https://github.com/RickVerbon
