1. `tail -n +2 nobel.csv | cut -d "," -f 3 | grep chemistry | wc -l`

Output `181`

`tail -n +2 nobel.csv | cut -d "," -f 3 | grep physics | wc -l`

Output `210`

`tail -n +2 nobel.csv | cut -d "," -f 3 | grep peace | wc -l`

Output `133`

`tail -n +2 nobel.csv | cut -d "," -f 3 | grep economics | wc -l`

Output `81`


`tail -n +2 nobel.csv | cut -d "," -f 3 | grep medicine | wc -l`

Output ` 216`

`tail -n +2 nobel.csv | cut -d "," -f 3 | grep chemistry | wc -l`

Output `114`


2. ` tail -n +2 nobel.csv | cut -d "," -f 5-6 | sort | uniq -d`

Output 
```
"Comité international de la Croix Rouge (International Committee of the Red Cross)",NA
"Frederick","Sanger"
"John","Bardeen"
"Linus Carl","Pauling"
"Marie","Curie
"Office of the United Nations High Commissioner for Refugees (UNHCR)",NA
```

3. `tail -n +2 nobel.csv | cut -d "," -f 6 | sort | uniq -c | sort -g`

Output 
 
```5 "Smith"
     31 NA```
Smith was the most common surname

4. `tail -n +2 nobel.csv | cut -d "," -f3 | sort | uniq -c | sort -g`

Output 
``` 
    81 "economics"
    114 "literature"
    133 "peace"
    181 "chemistry"
    210 "physics"
    216 "medicine"
```


Sort g sorts it numerically which shows me the least and most abundant awards







