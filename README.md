# latexmk-clear-test
Testing the `latexmk -c` after `latexmk -pdf` for bugfixing, tested with latexmk-4.43a

To reproduce the bug, run

    latexmk -pdf

then

    latexmk -C

Leaves behind `content/Chapter1.aux` and `content/Chapter2.aux`

Running

    latexmk

and then

    latexmk -C

correctly cleans everything.
