# Pit
Source control for binary files via Google Drive

## Installation
You need [ruby](https://www.ruby-lang.org/en/) and [gdrive](https://github.com/prasmussen/gdrive).
Copy the pit file into a directory that's in your `PATH`.

## Cloning a Drive directory with pit
Find the directory you want to clone in the Google Drive website and open it.
In the URL, you'll notice a long id at the end, like this:

`https://drive.google.com/drive/u/0/folders/<suspiciously-long-hash>`

Copy it, and then open the terminal. Go to the directory you want to download into, and do:

`pit clone <suspiciously-long-hash>`

Likewise for `pit init`.

### Why 'pit'?
Because it looks like git, but it's more like throwing your files in a pit.

### Why does it exist?
We were trying to do a collab in Unreal Engine 4, and we used git.
However, UE4's assets are binary files, and git keeps a copy for every version of a binary. So we reached our disk quota fast.
And after a week of procrastination and bad decisions, pit was magically born.
