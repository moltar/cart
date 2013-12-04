# NAME

cart - Helper script for running project scripts via plenv and Carton

# SYNOPSIS

    # Run project scripts from command line
    $ ./cart bin/script.pl --options

    # Install project scripts as cron
    * * * * * $HOME/project/cart bin/script.pl --options

# DESCRIPTION

This is a helper script that combines the efforts of two projects:

 * [plenv](https://github.com/tokuhirom/plenv/) - Perl binary manager
 * [carton](https://github.com/miyagawa/carton/) - Perl module dependency manager

This helper script sets up plenv environment variables and runs a given script
via plenv and carton.

Prior to running the command, it will change working directory to one where the
script itself is located.

Therefor it is necessary to put this script into the root of the project
alongside with `.perl-version` and `cpanfile`.

# INSTALLATION

    $ cd project/ ## chdir to your project root
    $ curl -Ls -o cart http://git.io/oF4Q_g && chmod 755 cart

# AUTHOR

Roman F.

# COPYRIGHT

Roman F. 2013

# LICENSE

This software is licensed under the same terms as Perl itself.

# SEE ALSO

 * [cpanfile](http://search.cpan.org/perldoc?cpanfile)
 * [plenv](https://github.com/tokuhirom/plenv/)
 * [carton](https://github.com/miyagawa/carton/)
