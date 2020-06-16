---
# Documentation: https://sourcethemes.com/academic/docs/managing-content/

title: "The Top Gun Effect"
subtitle: ""
summary: "The stupidest way to predict an election"
authors: [admin]
tags: []
categories: []
date: 2020-06-14T01:45:09-07:00
lastmod: 2020-06-14T01:45:09-07:00
featured: false
draft: false

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
# Focal points: Smart, Center, TopLeft, Top, TopRight, Left, Right, BottomLeft, Bottom, BottomRight.
image:
  caption: ""
  focal_point: ""
  preview_only: false

# Projects (optional).
#   Associate this post with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `projects = ["internal-project"]` references `content/project/deep-learning/index.md`.
#   Otherwise, set `projects = []`.
projects: []
---

If you’ve ever thought about political design — or even paid attention to elections — you’ve probably picked up on what I call the “Top Gun effect”. Every logo has to be red-white and blue and use the stars and stripes. Every ad has to end with a soldier framed against the sunset. Every slogan sounds like they're promoting "an American America, where our strength is strong".

The [Center for American Politics and Design](https://www.politicsanddesign.com/) maintains a database of campaign logos from each and every American congressional candidate in the 2018 midterms, and I decided to sort through the entire database of incumbent candidates’ logos and record the following data for each: state, party, office, color scheme, and iconography. Across 403 total logos I found the following: 171 red-white-and-blue color schemes, 147 stars, 41 American flags, 32 state outlines, 2 eagles, 1 Maryland flag, 2 cowboy hats, 1 cowboy, 1 photo of Barbara Lee, 1 photo of Jose Serrano’s house, and (most surprisingly) only 1 Texas flag.

## Mapping the House

I grouped the data together both by US State and Census Division (a grouping of states by geographic region) to determine which areas of the country are most and least explicitly nationalistic in their political design. Nebraska was the only state in which every logo made use of a red-white-blue (RWB) color scheme followed by Ohio (81.25%) and Georgia (71.47%) as second and third-most likely. Alaska, New Hampshire, New Mexico, Montana, and North Dakota each had no RWB logos. Out of all fifty states, surprisingly only nineteen had a logo that used the flag or its stars and stripes imagery. Georgia (35.71%) was the most likely state to use the flag, followed by Kansas (33.33%) and Alabama, Michigan, Mississippi, and Iowa (each 25%).

### Flag Imagery by Region

| Region             | Total Logos | RWB Logos | RWB Concentration | Flag Logos | Concentration |
| ------------------ | ----------- | --------- | ----------------- | ---------- | ------------- |
| Pacific            | 70          | 32        | 45.71%            | 4          | 5.71%         |
| Mountain           | 27          | 10        | 37.04%            | 0          | 0.00%         |
| West North Central | 27          | 16        | 59.26%            | 2          | 7.41%         |
| East North Central | 44          | 28        | 63.64%            | 6          | 13.64%        |
| West South Central | 61          | 32        | 52.46%            | 6          | 9.84%         |
| East South Central | 24          | 13        | 54.17%            | 3          | 12.50%        |
| New England        | 22          | 12        | 54.55%            | 1          | 4.55%         |
| Middle Atlantic    | 50          | 31        | 62.00%            | 6          | 12.00%        |
| South Atlantic     | 78          | 46        | 58.97%            | 13         | 16.67%        |

The Mountain Division (MT, ID, WY, NV, UT, CO, AZ, NM) is the least likely to use both the colors and image of the flag, earning it the "Least 'Top Gun' Region" award. East North Central (WI, MI, IL, IN, OH) is the most 'Top Gun' as the most likely to use RWB schemes and the second-most likely to use the flag. Further, I tracked party affiliations for every member to see differences in use of color by Republicans and Democrats.

### Logo Color by Party Affiliation

| Party       | Total Logos | Non-RWB Logos | RWB Concentration |
| ----------- | ----------- | ------------- | ----------------- |
| Democrat    | 280         | 71            | 74.64%            |
| Republican  | 250         | 36            | 85.60%            |
| Independent | 2           | 1             | 50.00%            |
| Libertarian | 1           | 0             | 100.00%           |

## Selling the President

Accomplished statesman Adlai Stevenson famously called media-oriented campaigning "the ultimate indignity to the democratic process," claiming that it amounted to "merchandis[ing] candidates for high office like breakfast cereal." Stevenson, however, is likely best known for his back-to-back landslide losses against Dwight D. Eisenhower in 1952 and 1956, rendering his objections to the modern campaign process more or less completely unheeded. Thus, I've decided to examine the different ways in which the President has been sold over time.

I mapped out every major-party Presidential nominee since 1980 and tracked their use of the image and colors of the American flag. Immediately, two candidates emerge as outliers. John McCain avoids the American flag and instead presents an image drawn from his background in the Navy: a white nautical star bounded by two buff stripes over a dark blue background. The facts that McCain: served as a Navy pilot for thirteen years, was both the son and grandson of admirals, based his Presidential campaign stylings after those of the Navy, is the namesake of a Navy destroyer ship, and shares the "Maverick" nickname with Tom Cruise's Lieutenant Mitchell; make him the undeniable winner of the "Most 'Top Gun' Politician" award. McCain notably reverted to a more traditional red-white-blue and flag logo for his 2010 Senate re-election campaign. Jimmy Carter, on the other hand, continues to be an anomaly amongst modern American presidents, invoking neither the image nor the colors of the American flag, instead opting for a white outline of the US map against a forest green background. Thus, Carter is the least 'Top Gun' candidate of the past forty years.

All ten other Presidential nominees make use of the red-white-blue color scheme. Similarly, every candidate used the imagery of the flag in their campaign logos except for Jimmy Carter, Ronald Reagan, Al Gore, John McCain, Mitt Romney, Hillary Clinton, and Donald Trump. Bill Clinton is unique in that he used the flag in his 1992 logo but not in his 1996 logo. The data then show that both parties are equally likely (90.91%) to use the red-white-blue color scheme, while the Democrats (63.64%) are unexpectedly more taken to using the image of the flag compared to Republicans (45.45%).

## Predicting 2020 

With these we are able to reverse-engineer a model to predict the outcome of a Presidential election based on the color and composition of the candidates' campaign logos. From the ten previous elections we see that both candidates that strayed from the red-white-blue scheme have lost, indicating that candidates that don't make use of the national colors have a 0% chance to win. Thus, we can conclude that the minor Libertarian and Green Parties have -- statistically speaking -- no shot at the Presidency due to their predilection for using yellow and green, respectively. The model gets this much correct, at least. Now that we've established that a candidate must use and RWB scheme to win, we can examine the effect that use of the flag / stars and stripes has on their chances. Over these ten elections, six of the eleven candidates that used the flag won, compared to four of the nine who did not. Thus, candidates who use stars and stripes imagery have a 54.54% chance to win, and those who don't have a 44.44% chance. Thus, the model will favor candidates who do use the flag over those who don't.

### Historical predictions, 1980-2016

| Year | Democrat | Republican | Prediction     |
| ---- | -------- | ---------- | -------------- |
| 1980 | 0.00%    | 44.44%     | Ronald Reagan  |
| 1984 | 54.54%   | 44.44%     | Walter Mondale |
| 1988 | 54.54%   | 54.54%     | No call        |
| 1992 | 54.54%   | 54.54%     | No call        |
| 1996 | 44.44%   | 54.54%     | Bob Dole       |
| 2000 | 44.44%   | 54.54%     | George W. Bush |
| 2004 | 54.54%   | 54.54%     | No call        |
| 2008 | 54.54%   | 0.00%      | Barack Obama   |
| 2012 | 54.54%   | 44.44%     | Barack Obama   |
| 2016 | 44.44%   | 44.44%     | No call        |

Now, to examine the 2020 Presidential election. Joe Biden and Donald Trump both use RWB logos, but only Biden makes use of the stars and stripes motif. As such, the aesthetic model lists the odds of a Biden victory over Trump at 55.10%. Notably, this model is only able to make a prediction six in ten times. So while two-thirds of its predictions are accurate (which technically is the same accuracy rate as electoral wunderkind Nate Silver's prized FiveThirtyEight model), it is only able to correctly predict four in ten total elections. There is another glaring critique of the model: that it is inherently ridiculous, willfully ignores any and all political reality, and was only created as a project with which to amuse myself. Each of those statements are, of course, true. However, I would again like to point to the fact that this model is as technically accurate as Nate Silver's. As I am honestly not interested or skilled enough to offer serious commentary on the state of the Biden or Trump campaigns, I will stand by this model as my official prediction for the 2020 election.

If you'd like to look over my data / critique my methods / accost me for not rigidly following Marx's dialectical view of history, you can view my work here: https://docs.google.com/spreadsheets/d/11oeiletOJ6fSh9m9teFnq-kVqtCDwgM2mcF7UBQ3Jx0/edit?usp=sharing