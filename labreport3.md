# Grep Command-Line Options
## grep -i
The -i command makes the grep search case insensitive, which can be useful because a case sensitive search can miss some matches.
```
# Example 1: Input
grep -i "outrigger" written_2/travel_guides/berlitz1/HandRHawaii.txt
```
```
# Example 1: Output
Outrigger Reef $$$ 2169 Kalia Road, Honolulu, HI 96815; Tel.
<www.outrigger.com>. This 17-story tower, perched on one of the
Outrigger and related Ohana hotels. Its rooms, views, and amenities
Outrigger Wailea Resort $$$–$$$$ 3700 Wailea Alanui,
622-4852; <www.outrigger.com>. This 22-acre oceanfront resort,
Outrigger Waikoloa Beach $$$ 69-275 Waikoloa Beach Drive,
886-7852; <www.outrigger.com>. Renovated in 2000, this
```
```
# Example 2: Input
grep -i "football" written_2/travel_guides/berlitz2/Amsterdam-WhatToDo.txt
```
```
# Example 2: Output
Football (Soccer)
The Netherlands are football (soccer) crazy and Ajax is the Amsterdam team, one of the most successful in Europe over the last 30 years. They play at the Amsterdam Arena, a fine modern stadium, which is also used for other sporting events — but unfortunately it is almost impossible to obtain tickets for matches.
```
As we can see, without the -i option some of the results would be omitted. 
## grep -c
The -c command outputs a count of the number of matching lines. This is useful because it can tell you how many times a string occurs in a file.
```
# Example 1: Input
grep -c "Aegean" written_2/travel_guides/berlitz1/IntroGreek.txt
```
```
# Example 1: Output
7
```
```
# Example 2: Input
grep -c "Nile" written_2/travel_guides/berlitz1/IntroEgypt.txt
```
```
# Example 2: Output
2
```
