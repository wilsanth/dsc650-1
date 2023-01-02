---
title: Assignment 1
subtitle: Computer performance, reliability, and scalability calculation
author: Anthony Wilson
---

## 1.2 

#### a. Data Sizes

| Data Item                                  | Size per Item | 
|--------------------------------------------|--------------:|
| 128 character message.                     | 512 Bytes     |
| 1024x768 PNG image                         | 3.15 MB       |
| 1024x768 RAW image                         | 1.5 MB        | 
| HD (1080p) HEVC Video (15 minutes)         | 600 MB        |
| HD (1080p) Uncompressed Video (15 minutes) | 800 MB        |
| 4K UHD HEVC Video (15 minutes)             | 700 MB        |
| 4k UHD Uncompressed Video (15 minutes)     | 950 MB        |
| Human Genome (Uncompressed)                | 200 GB        |

#### b. Scaling

|                                           | Size     | # HD       | 
|-------------------------------------------|---------:|-----------:|
| Daily Twitter Tweets (Uncompressed)       | 256 GB   |  1         |
| Daily Twitter Tweets (Snappy Compressed)  | 400 GB   |  2         |
| Daily Instagram Photos                    | 273 TB   |  82        |
| Daily YouTube Videos                      | 1.7 PB   |  519       |
| Yearly Twitter Tweets (Uncompressed)      | 93.4 TB  |  28        |
| Yearly Twitter Tweets (Snappy Compressed) | 146 TB   |  44        |
| Yearly Instagram Photos                   | 99.7 PB  |  29894     |
| Yearly YouTube Videos                     | 620.5 PB |  186165    |

#### c. Reliability
|                                    | # HD    | # Failures |
|------------------------------------|--------:|-----------:|
| Twitter Tweets (Uncompressed)      | 28      |  .46       |
| Twitter Tweets (Snappy Compressed) | 44      |  .72       |
| Instagram Photos                   | 29894   |   490.26   |
| YouTube Videos                     | 186165  |   2971.11  |

#### d. Latency

|                           | One Way Latency      |
|---------------------------|---------------------:|
| Los Angeles to Amsterdam  | 75 ms                |
| Low Earth Orbit Satellite | 7 ms                 |
| Geostationary Satellite   | 120 ms               |
| Earth to the Moon         | 1.2 -1.35 ms         |
| Earth to Mars             | 2.5 - 10 minutes     | 


Explanation of Latency: 
LA to Amersterdam: i just copied the average latency from this website: https://wondernetwork.com/pings/Los%20Angeles/Amsterdam for July 5th. I then divided the numbers by two, because it seems like it is a round trip, and then calculated the average.

For everything else I researched what the values are and found the following websites listed below where they have documented the latency. The websites describe the latency as a round trip so I just divided each of them by two. 

LEO - North America to LEO: https://www.ookla.com/articles/starlink-hughesnet-viasat-performance-q2-2022
Geostationary Satellite: https://www.satsig.net/latency.htm
Earth to the Moon: https://en.wikipedia.org/wiki/Earth%E2%80%93Moon%E2%80%93Earth_communication#:~:text=Echo%20delay%20and%20time%20spread,-Radio%20waves%20propagate&text=Propagation%20time%20to%20the%20Moon,the%20Moon%20is%20384%2C400%20km).
Earth to Mars: https://mars.nasa.gov/mars2020/spacecraft/rover/communications/#:~:text=It%20generally%20takes%20about%205,Earth%2C%20depending%20on%20planet%20positions.