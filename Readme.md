Data File Breakdowns
/ data 
   / feed_bookmarks 
        / feed_bookmarks.csv
            - Users who liked any of the collected feed generators
            - Values:   feed name, user ID, timestamp
    / feed_posts
        - files here contain posts that fit into the 11 different thematic feeds presented in the paper
        - stored in json format
        - Groupings of feeds
            - Socio-Political: #UkranianView, GreenSky
            - Science & Academia: Science, AcademicSky, Political Science, What's History
            - News contains posts from verified news organizations
            - Minority/Discrimination: BlackSky, #Disability
            - Advice/Reccomendation: Game Dev, BookSky
        - The relevant ones here are Socio-Political and Minority/Discrimination
        - Values:   post_id, user_id, instance, date, text, langs, like_count, reply_count, repost_count, reply_to, reply_author, thread_root, thread_root_author, quotes, quoted_author, labels
    / feed_posts_likes
        - Data on likes from ./feed_posts
        - Values: liker id, author id, post id, timestamp of like
    / followers
        - Anonymized follower edge list
        - Values: user 1 id, user 2 id
            - These values represent user 1 following user 2
    / graphs
        - Edge files for graphs from reposts, quotes, and replies
        - Interaction timestamps are saved
    / interactions
        - Anonymized interactions edge list
        - 6 integers representing a comment, repost, or quote 
        - user_id, replied_author, thread_root_author, reposted_author, quoted_author, date
    / user_posts
        - Data on individual posts collected
        - Probably don't need this, as feed_posts exists already
    

    