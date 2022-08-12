# SFM

**WARNING**: SFM is still in development, it lacks a lot of essential features
to make a good file explorer. Use it as a simple way to browse, open, rename
and delete files.

- Stands for **S**imple **F**ile **M**anager
- Inspired by [ranger](https://github.com/ranger/ranger)
- Vim keybindings
- Fast and minimal.
- Written in C++ using the ncurses library
 
![screenshot](sfm.png)

## Installation

```
git clone git@github.com:berimbo/sfm.git
cd sfm
make install
```
 
## Keybindings

| Key                | Function                          |
| :---:              | ---                               |
| <kbd>h j k l</kbd> | Navigation keys                   |
| <kbd>G</kbd>       | Go to end                         |
| <kbd>g</kbd>       | Go to top                         |
| <kbd>space</kbd>   | Add/Remove to/from selection list |
| <kbd>d</kbd>       | Move files to trash               |
| <kbd>r</kbd>       | Rename a file                    |
| <kbd>.</kbd>       | Toggle hidden files               |
| <kbd>q</kbd>       | Quit                              |

## xdg-open configuration example

SFM uses xdg-open to find the appropriate program to open the files. 

```
xdg-mime default nvim.desktop text/plain
xdg-mime default nvim.desktop application/json
xdg-mime default sxiv.desktop image/png
xdg-mime default sxiv.desktop image/jpeg
xdg-mime default nvim.desktop text/xml
xdg-mime default mpv.desktop audio/mpeg
xdg-mime default org.pwmt.zathura.desktop application/pdf
```
