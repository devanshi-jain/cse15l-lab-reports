# Lab Report - 2

The given MarkdownParse.java file has been updated, specifically the following code additions to take care of certain coundary cases have been made.
First, we try fixing the error that shows up when you leave a blank line betwen two links:

```
if (currentLine.length() == 0) continue;
            // Ensure that line isn't an image
```
Link to test-file : https://github.com/devanshi-jain/markdown-parser/blob/main/test-3.md

Fro a test-file with no links, we try fixing it as follows.
```
if (args[0] == null) {
            throw new IOException("No file specified");
        }
```
Link to test-file : https://github.com/devanshi-jain/markdown-parser/blob/main/test-2.md

Finally, to fix the bug which is when a file contains an image reference : 

```
if (currentLine.charAt(0) == '!') continue;
```
Link to test-file : https://github.com/devanshi-jain/markdown-parser/blob/main/test-1.md
