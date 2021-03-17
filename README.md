# DomesticFlightsAnalysis


### Introduction:
This is a dataset on Airline On-Time Statistics and Delay Causes.
The U.S. Department of Transportation's (DOT) Bureau of Transportation Statistics (BTS) tracks the on-time performance of domestic flights operated by large air carriers. Summary information on the number of on-time, delayed, canceled and diverted flights appears in DOT's monthly Air Travel Consumer Report, published about 30 days after the month's end, as well as in summary tables posted on this website. BTS began collecting details on the causes of flight delays in June 2003. Summary statistics and raw data are made available to the public at the time the Air Travel Consumer Report is released.

It includes 1493 entries. 16 domestic carriers. All these entries are in November 2020

### Key Insights:
This dataset is a valuable source of very important data. I wrangled and cleaned it in order to gleam interesting and useful insights. I was interested in seeing how carriers stack against each other. What factors make a carrier good and what make a carrier bad. I also wanted to analyze how different factors affect each other, if at all.

The following are the insights I was able to garner:

Number of delayed flights per carrier:
- SkyWest Airlines Inc.     4132.0
- Delta Air Lines Inc.      3952.0
- American Airlines Inc.    3528.0
- Southwest Airlines Co.    2912.0
- Envoy Air                 1754.0
- United Air Lines Inc.     1715.0
- Republic Airline          1238.0
- Mesa Airlines Inc.        1238.0
- Spirit Air Lines          1164.0
- PSA Airlines Inc.         1132.0
- Alaska Airlines Inc.      1071.0
- JetBlue Airways           1065.0
- Endeavor Air Inc.         1013.0
- Allegiant Air              846.0
- Frontier Airlines Inc.     479.0
- Hawaiian Airlines Inc.     165.0

Most efficient carrier (lower is better) :
- Southwest Airlines Co.     4.145904
- Endeavor Air Inc.          4.805275
- Hawaiian Airlines Inc.     5.662320
- Frontier Airlines Inc.     6.451178
- Republic Airline           6.691530
- United Air Lines Inc.      7.099098
- Delta Air Lines Inc.       8.020294
- SkyWest Airlines Inc.      8.098626
- PSA Airlines Inc.          8.279696
- American Airlines Inc.     9.168399
- Spirit Air Lines           9.470344
- JetBlue Airways            9.918972
- Alaska Airlines Inc.       9.947984
- Envoy Air                 11.055783
- Mesa Airlines Inc.        11.250454
- Allegiant Air             12.198991

It turns out that **American Airlines** is the worst domestic carrier in America with the highest mean delay time. 52.4% of its delays are due to carrier itself. This could be due to bad management or other factors like logistics, for example.
Not only is American Airlines highest in mean delay time but the number of times its flights were delayed is mostly also because of them! 
In contrast, **Hawaiian Airlines Inc** is the best domestic carrier in America since it has the lowest mean delay time and is the most efficient airline. Its flights are seldom delayed in comparison and even if they are they are only delayed for a relatively shorter time.

In general, it is pretty clear to me that carrier delay is the main reason carriers arrive late followed by late aircrafts. Security delay barely plays a part in arrival delay. I think this is due to the fact that security incidents happen rarely at airports.

### Conclusion:
In conclusion, I wish I had data for more years and months so I could analyze which airlines improved the most and which did not over a longer period of times. I would like to note that I faced a problem with all the columns ending in 'ct'. They are float but should be integers since they are a count of certain incidents. I tried to type cast them at first into integer but that created inaccuracies since numbers below 0.5 were turned into zeros and that is something I do not want.
