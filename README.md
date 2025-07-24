# radarr-import-list-guide
the EASY way to register a ton of movies on Radarr

# Instructions

## IMDB Import to Trakt.tv to Radarr

IMDB has blocked the ability to import movies from IMDB Lists into Radarr so this is the next best method

- Make an IMDB account https://www.imdb.com/ & log in
- make a Trakt.tv account https://trakt.tv/ & log in
- find an IMDB movie list
  - example https://www.imdb.com/list/ls056361892/
- on the IMDB list web page, select Export and obtain the .csv version of the list
- in Trakt.tv go to Settings > Data https://trakt.tv/settings/data and select the Import option
- select the option for IMDB and upload the .csv file you just downloaded
- in Trakt, the movies you imported show up in your Watchlist
- navigate to your Watchlist on Trakt at `https://trakt.tv/users/<your-username-here>/watchlist` and select Manage > Move to move the items to another list
  - optional: make the new list Public by navigating to the new list and updating its settings
- in Radarr navigate to Settings > Import Lists (`settings/importlists`) and scroll to the bottom and add a new Trakt List
- fill in all the options shown in the Radarr Import List menu
  - **IMPORTANT**: make sure you create a Tag for the list items under "Radarr Tags"
  - you do not give the URL to the list on the "Trakt List" page, instead you just list your username and the name of the list, which you can find in Trakt.tv under My Lists
    - example: if your list is at `https://trakt.tv/users/my-name/lists/my-list` then in Radarr you enter "my-name" as the Username and "my-list" as the name of the list
  - make sure to click the button for "Authenticate with Trakt" and allow Radarr to access the list via your Trakt.tv account
  - click Test and then Save if it looks good
 
Now all the items from your Trakt.tv list will automatically get imported to Radarr. If you selected the options in Radarr, they will automatically get Searched and added to your Download client upon getting added to Radarr.

## Import from a Custom List with mdblist

If you want to import items from a custom made Movie list that can also automatically update itself, then you want https://mdblist.com/

Make an account in mdblist and then create a list and Save it; you have the option to create only a mdblist List or both a mdblist List and a Trakt.tv List by linking your Trakt.tv account. Either option works. 

If you also make a Trak.tv list, then give mdblist a few minutes to sync with Trakt and then add the Trakt list to Radarr as described above.

If only make a mdblist List then in Radarr instead choose the option for Custom List and give the URL to the List on mdblist.

**IMPORTANT**: do NOT forget to add a Tag for each list so that you can keep track of which items were imported to Radarr via which List
