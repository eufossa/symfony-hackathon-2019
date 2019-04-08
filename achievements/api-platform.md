# API Platform Project achievements

During the hackathon multiple API Platform contributors were present, some of them from the core team and available to help others.

When it comes to **API Platform** we *merged 20 PR, opened 10 new PR, closed 87 issues and opened 4 new*. Lots of work being done from the contributors, big kudos !!

Since 2 years from now, API Platform supports subresources, which allows to access a relation from another.
It is used a lot and is very powerful, but since it has a lot of complexity and is limited.

With the help of @vincentchalamon, @soyuka & @torreytsui, we made some research on how to improve the subresources. How to reduce the complexity of the implementation, the management of collection is very important for us.

Thanks to @jewome62, it's now possible to populate an object recursively with the serializer, to normalize a DateTimeZone object, and to get an instanciated object from an associative array of values.

@soyuka did a lot to close stale issues, along with @vincentchalamon.

@gregoirehebert fixed the fact the cache was still purged even if there was no GET operation on an ApiResource, and added a way to switch version for the documentation.

@Deuchnord for his part worked on the client generator, you'll be able soon to use Mercure on the Vue.js generated client.

@alanpoulain worked on multiple things about graphQL, documentation and mongodb, and the event system of API Platform:
 	
- Relay Input Object Mutations Specification was not fully respected: https://facebook.github.io/relay/graphql/mutations.htm#sec-Mutation-inputs
- Input messenger was not tested with MongoDB
- Improve the contributing documentation
- Issue when 2.4 has been merged
- Internal events see https://github.com/api-platform/core/pull/2506

@jfthuillier Worked on the documentation on how to override function in the admin. He also started a PoC on how to use the guesser from react-admin in API Platform Admin.

@antograssiot did work on multiple features and fixtures: 

- Apply DenyAccessListener before deserialization
- Be more intelligent in determining property writable/readable link
- Adding behat tests
- WIP - Makes url generation strategy default
- Added an additional test for strict types validationvalue configurable

Same for @toflar who worked on his own big fixtures, like some hard dependencies:

- Added an additional test for strict types validation
- Removed hard dependencies on Doctrine ODM to run the tests
- Worked on a proposition for a general batch endpoint
- Added support for pagination parameters in subresource docs

@Nek worked on features and bugfixes:

- Ignore property that does not exist for interfaces (identifiers for interfaces)
- Fix error message in identifiers extractor
- Resource resolver for inheritance

@soyuka did finish something @simperfit started improving IDs management.
