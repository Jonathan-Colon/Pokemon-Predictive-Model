# POKEMON PREDICTIVE MODELING Project
### Using API, Kaggle datasets, and creating a similar battle model to pokemon, I attempted to create a predictive model via creation of composite scoring of 6-pokemon teams (synergy Scores)

# Program used
## Python via Spider and Google Collab 
### I pulled all data from pokeapi and coded equations that dictate similar patterns and damage to that of the pokemon franchise

## Currently, the best way I have found to create a predictive model for a team was create a synergy score that would be a quanitative expression encompassing things such as pokemon type and move type for coverage and bonus damage, as well as abilities and individualized stat distribution 
# Pokémon Predictive Model
This project builds a predictive model to analyze and forecast battle outcomes based on Pokémon stats, synergy scores, and team composition.
![Synergy Score Example](images/synergy.png)
#To evaluate best teams, I used K-means Clustering to catergorize what each type of pokemon fall under
![K-means Clustering for all known Pokemon](images/K-Means%20cluster.png)
## Example equation: Final damage calculation
### final_damage = base_damage * stab_multiplier * effectiveness * crit_multiplier * item_boost * random_factor


### This data is strictly for experimentation purposes and I do not receive, nor look to receive compensation from this data owned by any and all entities surround the Pokemon franchise.

## Dependencies

This project uses the following Python libraries:

- **pandas** – data cleaning, manipulation, and analysis  
- **numpy** – numerical operations and arrays  
- **matplotlib** – plotting and visualizations  
- **seaborn** – enhanced data visualizations (optional)  
- **scikit-learn** – clustering and predictive modeling  
- **requests** – retrieving data from the PokéAPI  
- **json** – parsing API responses  
- **itertools** – generating team combinations  
- **random** – randomizing team selection  

### Installation


## Below is an example of how I ran an inital process for finding the simulation
## Quick Simulation: Enter a Pokémon and Run

Use one of the options below to enter a Pokémon’s stats and run a test simulation.

> **What you’ll need:**  
> - Base stats (HP, Atk, Def, SpA, SpD, Spe)  
> - Types, Ability, and up to 4 Moves  
> - (Optional) Level, Nature, EVs/IVs if your model uses them

---

### Running initial dashboard — Console / Spyder (simple prompts)

```python
# Paste into a Python file or cell and run

def prompt_pokemon():
    print("Enter Pokémon info ↓")
    mon = {
        "name": input("Name (e.g., Garchomp): ").strip(),
        "type1": input("Type 1 (e.g., dragon): ").strip().lower(),
        "type2": input("Type 2 (or blank): ").strip().lower() or None,
        "ability": input("Ability (e.g., rough-skin): ").strip(),
        "hp": int(input("HP: ")),
        "atk": int(input("Attack: ")),
        "def": int(input("Defense: ")),
        "spa": int(input("Sp. Atk: ")),
        "spd": int(input("Sp. Def: ")),
        "spe": int(input("Speed: ")),
        "moves": [m.strip

To install the required dependencies, run:

```bash
pip install pandas numpy matplotlib seaborn scikit-learn requests
pip install notebook ipywidgets
```
# Current Dashboard Appearance
![Head-to-Head Visualization](images/Head_to_head.png)
