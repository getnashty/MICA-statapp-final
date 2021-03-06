Working demo can be found here: http://statapp.ctodd.co/

#MICA: Statistical Applications for Data Visualization Final Project 

###Design process
Having created many visualizations in Excel, Illustrator, and R-Studio as well as High Charts [Example](http://canada.ctodd.co/) and Charts.js [Example](http://fatal.ctodd.co/), I wanted a bigger challenge. Sure I could have easily continued using those tools. However, I had my eyes set on something bigger. D3.js is a powerful JavaScript library that most serious data visualizers have in their toolbox, and I had never used it so this final presented a perfect opportunity. And a challenge it was. I'd rather attempt the triple axl and falter than nail a double. 

###Design philosophy
Simpler is better. Yes, I could have created many graphs with all that data but that defeats the purpose of design, which is to simplify and clarify. Communication needs to be clear, to the point, and not be confusing. There are types of visualizations that might be better for exploration. However, I wanted this to be an explanatory visualization. 

###Data 
Initially, I wanted to use my [city's open data portal](http://data.somervillema.gov), however upon digging deeper into the data, it turned out the 2011 Wellness Survey, one of the first in the country, had a data export that was corrupt. It was mildly amusing that halfway down the column of responses in the "How satisfied with your life are you?" household income data appeared. I came across Andy Kirk's [blog post](http://www.visualisingdata.com/index.php/2015/02/bank-englands-data-visualisation-competition/) announcing the recent [Bank of England Data Visualisation Challenge](http://www.bankofengland.co.uk/research/Pages/onebank/dataviscomp.aspx) and thought this could be interesting data to pursue. 

###Challenges with the data.. and D3
Thankfully the Bank of England data files was quite elegant, well marked and clean. From experience, this is a rare state to encounter, and the Somerville example is far more common. The challenges here were in two areas
1. Specifically _what_ to examine as there are over three centuries of data to explore. 
2. How to visually represent the data 

I overcame the first challenge through exploration of the data, quickly plotting a few things out in excel and ultimately settled on a difference line chart showing the import and export differences.  I found the GDP and trade data interesting, and it helped me put some of Britain's economic history into context. I wondered if I could accomplish this with one or two well-designed graphs. 

The challenges with how to represent the data soon turned into a "how-do-I-use-D3" exercise. In fact, the majority of the time spent on this assignment was learning how to work with the objects in D3. I found it incredibly frustrating, despite the vast array of available resources, to create _precisely_ the visual you want. In fact, I couldn't believe how many different ways I tried to create tool-tips or a brush-focus area and completely failed. (Seven different strategies to add tool-tips, and three different strategies to add brush and focus, not that I'm counting). I found D3 difficult to de-bug since the entire graph would disappear if the code broke, so determining exactly what went wrong was a challenge. 

###Future improvements
No work is ever truly "done," there are many enhancements to make this piece more engaging and interesting. Future enhancements could be:  
1. Mouseover tooltips that allow the viewer to see more annotations (yes, I know how you love annotations, Jon).  
2. On that note: Adding mini stories to each of the green or red shaded areas further explaining why there was either a surplus or a deficit. For example after World War I (1918), you see a decline in surplus and during World War II there is far more consumption (import) than export.  
3. A "brush and focus" section below the graph allowing the viewer to drag and zoom into different years.  
4. An interesting overlay might be adding in unemployment on top of this to see what, if any, relationship there was with the trade balance.   
5. Linking points on the timeline to news articles that discuss trade balance.  
6. An overlay of UK Government budge balance, positive or negative, might also be an interesting contrast.  
7. Allowing the user to choose which aspects to examine could be interesting as well.



