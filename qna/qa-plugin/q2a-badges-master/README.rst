==============================
Question2Answer Badges v 1.0b2
==============================
-----------
Description
-----------
This is a plugin for **Question2Answer** that provides basic badge functionality. 

--------
Features
--------
- currently 55 badges implemented (see `Badge List`_ below)
- badges are categorized into types (e.g. gold, silver, bronze)
- badge notification system triggers jquery notice when awardee accesses the site
- option to notify users of badge awarding by email (fully customizable)
- public badge page displays awardable badges
- awarded badges may be shown in individual profile pages, with links to source (if available)
- awarded badge may be shown as medals in individual posts and on global users lists
- badge names and requirements are modifiable via admin page
- badge system may be deactivated via admin page
- badges may be individually deactivated via admin page
- full translation table available (see `Translation`_ below)

------------
Installation
------------

#. Install Question2Answer_
#. Get the source code for this plugin from github_, either using git_, or downloading directly:

   - To download using git, install git and then type 
     ``git clone git://github.com/NoahY/q2a-badges.git badges``
     at the command prompt (on Linux, Windows is a bit different)
   - To download directly, go to the `project page`_ and click **Download**

#. navigate to your site and check your database to make sure the tables were created (^badges and ^userbadges)
#. Go to **Admin -> Plugins** on your q2a install and select the '**Activate badges**' option, then '**Save Changes**'.

.. _Question2Answer: http://www.question2answer.org/install.php
.. _git: http://git-scm.com/
.. _github:
.. _project page: https://github.com/NoahY/q2a-badges

.. _Translation:

-----------
Translation
-----------
The translation file is **qa-lang-badges.php**.  Copy this file to the **qa-lang/<your-language>/** directory.  Edit the right-hand side strings in this file with notepad2, notepad++, etc. (don't ever use Window's Notepad. For anything. Ever.), for example, changing:

**'good_question'=>'Good Question',**

to

**'good_question'=>'Swali nzuri',**

for Swahili.  Don't edit the string on the left-hand side or bad things will happen.

Once you've completed the translation, don't forget to set the site language in the admin control panel... to Swahili.  

----------
Disclaimer
----------
This is **beta** code.  It is probably okay for production environments, but may not work exactly as expected.  Refunds will not be given.  If it breaks, you get to keep both parts.

-------
Release
-------
All code herein is Copylefted_.

.. _Copylefted: http://en.wikipedia.org/wiki/Copyleft

---------
About q2A
---------
Question2Answer is a free and open source platform for Q&A sites. For more information, visit:

http://www.question2answer.org/

.. _Badge List:

----------
Badge List
----------

==========   =================      ========================================
Level [#]_   Title                  Description
==========   =================      ========================================
1            Verified Human         Successfully verified email address

1            Nice Question          Question received +# upvote
2            Good Question          Question received +# upvote
3            Great Question         Question received +# upvote

1            Notable Question       Asked question received # views
2            Popular Question       Asked question received # views
3            Famous Question        Asked question received # views

1            Nice Answer            Answer received +# upvote
2            Good Answer            Answer received +# upvote
3            Great Answer           Answer received +# upvote

1            Renewal                Received "Nice Answer" badge in response to a question more than # days old
2            Revival                Received "Good Answer" badge in response to a question more than # days old
3            Ressurection           Received "Great Answer" badge in response to a question more than # days old

1            Gifted                 # answers selected as best answer
2            Wise                   # answers selected as best answer
3            Enlightened            # answers selected as best answer

1            Grateful               Selected # answers as best answer
2            Respectful             Selected # answers as best answer
3            Reverential            Selected # answers as best answer

1            Liked                  Received # total upvotes
2            Loved                  Received # total upvotes
3            Revered                Received # total upvotes

1            Asker                  Asked # questions
2            Questioner             Asked # questions
3            Inquisitor             Asked # questions
 
1            Answerer               Posted # answers
2            Lecturer               Posted # answers
3            Preacher               Posted # answers

1            Commenter              Posted # comments
2            Commentator            Posted # comments
3            Annotator              Posted # comments

1            Voter                  Voted # times
2            Avid Voter             Voted # times
3            Devoted Voter          Voted # times

1            Editor                 Performed total of # edits
2            Copy Editor            Performed total of # edits
3            Senior Editor          Performed total of # edits

1            Watchdog               Flagged # posts as inappropriate
2            Bloodhound             Flagged # posts as inappropriate
3            Pitbull                Flagged # posts as inappropriate

1            Reader                 Read total of # questions
2            Avid Reader            Read total of # questions
3            Devoted Reader         Read total of # questions

1            Dedicated              Visited every day for # consecutive days
2            Devoted                Visited every day for # consecutive days
3            Zealous                Visited every day for # consecutive days

1            Visitor                Visited site on total of # days
2            Trouper                Visited site on total of # days
3            Veteran                Visited site on total of # days

1            Regular                First visited more than # days ago
2            Old Timer              First visited more than # days ago
3            ancestor               First visited more than # days ago

1            100 Club               Received total of # points
2            1,000 Club             Received total of # points
3            10,000 Club            Received total of # points

1            Medalist               Received total of # badges
2            Champion               Received total of # badges
3            Olympian               Received total of # badges
==========   =================      ========================================

.. [#] Level refers to difficulty level (e.g. gold, silver, bronze).
