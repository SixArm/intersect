# The `intersect` command for Unix text processing

Print the lines that are in all of the inputs.

Syntax:

    intersect <input> ...

Example:

    $ intersect 1.txt 2.txt
    => lines that are in both of the files.


## Notes

The order doesn't matter.

In set theory, this command is (A intersect B).

This command is currently implemented using `awk` and POSIX.


## Related

Related commands for Unix text processing sets:

* [`union`](https://github.com/sixarm/union): print lines in (A union B)
* [`intersect`](https://github.com/sixarm/intersect): print lines in (A intersect B)
* [`except`](https://github.com/sixarm/except): print lines in (A except B) a.k.a. (A - B)
* [`extra`](https://github.com/sixarm/extra) : print lines in (A extra B) a.k.a. (B - A)

Examples:

    $ cat 1.txt
    alpha
    bravo

    $ cat 2.txt
    alpha
    charlie

    $ union a.txt b.txt
    alpha
    bravo
    charlie

    $ intersect a.txt b.txt
    alpha

    $ except a.txt b.txt
    bravo

    $ extra a.txt b.txt
    charlie


## Tracking

* Program: intersect
* Version: 2.0.2
* Created: 2017-01-30
* Updated: 2017-01-30
* License: GPL
* Contact: Joel Parker Henderson (joel@joelparkerhenderson.com)
