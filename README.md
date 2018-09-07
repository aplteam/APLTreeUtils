# APLTreeUtils

General utilities included/used by most members of the APLTree library.


## Overview

Many classes of the APLTree project `:Include` the namespace script `APLTreeUtils` and all applications of the APL-cation projects call functions in it.

That means that before you can fix successfully one of these classes you must make sure that the namespace script `APLTreeUtils` is already in the current workspace.

Note that all functions in `APLTreeUtils` are independent from `⎕IO` as well as `⎕ML`.

Although `APLTreeUtils` is designed to be included in classes there is nothing wrong with calling its functions from outside like this:

```
      APLTreeUtils.FindPath
```

## List of functions

```
FindPathTo              ⍝ Useful to find a certain script in the workspace.
FormatDateTime          ⍝ Formats one ⍺to many date.
GetOperatingSystem      ⍝ Takes `⍬` as right argument and returns a three-item vector like "Win", "AIX", "Mac" or "Lin".
GoToWebPage             ⍝ Fires up the default browser and displays the page specified as right argument.
IsChar                  ⍝ Returns a 1 if the right argument is of type Char.
IsDevelopment           ⍝ Returns a 1 if executed in a Unicode version of Dyalog.
IsUnicode               ⍝ Returns a 1 if executed in a Unicode version of Dyalog.
Last                    ⍝ Returns the extension from a full path. Separator ⍺ defaults to ".".
Lowercase               ⍝ Enforces lowercase for strings as well as a vector of strings.
Nest                    ⍝ Enclose if right argument is simple.
ReadUtf8File            ⍝ Return contents of a UTF8 file.
Split                   ⍝ Split string . Separator ⍺ defaults to CR+LF.
SplitPath               ⍝ Part Path from filename+extension. Separator ⍺ defaults to "\".
Uppercase               ⍝ Enforce uppercase for strings as well as a vector of strings.
Where                   ⍝ Returns indices for Boolean scalar or vector `⍵`.
WriteUtf8File           ⍝ Creates or overwrites a UTF8 file without BOM.
dlb                     ⍝ Delete leading blanks.
dmb                     ⍝ Delete multiple blanks.
dtb                     ⍝ Delete trailing blanks.
```