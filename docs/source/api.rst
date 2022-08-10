API reference
=============

Reddit
-------
Description
-----------
CPPRAW's main class, this must be the first class to be instantiated.
.. code-block:: c++
    cppraw::reddit reddit("client-id", "client-secret","reddit-user", "reddit-password", "user-agent");
Member functions
----------------
subreddit
~~~~~~~~~
This function returns a subreddit object, taking a string as a parameter, corresponding to the subreddit you wish to look for.
Parameters:
std::string subreddit //the name of the subreddit you wish to look for
.. code-block:: c++
    cppraw::subreddit subreddit = reddit.subreddit("cpp");


Subreddit
----------
Description
-----------
This class lets you interact with a subreddit.
.. code-block:: c++
    cppraw::subreddit subreddit = reddit.subreddit("cpp");
Member functions
----------------
recent
~~~~~~~
hot
~~~~
rising
~~~~~
top
~~~~
controversial
~~~~~~~~~~~~~
random
~~~~~~
get_post
~~~~~~
Post
------