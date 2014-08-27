PHP_CodeSniffer
===============

About
-----

PHP\_CodeSniffer is a PHP5 script that tokenises PHP, JavaScript and CSS files to detect violations of a defined coding standard. It is an essential development tool that ensures your code remains clean and consistent. It can also help prevent some common semantic errors made by developers.

Requirements
------------

PHP\_CodeSniffer requires PHP version 5.1.2 or greater, although individual sniffs may have additional requirements such as external applications and scripts. See the [Configuration Options manual page](http://pear.php.net/manual/en/package.php.php-codesniffer.config-options.php) for a list of these requirements.

The SVN pre-commit hook requires PHP version 5.2.4 or greater due to its use of the vertical whitespace character.


Documentation
-------------

The documentation for PHP\_CodeSniffer is available on the [Github wiki](https://github.com/squizlabs/PHP_CodeSniffer/wiki).

Information about upcoming features and releases is available on the [Squiz Labs blog](http://www.squizlabs.com/php-codesniffer).

Contributing
-------------

If you do contribute code to PHP\_CodeSniffer, please make sure it conforms to the PEAR coding standard and that the PHP\_CodeSniffer unit tests still pass. The easiest way to contribute is to work on a checkout of the repository, or your own fork, rather than an installed PEAR version. If you do this, you can run the following commands to check if everything is ready to submit:

    cd PHP_CodeSniffer
    php scripts/phpcs --ignore=*/tests/* . -n

Which should give you no output, indicating that there are no PEAR coding standard errors. And then:

    phpunit tests/AllTests.php

Which should give you no failures or errors. You can ignore any skipped tests as these are for external tools.

Issues
------

Bug reports and feature requests can be submitted on the [PEAR bug tracker](http://pear.php.net/package/PHP_CodeSniffer/bugs).
