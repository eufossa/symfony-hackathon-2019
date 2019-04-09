# API Platform Project achievements

During the hackathon multiple API Platform contributors were present, some of them from the core team and available to help others.

When it comes to **API Platform** we *merged 20 PR, opened 10 new PR, closed 87 issues and opened 4 new*. Lots of work being done by the contributors, big kudos!!

Since 2 years ago, API Platform supports subresources, which allows to access a relation from a resource.
It is used a lot and is very powerful, but it has a lot of complexity and is limited.

With the help of [@vincentchalamon](https://github.com/vincentchalamon), [@soyuka](https://github.com/soyuka) and [@torreytsui](https://github.com/torreytsui), some research was made on how to improve the subresources by reducing the complexity of the implementation and by enabling the POST/PUT operations for the subresources (<https://github.com/api-platform/core/pull/2598>, <https://github.com/api-platform/core/pull/2428>).

Thanks to [@jewome62](https://github.com/jewome62), it's now possible to populate an object recursively with the serializer to normalize a `DateTimeZone` object, and to get an instanciated object from an associative array of values.

[@soyuka](https://github.com/soyuka) did a lot to close stale issues, along with [@vincentchalamon](https://github.com/vincentchalamon).

[@gregoirehebert](https://github.com/gregoirehebert) fixed an issue where the cache was still purged even if there was no GET operation on an ApiResource, and added a way to switch the API Platform version for the documentation (<https://github.com/api-platform/website/pull/103>).

[@Deuchnord](https://github.com/Deuchnord) worked on the client generator, you'll be able to use Mercure on the Vue.js generated client soon.

[@alanpoulain](https://github.com/alanpoulain) worked on multiple things about GraphQL, MongoDB, and the event system of API Platform:

- The event system is being reworked to have internal events in API Platform instead of being based on the Symfony ones. It will allow to be decoupled from Symfony and to add events for GraphQL (<https://github.com/api-platform/core/pull/2506>)
- Relay Input Object Mutations Specification (GraphQL) was not fully respected (<https://github.com/api-platform/core/pull/2696>)
- Input messenger was not tested with MongoDB
- Improve the contributing documentation

[@jfthuillier](https://github.com/jfthuillier) worked on the documentation on how to customize easily the API Platform admin. He also started a PoC on how to use the guesser from react-admin in API Platform Admin.

[@antograssiot](https://github.com/antograssiot) did work on multiple features and fixes: 

- Apply DenyAccessListener before deserialization
- Be more intelligent in determining property writable/readable link
- Makes URL generation strategy default value configurable

Same for [@toflar](https://github.com/toflar) who worked on his great improvements, like removing some hard dependencies:

- Added an additional test for strict types validation
- Removed hard dependencies on Doctrine ODM to run the tests
- Worked on a proposition for a general batch endpoint
- Added support for pagination parameters in subresource docs

[@Nek](https://github.com/Nek-) worked on features and bugfixes:

- Ignore property that does not exist for interfaces (identifiers for interfaces)
- Fix error message in identifiers extractor
- Resource resolver for inheritance

[@soyuka](https://github.com/soyuka) finished something [@simperfit](https://github.com/simperfit) started improving IDs management.
