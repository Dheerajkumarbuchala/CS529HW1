Firstly I concentrated on Whitehat.js code -> the code concentrates on drawing the map. But I have gone through the code and completed all the TODO's specified in the coede.
1) changed the maxRadius (changed the denominator to 50, initial value was 100)
2) changed the colormap based on colorbrewer2
   Made the map colorblind friendly
   changed the getEncodedFeature to (population/count) but the html used by the tooltip will also change as the function will be called and the values will change.
3) Made optional change -> added tooltip, added stroke (so that the boundary will highlight) and changed stroke-width to 1.
4) Changed the city marker being used, changed d3.scaleLinear to d3.scaleSqrt
5) Added the code to plot cityData, the cities are plotting in Green and when the mouse was hovered on the city then the city data will be
   displayed. If the mouse was hover on the empty areas then tooltip will display the data of the state by default.
6) I made a optional change to the array which is related to the scale shown beside the map. The scale is not in a sorted order as I changed
   the values in the code.
7) I did changed the code such that when we hover over the state, the state slightly comes up. But I didn't like it as the state will respond
   to the mouseover but the cities in that state remains on the map.

The main concentration and a lot of work went into coding the WhiteHatStats.js.
1) I changed the entire plot. I think a bar graph will be a good representation unlike the graph provided.
2) We cannot come to any conclusion from thed graph provided as the circles are overlapped and etc.
3) I choose to plot the bar graph.
4) I added options in HTML, and populated the options with the state names.
5) When 'ALL' is selected then the data represented in the bar graph will be the data from the map, i.e., Total gun deaths vs the state.
6) When a particular state is selected then a new bar graph will be plotted and displayed,
   the new plot will consist of male gun victims and female gun victims vs the mmonthYear data.
7) Tooltip was added so that when we hover over the graph that will display the male gun count and female gun count.


Finally, the reasons what makes the White-Hat visualization whiteHat is, I made the map colorBlind friendly, the main thing which really makes it whiteHat is the bar graph which is more informational and clear rather than the dot plot provided.

Sources:
StateMap : https://eric.clst.org/tech/usgeojson/
Original State Population : https://www.census.gov/data/tables/time-series/demo/popest/2010s-state-total.html
Original state gun violance dataset : https://www.slate.com/articles/news_and_politics/crime/2012/12/gun_death_tally_every_american_gun_death_since_newtown_sandy_hook_shooting.html
