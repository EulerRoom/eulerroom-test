EulerRoom
===================

This is copied from the dorkbotlondon.org website, hope they don't mind.

Their instructions are below.

How to add Dorkbot events
--------------------------------------------------------
This website is generted by jekyll, and automatically builds when someone (maybe you!) pushes a new version to github.

The entries for each Dorkbot live in the _posts directory, and are named as YEAR-MONTH-DAY-DORKBOTNUMBER.html.

At the top of each file you find a section of metadata, the only things you need to care about are:
* `number`. Which should be the Dorkbot number.
* `start`. The date + time this Dorkvent starts.
* `end`. Obvious.
* `where`. A reference to where the event took place - this needs to match up to an entry in _data/locations.yaml.
* `tags`. This should be a list of all the people who spoke at this dorkbot.
* Optionally, `title`. This is used for named events such as Dorkboat.

Below the --- line, you can put whatever you like, it'll be inside a `<pre>` tag on the website, but you can use html tags and other fancy things.

If you want to preview the website after you've added a new event or changed an old one, run `jekyll serve` (assuming you have it installed) and it'll give you a webserver address to visit.

When you're done, `git add`, `git commit` and `git push` the changes.

Adding new locations
-----------------------------------------
Look in the `_data/locations.yaml` file, it should be somewhat obvious.

Handy scripts
-----------------------------------------
If you look in `/scripts/` there's a little program called `autoformat.py`. If you feed this one or more filenames in the style `./scripts/autoformat.py file1.txt file2.txt` it will take the raw text, wrap it nicely and sort out all the links. It's not perfect, but it's tremendously useful when importing old posts from the mailing list.
