```
cut -f1 file| sort -u | wc -l # file no of unique row
awk -F ',' '{print $1}' file| wc -l #split file using , then find no of row in column 1 
awk -F ',' '{print $1}' file| sort -u | wc -l #split file using , then find no of unique row in column 1
```
