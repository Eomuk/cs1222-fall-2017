# Lab3

Total points: 10pts

Due at the end of class, please raise your hand when you are finished, and we can walk over your implementation.

> I may ask a few question on your implementation to further clarify your understanding.

## Section 7 and 8 (12:00 to 4:30 section)

3. Report the number of female, male members and the total number.  Use proper column names.
5. For each title id, report the number of sound files.
6. The following SQL statement uses an Intersect to list all cities and regions that have both members and artists:
    ```
SELECT         city, region
FROM            Members
INTERSECT
SELECT         city, region
FROM            Artists. 
    ``` 

    > Unfortunately you cannot use Intersect in MySQL. Write a query that would run in the other databases, using a Join to accomplish the  same thing.

11. Produce a list of all of the area codes used in both member's home phones and studio's phones along with a count of the phone numbers for each area code.

**Data Manipulation**

> Please use “select * from …” after each query to show the effect of the query.  

2. The title 'Time Flies' now has a new track, the 11th track 'Spring', which is 150 seconds long and has only a MP3 file. Insert the new track into Tracks table.
5. The area code for Columbus, Ohio has been changed from 277 to 899. Update the homephone and workphone numbers of all members in Members2 table accordingly.
6. Salesperson Bob Bentley has agreed to turn over all his female members to salesperson Lisa Williams whose sales id is 2. Update the Members2 table accordingly. 
7. Members Doug Finney and Terry Irving are forming a new artist to be called "Doug and Terry." Add this record to the Artists table, using ArtistID 13, the address information of Doug Finney, no web address, today's entry date, and no lead source. Don’t hand-code any data for insert that can be looked up from the Members table.
8. Add the appropriate new records to the XrefArtistsMembers table for the artist "Doug and Terry" (see #4). Doug is the responsible party. Don’t hand-code any data for insert that can be looked up from the Members table.


## Section 9 and 10 (4:30 to 8:30 section)

4. Report the number of artists who entered in the same year  and the total number.
7. For  title id 1, report  the title ID, track title, lengthseconds, the average lengthseconds for all tracks of title id 1 , and the difference value between the lengthseconds and the average value.
10. Report the title name, number of tracks, and total time in minutes for each title.
12. For each artist list the artist name and the first and last name (together in one column) of every member associated with that artist followed on the next line by a count of the number of members associated with that artist. Include all artists whether they have members or not.
14. List the artist id and the artist name of all artist who have members not in USA

> Please use “select * from …” after each query to show the effect of the query.   

1. Add a new artist with the following information. Use a proper function to automatically get today's date.

| ArtistID | ArtistName | City | Region | Country | WebAddress | EntryDate | LeadSource |
| :-- | :-- | :-- | :-- | :-- | :-- | :-- | :-- |
| 12 | November | New Orleans | LA | USA | www.november.com | (today) | Directmail |

4. Populate Members2 the content of the Members table.

    > Suppose table is created with below

    ```
CREATE TABLE Members2 LIKE Members;
    ```

9. Lyric Music has decided to set up a web page for every artist who doesn't have a web site. The web address will be www.lyricmusic.com/ followed by the artistID. Fill this in for every artist record that doesn't already have a web site.
10. Delete all members who work for the artist 'Sonata' from Members2 table.
5. The area code for Columbus, Ohio has been changed from 277 to 899. Update the homephone and workphone numbers of all members in Members2 table accordingly.
