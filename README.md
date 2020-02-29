# NAME

Dist::Zilla::App::Command::coverh - Code coverage metrics, with history

<div>
    <p>
    <img src="https://img.shields.io/badge/perl-5.10.1+-blue.svg" alt="Requires Perl 5.10.1+" />
    <a href="https://travis-ci.org/Csson/p5-Dist-Zilla-App-Command-coverh"><img src="https://api.travis-ci.org/Csson/p5-Dist-Zilla-App-Command-coverh.svg?branch=master" alt="Travis status" /></a>
    <a href="http://cpants.cpanauthors.org/release/CSSON/Dist-Zilla-App-Command-coverh-0.0101"><img src="http://badgedepot.code301.com/badge/kwalitee/CSSON/Dist-Zilla-App-Command-coverh/0.0101" alt="Distribution kwalitee" /></a>
    <a href="http://matrix.cpantesters.org/?dist=Dist-Zilla-App-Command-coverh%200.0101"><img src="http://badgedepot.code301.com/badge/cpantesters/Dist-Zilla-App-Command-coverh/0.0101" alt="CPAN Testers result" /></a>
    <img src="https://img.shields.io/badge/coverage-19.1%-red.svg" alt="coverage 19.1%" />
    </p>
</div>

# VERSION

Version 0.0101, released 2020-02-29.

# SYNOPSIS

    $ dzil coverh
    $ dzil coverh --history

# DESCRIPTION

Dist::Zilla::App::Command::coverh is a command extension for [Dist::Zilla](https://metacpan.org/pod/Dist::Zilla). It provides the `coverh` command, which generates code coverage metrics (in json format)
for the current distribution using [Devel::Cover](https://metacpan.org/pod/Devel::Cover). It appends the summary to a `.coverhistory.json` file in the distribution root.

Tests must pass for this to work. Author and release tests are not run. No command-line arguments are passed on to
the `cover` command from [Devel::Cover](https://metacpan.org/pod/Devel::Cover).

## Options

### --history

Prints the contents of the log file:

    version date...... ...tot ..stmt ..bran ..cond ...sub ...pod
     0.0001 2016-01-16  25.8%  22.4%   0.0%   0.0%  66.7% 100.0%
     0.0002 2016-01-17  68.0%  79.8%  23.4%  19.4%  83.0% 100.0%

# NOTE

Depending on which VersionProvider is in use, the version number logged in the log file may or may not correspond to the version number
on cpan (for the same _version_ of the distribution).

Only the latest run of `coverh` for a certain version number is kept in the log file.

# SEE ALSO

- [Dist::Zilla::App::Command::cover](https://metacpan.org/pod/Dist::Zilla::App::Command::cover)
- [Devel::Cover](https://metacpan.org/pod/Devel::Cover)

# ACKNOWLEDGEMENTS

Some parts were borrowed from [Dist::Zilla::App::Command::cover](https://metacpan.org/pod/Dist::Zilla::App::Command::cover).

# SOURCE

[https://github.com/Csson/p5-Dist-Zilla-App-Command-coverh](https://github.com/Csson/p5-Dist-Zilla-App-Command-coverh)

# HOMEPAGE

[https://metacpan.org/release/Dist-Zilla-App-Command-coverh](https://metacpan.org/release/Dist-Zilla-App-Command-coverh)

# AUTHOR

Erik Carlsson <info@code301.com>

# COPYRIGHT AND LICENSE

This software is copyright (c) 2016 by Erik Carlsson.

This is free software; you can redistribute it and/or modify it under
the same terms as the Perl 5 programming language system itself.
