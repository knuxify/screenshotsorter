# Screenshot Sorter

This is a small bash application designed to sort screenshots into folders named YYYY-MM, kinda like ShareX. It also renames the files to "Screenshot_(rising number)". That behaviour can be cut out by commenting out one line.

It is reccomended to run this script at startup. Most modern DEs allow you to do so from their settings. If you want to run it manually, type in the command as normal and follow it with an `&`, for example `sorter.sh 5 ~/Pictures` becomes `sorter.sh 5 ~/pictures &`. This will allow you to continue using your shell as normal.

## Exit codes

0 - OK (but shouldn't happen, since this runs an infinite loop)
1 - some arguments are missing
2 - some arguments are incorrect (screenshot directory doesn't exist)