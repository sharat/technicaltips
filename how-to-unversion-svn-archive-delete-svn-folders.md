#How to cleanup your SVN archive (delete all .svn and unversion)?

You can find lot of scripts or you can simply remove .svn folder recursively. But there's a really handy way to do this with `TortoiseSVN`. 

Just use `Export` option in the context menu. You can export to a destination an unversioned copy of the working copy. If you give the export path same as the current folder, it will remove all the `.svn` folders recursively within the working copy (make the folder unversioned).
