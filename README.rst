PyAtom
=============================

A Python library for generating Atom 1.0 feeds.

Extracted from werkzeug.contrib.atom and created as a standalone package.


Latest Version
-----------------------------------------
The latest version of this project can be found at : http://bitbucket.org/sramana/pyatom.


Installation
-----------------------------------------
# Option 1 : Install via pip ::

    pip install pyatom

# Option 2 : If you have downloaded the source ::

    python setup.py install

Documentation
-----------------------------------------
How to use? ::

    from pyatom import AtomFeed

    feed = AtomFeed(title="My Blog",
                    subtitle="My example blog for a feed test.",
                    feed_url="http://example.org/feed",
                    url="http://example.org")

    # Do this for each feed entry
    feed.add(title="My Post",
             content="Body of my post",
             content_type='html',
             author="Me",
             url="http://example.org/entry1",
             updated=datetime.datetime.utcnow(),
             published=datetime.datetime.utcnow())

    print feed.to_string()


License
-----------------------------------------
This project is licensed under New BSD license.


Contribution and Feedback
-----------------------------------------
Contributions and Feedback are most welcome. Please email the author with your comments.


Author Information
-----------------------------------------
Ramana <sramana9@gmail.com>

* http://bitbucket.org/sramana
* http://github.com/sramana