# Technical Documentation

## `note-create`

This simple script facilitates creating of notes in a dated folder structure.

Running this:

```
$ ./note-create This is my first note
```

reated a file with this content:

```
Title: This is my first note
Author: pete
Date Created: 2024-01-05 19:55:21:373897000


```

After adding some text and saving it, the file was stored at:

```
/Users/pete/notes/2024/01/05/2024-01-05.19.55.21.373897000_This_is_my_first_note.txt
``` 

The utility allows for not specifying a title, in which case it will let you fill in the title
and then will calculate the filename afterwards.

This could be easily extended to use a template, which might be nice.

## `email-extract`

This script will simply parse an MBOX formatted file and spit out some of the pertenent data.

The thought here being that one possibly could use email as the communications mechanism, with the right
tools to extract / search the files directly.

Use like this:

```
$ ./email-extract <MBOX filename>
```

On my Mac using the built-in mail client, these files are located in `~/Libraray/Mail`.
