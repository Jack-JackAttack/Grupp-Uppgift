



## Miljö
- **Python:** 3.13.7
- **Paket:** `Pandas`, `Numpy`, `Matplotlib`, `Seaborn`, `Scikit-learn` (se `requirements.txt`)
 
## Kom igång
```bash
# klona projektet
git clone https://github.com/Jack-JackAttack/Grupp-Uppgift.git
 
# Skapa och aktivera virtuell moljö
python -m venv .venv
 
# installera beroenden
python -m pip install -r requirements.txt

```

## Kravkort
Digital marknadsplats med hög aktivitetsnivå
Viss mängd misstänkta annonser och meddelanden
Manuell granskning ineffektivt
Kravställning från Legal/Compliance:
- Förklarbarhet
- Spårbarhet
- Konsekvent beteende

## Strategi
Hitta en enkel förklarbar modell.
Syftet med modellen är att prioritera vilka annonser som ska granskas manuellt, inte att automatiskt fatta beslut om borttagning. Detta gör att modellen kan hjälpa granskningsteamet att fokusera på de annonser som har högst risk.
Legal/compliance vill inte att oskyldiga drabbas, dvs inte för mycket FP(falsklarm) därför väljer vi att optimera på precision. Det har dock funnits utrymme att ha en del FP eftersom det granskas manuellt. 
Vi vill halvera teamets arbetsbelastning. 

## Ansvarsfördelning
EDA - Jack
Train/test + preprocessing - Nadine
Modellering och jämförelse - Carina
Hyperparameter-tuning - Malin
Threshold / prioritering - (Jack, Nadine, Carina, Malin)
Deploy-test - (Jack, Nadine, Carina, Malin)