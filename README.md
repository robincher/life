Life
====

It's a **timeline of important events** in my life, visualized in a way my mind always imagine it. 

Forked from @cheeaun [cheeaun.life](http://cheeaun.life/).

Features
--------
- Super simple
- No fancy formatting
- No fancy setup
- No fancy effects
- Flexible datetimes because sometimes you don't remember the exact date of an event

How to setup your own *Life*
----------------------------

1. Fork this project.
2. `git checkout -b gh-pages` (or any branch name you like)
3. Make a copy of `life.example.md`, rename it to `life.md`.
4. Add your life events into `life.md`.
5. Preview it on a local server. Use [`python -m SimpleHTTPServer`](http://docs.python.org/2/library/simplehttpserver.html) or [`http-server`](https://github.com/nodeapps/http-server).
6. Commit `life.md` (not in `master` branch).
7. `git push origin gh-pages -f` and publish to [GitHub Pages](http://pages.github.com/).
8. Update the website link in your GitHub repo description.
9. Tell the world about your Life.
10. Add your Life to the [Lives](https://github.com/cheeaun/life/wiki/Lives) page.

How to upgrade your *Life*
--------------------------
1. `git checkout master`
2. `git remote add upstream https://github.com/cheeaun/life.git`
3. `git fetch upstream` and `git merge upstream/master` to upgrade to latest Life.
4. `git checkout gh-pages` and `git merge master` to sync changes back to GitHub Pages.

[Learn more](https://help.github.com/articles/fork-a-repo).


How to configure your *Life*
----------------------------
1. Make a copy of `config.example.json`, rename it to `config.json`.
2. Only commit it in `gh-pages` branch.

The configuration:

- `customStylesheetURL` - (*string*, default to `null`) Path to a custom stylesheet file, for those who doesn't like the default *theme*.
- `yearLength` - (*number*, default to `120`) The width of the year grids, in pixels.
- `hideAge` - (*boolean*, default to `false`) Option to hide age from year axis.

Datetime "syntax"
-----------------

- `2000` - event that happen in that year
- `01/2000` - event that happen in that month/year
- `01/01/2000` - event that happen exactly in that day/month/year
- `2001-2005`, `10/2001-02/03/2005` - event that happen within the two dates
- `~2005` - event that happen around the time in that year
- `2005-~` - event that happen from that year and beyond (now).
