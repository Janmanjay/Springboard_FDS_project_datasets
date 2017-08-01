# Introduction

Your capstone project is a crucial part of your Springboard Foundations of Data Science
workshop. Through it you will practice and demonstrate key skills required of a
data scientist. As such, identifying a suitable data set (and associated question)
is your singlemost important task when starting on your workshop. It is also notoriously
difficult and bemuses many a student!

The data set should:
* facilitate, even generate, good questions to answer
* be big and complex enough to require a computer
* be small and manageable enough to analyse on a single computer (yours)
* be readily available, e.g. as a download of a (few) CSV file(s)
* be available under sufficiently unrestrictive terms.

A data set that just about allows you to plot a graph showing an up/downward trend
is not really answering a good question; anyone can plot a line chart in excel.
A summary table of the annual GDP of the G8 countries over the past five years
is neither big nor complex; something small and simple like that offers no potential
for answering an interesting question. A project question that depends upon
scraping a thousand web pages, when you've done no web scraping before, or that you
cannot even load into memory on your computer, will likely put you in the position two
months down the road of not even having finished obtaining your data. Several students
have thought to use data from their work, but the reality of seeking, and obtaining,
permission to publicly use company (generally proprietary) data makes it undesirable,
if permission is even finally granted; yes, ways can be found to manage the use of
confidential data, but it presents a difficulty that is well worth avoiding in the 
first place.

Here I attempt to point you towards some nice data sets I've found on my travels
(okay, some have been found by students). Your capstone project should be your own
work, and I try not to be too leading or prescriptive in these examples to leave
you room to form your own questions.

# Data sets

## Depressive symptoms during experiment to reduce anti-depressant medication

### Keywords
medical, medicine, mental health

### Summary
A single patient on anti-depressant medication had his medication dosage
gradually decreased in a double-blind manner. Mood and symptoms were monitored
several times a day. Data comprises some 1478 measurements (rows) of multiple
parameters over 239 consecutive days.

### What I love about it
The data are readily available as a single download. There is a great dictionary.
The paper describes very useful context. The features are rich and measured
over varying frequencies (some daily, some weekly). The anti-depressant dosage
is recorded for each day, although not known at the time to the patient. The
patient answered questions at random times throughout the day. There is thus abundant
scope for investigations of relationships between the measured parameters.

### How do I get it?
The page for the paper is [here](http://openpsychologydata.metajnl.com/articles/10.5334/jopd.29/)
and the link to the data download is under "Repository location".

## DOTA2 online game statistics

### Keywords
online game, MOBA, player, match, skill

### Summary
A dataset containing 50000 matches from the online game Dota2. The data details which team won,
which heroes (characters) were in the teams, which player ID was playing, match duration,
parameters such as how many times a player/character killed and died and many other features.

### What I love about it
I've actually seen this turned into a great capstone project analysis. There is scope for
analysing the characteristics of the different heroes, interactions between them, matches,
and much more. All data are readily available in a
single download, but over multiple files, allowing plenty of scope to add value by joining
data from different files on common fields. 

### How do I get it?
The data are hosted on kaggle [here](https://www.kaggle.com/devinanzelmo/dota-2-matches).
Whilst kaggle links often make us roll our eyes, this is one of those times when it's used
to host a really interesting data set rather than a typical kaggle data set of "training.csv"
and "test.csv".

## Flights departing NYC in 2013

### Keywords
airline, travel, delay, time, plane, weather

### Summary
A collection of datasets giving information about all flights departing NYC in 2013,
the airports, airlines, planes, and even the weather. Thus there is information
on what type of plane (and engine) departed what airport at what time and whether it
was on time leaving/arriving, as well as the weather conditions.

### What I love about it
This is a great dataset that's available as an R package. Do not think that such
easy availability makes this a poor choice; it's a great choice that allows you to
get started on your project without getting bogged down by unavailable data. It is a rich
dataset that captures a wide variety of parameters and offers lots of scope for
adding value by joining data from different data frames.

### How do I get it?
The data is available as an R package from 
[CRAN](https://cran.r-project.org/web/packages/nycflights13/index.html).
Now, the tailnumbers of the flights are given, but the information about the planes
seems to be a subset of what is available from the 
[FAA](https://www.faa.gov/licenses_certificates/aircraft_certification/aircraft_registry/releasable_aircraft_download/).
The downloadable FAA data, for example, also includes data about the plane's home 
location, which I don't think is included in the R package data. This second source
of data provides scope for the more adventurous to explore further. Does the
population of plane types that use NYC match the general population in the FAA
database? Is there anything surprising about the registered addresses of the planes
that use NYC? (I don't know...)

## UK Environment Agency Water Quality Archive

## Keywords
environment, water, quality, EA open datasets

### Summary
Data on water quality measurements around England. Sample points can be coastal, estuarine waters,
rivers, lakes, canals or groundwaters. Data from years 2000 onwards are available. A large number
of water quality parameters are provided along, for example, the sample locations name and
position, and date of course. The purpose of the sample is also given.

### What I love about it
Firstly, the documentation available is excellent. I commend the EA for this. Note that it's
open data, but they do request you acknowledge the source if you use the data (well it would
only be polite). Note also that there's an API *but I recommend you don't use this*. The reason
is that there are CSV files available that are really easy to download and start using and ideal
for a capstone project. You can pick a region and a year, download the file, and you're off. There's
plenty of scope for demonstrating data wrangling because, for example

* different quality parameters are provided for different purposes
* the data format is just begging to be made "wide"

What locations would you select? What patterns can you see over time? Can you infer any relationships
between the various water quality parameters? If you nail this and get bored, can you find any local
historic weather data (e.g. rainfall) to join with it? If you have an environmental interest, this
could be a great selection of data.

One sneaky hint that I use myself is that the download data have location in easting and northing and
this gives you a really easy way to just plot locations as x and y in a scatter plot to essentially
get a geographic plan view! 

### How do I get it?
The download page is [here](http://environment.data.gov.uk/water-quality/view/download#).
It's really easy to navigate to the [Documentation](http://environment.data.gov.uk/water-quality/view/doc/reference).
