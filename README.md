# Russian Presidential Election 2018
CSV formatted data of results from 97k+ election sites.
##### Kaggle dataset is here: https://www.kaggle.com/rexhaif/ru-elections-2018
##### Based on Sergey Shpilkin raw data. https://podmoskovnik.livejournal.com/
##### Raw data can be obtained from google drive: https://drive.google.com/file/d/1hQQM_ceSzwVWBVyJJynW3_3UNKaJe4o5/view?usp=sharing
## File types: 
 - *-utf8.csv files can be used in python
 - *-utf8-sig.csv files can be used for excel-based processing (this is a correct encoding to view cyrillic chars in excel with no additional config) 
# What columns means:
  - region_name - name of region where election site was located
  - tik_name - name of terrirorial election comission (oftenly based on district name)
  - uik_name - name of election site (local election comission)
  - registered_voters - number of voter, who were linked to that election site
  - received_ballots - number of empty ballots, received from territorial election comission
  - early_voting_ballots - number of ballots, which were given for those, who wants to vote before main date
  - onsite_ballots - number of ballots, which were given on the election site
  - offsite_ballots - number of ballots, which were given, for those, who wants to vote outside of that election site (home-based voting)
  - unused_ballots - number of ballots, which were still unsed at the end of election day
  - found_offsite_ballots - number of ballots, which has been found in the offsite voting boxes
  - found_onsite_ballots - number of ballots, which has been found in the onsite voting boxes
  - invalid_ballots - number of ballots, which were recognized as invalid (more that one selection, paintings etc.)
  - valid_ballots - number of ballots, which were recognized as valid (only one selection)
  - lost_ballots - number of ballots, which has been lost (received_ballots - (onsite_ballots + offsite_ballots + unused_ballots))
  - unaccounted_ballots - number of ballots, which were unaccounted when received (-1 * lost_ballots if lost_ballots is < 0)
  - baburin - number of votes for Baburin Segey Nikolayevich
  - grudinin - number of votes for Grudinin Pavel Nikolayevich
  - zhirinovsky - number of votes for Zhirinovsky Vladimir Volfovich
  - putin - number of votes for Putin Vladimir Vladimirovich
  - sobchak - number of votes for Sobchak Xenia Anatolyevna
  - suraykin - number of votes for Suraykin Maxim Alexandrovich
  - titov - number of votes for Titov Boris Jurjevich
  - yavlinsky - number of votes for Yavlinsky Grigoriy Alexeevich
  
Total number of votes can differ from official CIKRF data because some of election sites hasn't been represented in Sergey Shpilkin data.
