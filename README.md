# UW-Madison SP22 ECE/CS/ISyE 524 — Introduction to Optimization
Final Project Repo

Team Members: Rayne Wolf, Zhaoxing (Bella) Wu

Professor Name: Line A. Roald

## Project Name
The Traveling Software Engineer

<p float="left">
  <img src="https://github.com/zwu363/UW-Madison-SP22-CS524/blob/main/figure/figure3.png" width="200" />
  <img src="https://github.com/zwu363/UW-Madison-SP22-CS524/blob/main/figure/figure4.png" width="200" /> 
  <img src="https://github.com/zwu363/UW-Madison-SP22-CS524/blob/main/figure/figure5.png" width="200" />
</p>

Figure: **Left**: The optimal flights to optimize cost and visit each region. **Middle**: The optimal flights to optimize time and visit each region. **Right**:The optimal flights to optimize cost & time and visit each city.

## Project Introduction
Epic, a healthcare software company located in Fitchburg, Wisconsin, would like to have one of its software developers visit their clients in major hospitals throughout the United States to discuss possible improvements and troubleshoot errors. Our group has been hired by Epic to create a model that would determine the options of travel along a predetermined network of possible flight paths to various cities across the US. This problem is modeled after the Traveling Salesman Problem; however, we renamed it to the Traveling Software Engineer Problem!

The Traveling Salesman Problem was first mathematically formulated in the 1930s by Merrill M. Flood. It was used to solve a school bus routing problem: minimizing the distance of the bus route while ensuring that all students were picked up (Flood, 1935). Our problem takes a similar approach, minimizing flight time or travel cost while making a certain number of stops to various cities across the country.

Our model has two approaches depending on what Epic would like to optimize. The first is minimizing travel costs, these include flight costs and the hotel cost that corresponds to staying in a particular city. The second is minimizing the travel time, this includes the time spent flying from one city to the next. Both approaches (e.g. objective functions) will be investigated in each different formulations of the problem. The network of flights considered can be seen in the figure below. Figure (left) depicts the intermediate flight paths between cities, and Figure (right) depicts the departing and returning flights from Madison for each city. As shown as below, the software developer could visit one of the 14 different major cities from Madison: Seattle, San Francisco, Los Angeles, Denver, Las Vegas, Atlanta, Minneapolis, Dallas, Orlando, Chicago, Detroit, Charlotte, Miami, and New York.

<p float="left">
  <img src="https://github.com/zwu363/UW-Madison-SP22-CS524/blob/main/figure/figure1.png" width="30" />
  <img src="https://github.com/zwu363/UW-Madison-SP22-CS524/blob/main/figure/figure2.png" width="300" /> 
</p>

The following data was collected for this problem: flight costs, hotel costs, and flight times. Flight costs and hotel costs were collected using Google, and the cheapest airline and hotel chain was selected. Flight and hotel costs were collected for June 1st – 7th 2022. It is assumed that the costs remain the same day to day within this narrow timeframe. Flight times were collected using https://www.travelmath.com/flying-time/. It is assumed that flights cannot be delayed or canceled.

We have modeled 3 separate scenarios that Epic might be interested in. Each scenario will consider the two problems mentioned above, either minimizing travel costs or flight time. The first model (Model 1) considers if Epic wanted to send their software engineer from Madison to one US city, stay overnight in that city, and then fly back to Madison. The second model (Model 2) considers if Epic wanted to send their software engineer from Madison to one city in each region (North, East, South, and West), stay overnight in each of the four selected cities, and then fly back to Madison. The final model (Model 3) considers if Epic wanted to send their software engineer from Madison to each US city, staying overnight in each city, and then fly back to Madison. Each model will choose the optimal flight path to minimize travel cost or flight time.
