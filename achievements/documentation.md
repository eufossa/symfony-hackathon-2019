# Documentation

The EU-FOSSA hackathon allowed us to, for the first time ever, gather
4 of the doc team members together to work on the documentation. Also,
by combining the doc team with all code contributors, we managed to
help code contributors to write doc PRs for their contributions. Being
able to directly help people understand the reStructuredText syntax and
logics of writing docs was a huge help to get more features documented.

This resulted in a diverse set of work done. Below is a short summary
of all work done, but please have a look at [all GitHub issues and pull
requests](https://github.com/symfony/symfony-docs/pulls?q=label%3A"⭐️+EU-FOSSA+Hackathon")
handled during the weekend.

### Documenting Features that were Missing for Years

While Symfony puts lots of effort into documenting all new features,
it cannot be avoided that sometimes great features are missed. During the
weekend, new undocumented features were discovered in discussions between
contributors and time finally was found to add some more articles.

Among this, [@Toflar](https://github.com/Toflar) worked on [documenting the
changes in `.env` files in Symfony 4.2](https://symfony.com/doc/current/components/dotenv#usage)
While the recommendations changed (from `.env.dist` to `.env.local`), the
docs were never updated accordingly.

[@Nyholm](https://github.com/Nyholm) combined the knowledge of almost everyone
around to write a brand new [Cache guide](https://symfony.com/doc/current/cache.html).
As the component has changed quite often and involved many code contributors, we're
very happy there was finally an occasion where the documentors and code contributors
couuld combine their knowledge about this topic. This will be a great help for all futur
users of caching in Symfony!

At last, [@heahdude](https://github.com/heahdude) started all enthousiasm this
weekend by creating documentation for the
[Traverse constraint](https://symfony.com/doc/current/reference/constraints/Traverse.html).
This constraint was introduced in Symfony 2.5 (that's 5 years ago!) and I'm not sure if
anyone knew it even existed. Great to find this feature and have it documented now!

### Finishing old Pull Requests

The documentation has around 100 open PRs, most of which are open for months or even
years. During the hackathon, developers were encouraged to finish these old PRs.
[@llaakkkk](https://github.com/llaakkkk) worked on finishing a [new article on Message
Transports](https://github.com/symfony/symfony-docs/pull/11331), [@Toflar](https://github.com/Toflar)
finished [adding Doctrine ORM installation instructions](https://github.com/symfony/symfony-docs/pull/11332),
and some more old PRs were closed and fixed by doc team members with the help of
[@dbrumann](https://github.com/dbrumann), who focussed for the complete hackathon on
the docs.

### Documenting new Features

At the second day, the docs corner became quite busy, as all developers that created
new features on the first day wanted to directly document it. "A feature does not exists
without documentation" became reality this weekend! In total, 39 different authors created
61 pull requests during the weekend!

### The Hackathon ended, the Contributions did not!

The hackathon gave all participants lots of positive energy, something that became obvious
during the days after the hackathon. The stream of new PRs continued to be impressively high,
with over 24 new pull requests created at Monday (that almost equals the achievements of the
hackathon!). As new contributors have learned how to document their features, our hopes are
high that the documentation will receive more help from all contributors in the future!
