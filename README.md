# finalProjProposal

Project Name:
Video Search Roulette

Problem:
User is bored and wants to kill time by watching random/nonsensical videos on YouTube. User does not want to think up goofy words to type in and search.

Description:
App that generates three random words and sends search request to YouTube. App returns top result and displays to user.

Features:
  MVP:
    Random Word selection
    Search based on random words
    Display of videos
  Additional:
    Share video with friends
    Save video link to go back and watch again
    Create playlists of goofy videos


User Stories:

  Application:
    >UI interface that is responsive (viewable on mobile, tablet, laptop)
    >One page app
    >Interface with word generator API
    >Interface with YouTube API
    >View video
    >share on social media

  Feature: Random Word selection
    1) As a user I want the random word generator to use English, Non-Curse words, so that I can view content meaningful to me.
      >Research and select a word generator API
        >API must be free
        >API must have feature to filter out curse words

    2) As a user I want the random word generator to be initiated by me so that I can control when words are generated. Or if i want to request more than once.
      >Create button on UI
      >Create button function that initiates GET to random word API

  Feature: Execute video search
    3) As a user I want the system to send the three random words to YouTube API so that a single video is returned for me to view.
    4) As a user I want the search to filter results so that I am viewing top rated, safe, shorter than 4 min content.
      >Create GET that concatenates three random words in request to YouTube
      >Include in GET params rating, safe, length (see API documentation for syntax)


  Feature: Display of videos
    5) As a user I want to view videos within the context of my screen so that i can access other features on my laptop or mobile phone.
    6) As a user I want to be able to view videos full screen on my laptop, tablet or phone so that i can see better.
      >Research and select video player component
      >

  Feature: Share video with friends
    7) As a user I want to share my video with my friends across standard social platforms so that I do not have to laugh alone.
      >Research and select share feature (could this be included in the video component?)

  Feature: Save video link to view again
    8) As a user, I want to identify videos as favorites so that i can recall and view them again
      >

  Feature: Create a playlist of videos
    9) As a user, I want to be able to create multiple playlists so that I can view many groups of videos.
    10) As a user I want to be able to name my playlist so that i can discern it from other playlists
    11) As a user i want to be able to add one or many videos to a playlist

    Notes:

      YouTube API:
        https://developers.google.com/youtube/v3/

      Some potential API's for random word selection (just a list, not vetted yet):
        http://randomword.setgetgo.com/
        https://www.programmableweb.com/api/setgetgo-random-word

      Initial research for share feature:
        http://socialsharekit.com/
        https://github.com/bostondv/bootstrap-share-buttons

      Video player info:
        https://stackoverflow.com/questions/26040136/bootstrap-3-responsive-mp4-video
        http://getbootstrap.com/components/#responsive-embed

      Playlist info:
        (not sure this applies - requires additional reading) http://lab.abhinayrathore.com/bootstrap-youtube-playlist-popup/
