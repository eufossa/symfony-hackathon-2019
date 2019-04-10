# Box Achievements

[Humbug Box][box] is an application bundler for PHP apps. It allows one to ship a PHP app into a PHAR and distribute it with 
ease.

Over the last few months, Box has been growing in popularity especially within the [Laravel][laravel] community thanks to the
[Laravel Zero][laravel-zero] framework, a spin-off of Laravel more focused on CLI applications.

In contrast, while Box is being used a lot with projects making use of [Symfony][symfony] components, it cannot be used, at
least easily with a standard Symfony application.

Thanks to this hackathon, [I][me] could, besides working on other Symfony related issues, and with the help of 
[@nicolas-grekas][nicolas], [@stof][stof] and [@tucksaun][tucksaun], work on adding support for Symfony to Box.

The result was:

- The release of [Box 3.7.0][box-3.7.0]
- 11 issues closed
- 14 pull requests

This work also resulted directly into:

- 2 pull requests made on the Symfony repositories (recipes & core) regarding the CLI guards within the Symfony codebase
- Adding additional screening on Symfony regarding the [HTTPoxy][httpoxy] vulnerability (no security issue found during the process)
- 1 issue with a reproducer regarding the [Symfony Console component][symfony-console]
- 1 issue reproduced and solved for the [Symfony CLI tool][symfony-cli]

Also, more discussions have been made on how to integrate a [REPL][repl] to Symfony with minimal dependencies (which has been
a recurring problem so far) thanks to [PsySH][psysh] and [Box][box].


[box]: https://github.com/humbug/box
[laravel]: http://laravel.com
[laravel-zero]: https://laravel-zero.com/
[symfony]: https://symfony.com/
[me]: https://github.com/theofidry
[nicolas]: https://github.com/nicolas-grekas
[tucksaun]: https://github.com/tucksaun
[box-3.7.0]: https://github.com/humbug/box/releases/tag/3.7.0
[httpoxy]: https://httpoxy.org
[symfony-console]: https://symfony.com/doc/current/components/console.html
[repl]: https://es.wikipedia.org/wiki/REPL
[psysh]: https://psysh.org/
[symfony-cli]: https://symfony.com/cloud/

