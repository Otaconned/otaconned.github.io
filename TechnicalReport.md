
## Dataset and Description 
The data is derived from the Internet Inclusivity Index, requisitioned by Facebook and developed by The Economist Intelligence Unit, looking at internet availability trends annually from 2017 to 2021. It polls 120 countries for four key metrics: accessibility, affordability, relevance, and readiness regarding internet integration.

## Preprocessing/Cleaning steps 
After obtaining an overview of the data, I dropped any columns which did not have to do with my specific story, including (while endlessly fascinating) largely irrelevant variables, such as ‘1.2.5) Average mobile download speed’ and ‘3.1.1) Availability of local news in local languages’. I narrowed the data down to the most important columns: 
Country

1.1.1) Internet users
1.1.4) Gender gap in internet access
1.1.5) Gender gap in mobile phone access
BG17) Internet access gender gap
BG18) Mobile phone access gender gap
BG20) Male internet users
BG21) Female internet users
BG22) Male mobile phone subscribers
BG23) Female mobile phone subscribers


And then those which could have relevance to the overall story, including:
4.1.1) Level of literacy
4.1.3) Support for digital literacy
4.3.1) National female e-inclusion policies
4.3.1.1) Comprehensive female e-inclusion plan
4.3.1.2) Female digital skills training plan
4.3.1.3) Female STEM education plan

From here, I scrubbed the data for nulls and duplicates. 

## Visualization/Design choices via [Colab](https://colab.research.google.com/drive/1N-Hrtrke-jF9KIw_QzSxQNPHxkf7Agx3?usp=sharing)
I chose three graphs: a heatmap, a bubble graph, and the traditional bar chart. 
The map was a relatively easy decision: it’s already built into Plotly Express, so it became a matter of passing the data to be visualized. I did, however, choose to use only a static snapshot in my final version (since dynamic visuals are a next-project piece), and I felt that my point was still being effectively communicated by the stark visuals. I do think the map loses some benefit by not being interactive, since specific data/details about the individual countries could’ve been interesting to the reader.

The bubble chart was more difficult — because I wanted to compare a number of major metrics against one another, I felt it would be the most effective for relaying a lot of data quickly. It posed some challenges through visualization, but I’m ultimately pleased with the clear trend visible. 

I was between a bar chart and a pie chart for the final graph, but I felt that the simplicity of dividing the policy variable into two simple columns was more straightforward and created a more stark, hard-hitting contrast.

## Reflection
Over the course of this project, I undertook a number of learning challenges — using MatPlotLib, a library I am a novice at, in tandem with Plotly (Express) and the migration to Colab as compared to my more-familiar Jupyter environment. I think they were a benefit to my overall growth and learning — I had a lot of stumbling blocks when it came to Plotly in specific, but found that more research actually helped to prepare me for the upcoming second project.
