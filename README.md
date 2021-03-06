README for fitnesse.vim (Version 0.1) / May 22 2009

  * INSTALLATION
  * RELEASE NOTES
  * CREDITS


fitnesse.vim is a syntax file (and eventually some filetype specific functions) 
for editing FitNesse tests using Vim.  It was created to make it easier to work
with fitnesse files.  It works great in conjunction with "It's All Text" a 
plugin for FireFox (found at https://addons.mozilla.org/en-US/firefox/addon/4125). 

FitNesse is a collaborative testing tool that uses Wiki markup to create test 
scripts as web pages.  See http://fitnesse.org for more information.

This release is very Slim centric.


INSTALLATION
------------------------

The files in the Zip file are stored in the same folders they need to be 
placed in under the vimfiles folder ( $HOME/.vim/ or %VIM%\vimfils depending
on your OS).

1) Unzip the fitnesse.vim.zip file to the vimfiles folder.  Unless you are 
   customizing the file, you should be OK to overwrite the files.
  
2) Syntax coloring support must be enabled. 
      
      You can do this by adding :syntax enable to your _vimrc or .vimrc file.

3) If you want automatic detection you will need to:

      a) Check to see if you have a scripts.vim file already in place.  This 
         file allows post loading checking of files to execute scripts.  

      b) If you do not have a scripts.vim file in your vimfiles folder, rename
         the scripts.vim.add file to scripts.vim.

      c) If you do have a scripts.vim file; open the scripts.vim.fitnesse_add 
         file and copy the text in that file to your scripts.vim file.

RELEASE NOTES
------------------------

Version 0.1:

   This release supports the following syntax:
      * Numerous keywords in Slim and FitNesse are supported:
         scenario, script, Query:, start, check, reject, show, Comment, comment, 
         !see, !include, !See, null, !define, !include
      * Simple collapsible sections (with folding enabled)  !** *!, !**> *!
      * Table cell delimiter "|"
      * Cell contents
      * Incomplete cell is error
      * !style_(class) 
      * Strings in Quotes
      * Scenario variables @parametername
      * Symbols $symbolname
      * Simple WikiWord support

CREDITS
------------------------

 * Bob Martin for FitNesse and Slim
 * Brett Schuchert for Recommending It's All Text
