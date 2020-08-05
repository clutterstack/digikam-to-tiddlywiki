# digikam-to-tiddlywiki

Jupyter is a friendly environment from which to execute exploratory database queries, and it can be used to create files that can be made into tiddlers by TiddlyWiki.

This notebook documents my exploration of the format of TiddlyWiki's .tid files, and of the SQLite database that digiKam uses to keep track of images and their metadata.

It loops through a list of files found to have a given tag in the digiKam DB (more sophisticated queries are possible but not implemented here), and assembles some image metadata and file location information into fields in individual .tid files, or a single .json file, that TiddlyWiki can reconstitute into tiddlers.

This is a very niche application, and is not prepared for general use, but may contain information that helps someone else in their niche exploration. More beginner-level notes, chiefly on making database queries within a Jupyter notebook using the `sqlite3` module, at http://chrisnicoll.net/2020/02/exploring-an-sqlite-database-from-jupyter-notebook/
