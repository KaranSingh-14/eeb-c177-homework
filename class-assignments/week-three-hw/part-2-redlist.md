

Part 2 

1. `tail -n +2 European_Red_List.csv | cut -d "," -f 10 | sort | uniq -c`

Output 
```
    456 CR
      8 CR (PE)
   2409 DD
    687 EN
      4 EW
     29 EX
   5805 LC
    411 NA
      4 NE
    964 NT
      8 RE
    885 VU
```

2. `tail -n +2 European_Red_List.csv | cut -d "," -f 4,10 | grep AVES | sort | uniq -c`

Output
```
     10 AVES,CR
     18 AVES,EN
      2 AVES,EX
    428 AVES,LC
     32 AVES,NT
      4 AVES,RE
     39 AVES,VU
```

3. `tail -n +2 European_Red_List.csv | cut -d "," -f 4,5,10 | grep AVES | sort | uniq -c | grep -w -E "EX|CE|RE"`

Output
```
      
      2 AVES,CHARADRIIFORMES,EX
      1 AVES,CHARADRIIFORMES,RE
      1 AVES,PASSERIFORMES,RE
      1 AVES,PELECANIFORMES,RE
      1 AVES,SULIFORMES,RE
```



