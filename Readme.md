Data File Breakdowns <br />
/ data <br />
&nbsp;/ feed_bookmarks <br />
&nbsp;&nbsp;/ feed_bookmarks.csv <br />
&nbsp;&nbsp;&nbsp;- Users who liked any of the collected feed generators <br />
&nbsp;&nbsp;&nbsp;- Values:   feed name, user ID, timestamp <br /><br />
&nbsp;/ feed_posts <br />
&nbsp;&nbsp;- files here contain posts that fit into the 11 different thematic feeds presented in the paper <br />
&nbsp;&nbsp;- stored in json format <br />
&nbsp;&nbsp;- Groupings of feeds <br />
&nbsp;&nbsp;&nbsp;- Socio-Political: #UkranianView, GreenSky <br />
&nbsp;&nbsp;&nbsp;- Science & Academia: Science, AcademicSky, Political Science, What's History <br />
&nbsp;&nbsp;&nbsp;- News contains posts from verified news organizations <br />
&nbsp;&nbsp;&nbsp;- Minority/Discrimination: BlackSky, #Disability <br />
&nbsp;&nbsp;&nbsp;- Advice/Reccomendation: Game Dev, BookSky <br />
&nbsp;&nbsp;- The relevant ones here are Socio-Political and Minority/Discrimination <br />
&nbsp;&nbsp;- Values:   post_id, user_id, instance, date, text, langs, like_count, reply_count, repost_count, reply_to, reply_author, thread_root, thread_root_author, quotes, quoted_author, labels <br /><br />
&nbsp;/ feed_posts_likes <br />
&nbsp;&nbsp;- Data on likes from ./feed_posts <br />
&nbsp;&nbsp;- Values: liker id, author id, post id, timestamp of like <br /><br />
&nbsp;/ followers <br />
&nbsp;&nbsp;- Anonymized follower edge list <br />
&nbsp;&nbsp;- Values: user 1 id, user 2 id <br />
&nbsp;&nbsp;&nbsp;- These values represent user 1 following user 2 <br /><br />
&nbsp;/ graphs <br />
&nbsp;&nbsp;- Edge files for graphs from reposts, quotes, and replies <br />
&nbsp;&nbsp;- Interaction timestamps are saved <br /><br />
&nbsp;/ interactions <br />
&nbsp;&nbsp;- Anonymized interactions edge list <br />
&nbsp;&nbsp;- 6 integers representing a comment, repost, or quote  <br />
&nbsp;&nbsp;- user_id, replied_author, thread_root_author, reposted_author, quoted_author, date <br /><br />
&nbsp;/ user_posts <br />
&nbsp;&nbsp;- Data on individual posts collected <br />
&nbsp;&nbsp;- Probably don't need this, as feed_posts exists already <br />
