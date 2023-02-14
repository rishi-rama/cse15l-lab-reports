# Grep Command-Line Options
## grep -i
The -i command makes the grep search case insensitive, which can be useful because a case sensitive search can miss some matches.
Source: https://en.wikibooks.org/wiki/Grep
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
Source: https://man7.org/linux/man-pages/man1/grep.1.html
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
## grep -n
The -n adds a prefix to every output line containing its line number. This can be useful if you want to find where an output occurred in a large document.
Source: https://man7.org/linux/man-pages/man1/grep.1.html
```
# Example 1: Input
grep -n "South Coast" written_2/travel_guides/berlitz2/Bermuda-WhereToGo.txt
```
```
# Example 1: Output
78:The South Coast to Castle Harbour
```
```
# Example 2: Input
grep -n "Yosemite" written_2/travel_guides/berlitz2/California-WhereToGo.txt
```
```
# Example 2: Output
149:If California’s great outdoors is a religion, then its cathedrals are found in the Yosemite and Sequoia and Kings Canyon national parks, as well as the Death Valley National Park. In these magnificent stretches of wilderness — the mountains of the Sierra Nevada, the huge, silent redwood forests, and the awe-inspiring emptiness of the desert — you can begin to recapture the adventurous spirit of the earliest American experience. These parks are, naturally, immensely popular with Californians and tourists alike, Yosemite more so than the others, but they all have ample room for everyone to escape the crowds.
152:Yosemite National Park
153:The scenic Yosemite Valley is a perfect example of a glacier-carved canyon, with its sheer granite walls 3,200ft (975m) high plunging to a flat floor of woods and wild-flower meadows, enclosing the waters of the Merced River. Your “base camp” could be a plush hotel room, more modest lodge accommodation, or even just a tent. From the valley meadows you can hike, bike (rentals at Yosemite Lodge or Curry Village), or take the shuttle bus to all the principal sights.
157:You can see Yosemite Creek drop down half a mile from the opposite wall in the spectacular Upper, Middle, and Lower Yosemite Falls, and you’ll get an outstanding view of the majestic Half Dome, a granite monolith sliced in two by the Ice Age glaciers. From here you may feel like leaving the bus and hiking back down to the valley, along the Panorama Trail via the Nevada and Vernal Falls, a trip of 8 miles (13 km), most of it downhill!
```

## grep -x
The -x command only outputs results where the entirety of the line matches
Source: https://linux.die.net/man/1/grep
```
# Example 1: Input
grep -x "Downtown" written_2/travel_guides/berlitz2/California-WhereToGo.txt
```
```
# Example 1: Output
Downtown
Downtown
```
```
# Example 2: Input
grep -x "Sanur" written_2/travel_guides/berlitz2/Bali-WhereToGo.txt
```
```
# Example 2: Output
Sanur
```
