# Log-Analysis

```
Try Hack Me "Advent of Cyber - 2023" Task 13 [Day 7] Log analysis ‘Tis the season for log chopping! 
```

*THM{     }*

```
cut -d ' ' -f2 access.log | sort | uniq -c | sort -n | wc -l
```

```
cut -d ' ' -f3 access.log | cut -d ':' -f1 | sort | uniq -c | sort -n | wc -l
```

```
cut -d ' ' -f3,6 access.log | grep partnerservices.getmicrosoftkey.com
```

```
cut -d ' ' -f2,3 access.log | grep frostlings.bigbadstash.thm
```

```
grep frostlings.bigbadstash.thm access.log | cut -d ' ' -f5 | cut -d '=' -f2 | base64 -d
```
