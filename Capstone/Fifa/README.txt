Readme for FIFA Corruption Tweets (JSON) Dataset :
==================================================

This dataset is being made available using a Creative Commons CC0
Public Domain Dedication. See http://creativecommons.org/publicdomain/zero/1.0/

Data contained within each tweet sample is copyright by the tweet's authors and
is subject to all copyright law. The creator of the dataset makes no assertion
of rights related to the content of each tweet.

The dataset is provided 'as is' without warranty or any representation of
accuracy, timeliness or completeness.

The dataset format is line-oriented JSON in utf8 encoding.


Dataset Overview :
------------------

This dataset is comprised of tweets that are related to the 2015 FIFA corruption
scandal.
 
This dataset was created using the twarc (https://github.com/edsu/twarc)
package that makes use of Twitter's search API.

This dataset provides public access to descriptive files of the contents of the full
Twitter dataset as well as the Tweet Identifiers required to reconstitute the dataset. 

A full copy of the dataset is archived in a restricted format along with the public 
dataset but are not made available for public download due to limitations from the 
Twitter Terms of Service.

The following searches are included in this dataset.

#FIFA

Twitter data making up this dataset was captured between 2015-05-21 and 2015-06-05. 

All Twitter data is stored as line-oriented JSON (each line is a complete JSON
document), and is exactly what was received from the Twitter API.


Public Files:
-------------

fifa_dates.txt.gz     :  Number of tweets per day
fifa_hashtags.txt.gz  :  Number of tweets per hashtag
fifa_ids.txt.gz       :  Tweet IDs for tweets in dataset
fifa_times.txt.gz     :  Number of tweets at a given timestamp
fifa_users.txt.gz     :  Number of tweets per username


Restricted Files:
-----------------

fifa.json.gz          :  8,615,937 unique tweets that form the dataset
fifa_media.tar        :  318,308 media files (images) harvested from tweets

If you find errors, have questions, or are interested in the full dataset for research, 
please  contact Mark Phillips at mark.phillips@unt.edu
