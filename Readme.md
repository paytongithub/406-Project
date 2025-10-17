Data File Breakdowns \n
/ data \n
   / feed_bookmarks \n
        / feed_bookmarks.csv \n
            - Users who liked any of the collected feed generators \n
            - Values:   feed name, user ID, timestamp \n
    / feed_posts \n
        - files here contain posts that fit into the 11 different thematic feeds presented in the paper \n
        - stored in json format \n
        - Groupings of feeds \n
            - Socio-Political: #UkranianView, GreenSky \n
            - Science & Academia: Science, AcademicSky, Political Science, What's History \n
            - News contains posts from verified news organizations \n
            - Minority/Discrimination: BlackSky, #Disability \n
            - Advice/Reccomendation: Game Dev, BookSky \n
        - The relevant ones here are Socio-Political and Minority/Discrimination \n
        - Values:   post_id, user_id, instance, date, text, langs, like_count, reply_count, repost_count, reply_to, reply_author, thread_root, thread_root_author, quotes, quoted_author, labels \n
    / feed_posts_likes \n
        - Data on likes from ./feed_posts \n
        - Values: liker id, author id, post id, timestamp of like \n
    / followers \n
        - Anonymized follower edge list \n
        - Values: user 1 id, user 2 id \n
            - These values represent user 1 following user 2 \n
    / graphs \n
        - Edge files for graphs from reposts, quotes, and replies \n
        - Interaction timestamps are saved \n
    / interactions \n
        - Anonymized interactions edge list \n
        - 6 integers representing a comment, repost, or quote  \n
        - user_id, replied_author, thread_root_author, reposted_author, quoted_author, date \n
    / user_posts \n
        - Data on individual posts collected \n
        - Probably don't need this, as feed_posts exists already \n
    

    
