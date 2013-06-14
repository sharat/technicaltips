
If you want to convert line ending of files in bulk, you can easily do it with following script.

```
#Convert from dos/unix to unix
 
#To convert from any mixture of CRLF endings and LF-only endings, to LF-only endings:[C 1]
:set hidden #Allow modified buffers to be hidden.
:set ffs=dos #Assume dos line endings (CRLF or LF-only) when reading files.
:args *.c *.h #Specify the files to convert.
:argdo set ff=unix|w #For each argument, set unix file format for the buffer, and write the file.[C 2]
 
#Convert from dos/unix to dos
 
#To convert from any mixture of CRLF endings and LF-only endings, to CRLF endings:[C 1]
:set ffs=dos #Assume dos line endings (CRLF or LF-only) when reading files.
:args *.c *.h #Specify the files to convert.
:argdo w #Write each file with CRLF line endings. 
```
