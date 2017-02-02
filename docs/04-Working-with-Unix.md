# Working with Unix

## Self-Help

Each of the commands that we've discussed so far are thoroughly documented, and
you can view their documentation using the `man` command, where the first
argument to `man` is the command you're curious about. Let's take a look at the
documentation for `ls`:


```bash
man ls
```

```
LS(1)                     BSD General Commands Manual                    LS(1)

NAME
     ls -- list directory contents

SYNOPSIS
     ls [-ABCFGHLOPRSTUW@abcdefghiklmnopqrstuwx1] [file ...]

DESCRIPTION
     For each operand that names a file of a type other than directory, ls
     displays its name as well as any requested, associated information.  For
:
```

The controls for navigating `man` pages are the same as they are for `less`.
I often use `man` pages for quickly seraching for an option that I've forgotten.
Let's say that I forgot how to get `ls` to print a long list. After typring
`man ls` to open the page, type `/` in order to start a search. Then type the
word or phrase that you're searching for, in this case type in `long list` and
then press `Enter`. The page jumps to this entry:

```
     -l      (The lowercase letter ``ell''.)  List in long format.  (See below.)
             If the output is to a terminal, a total sum for all the file sizes is
             output on a line before the long listing.
```

Press the `n` key in order to search for the next occurance of the word, and if
you want to go the previous occurance type `Shift` + `n`. This method of
searching also works with `less`. When you're finished looking at a `man` page
type `q` to get back to the prompt.

The `man` command works wonderfully when you know which command you want to look
up, but what if you've forgotten the name of the command you're looking for? You
can use `apropos` to search all of the available commands and their
descriptions. For example let's pretend that I forgot the name of my favorite
command line text editor. You could type `apropos editor` into the command line
which will print a list of results:


```bash
apropos editor
```

```
## ed(1), red(1)            - text editor
## nano(1)                  - Nano's ANOther editor, an enhanced free Pico clone
## sed(1)                   - stream editor
## vim(1)                   - Vi IMproved, a programmers text editor
```

The second result is `nano` which was just on the tip of my tounge! Both `man`
and `apropos` are useful when a search is only a few keystrokes away, but if 
you're looking for detailed exmaples and explanations you're better off using 
a search engine if you have access to a web browser.

## Get Wild

## Search

## Make

## Control

## Configure