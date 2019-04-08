# API Platform Project achievements

This weekend we were multiple contributors to API Platform, some of the core team were here too to help in the hackathon.
When it comes to **API Platform** we just merge 20 PR, 10 new opened PR, 87 closed issues and 4 news. Lots of word being done from the old and the new contributors, big kudos !!

Since 2 years from now, API Platform supports subresources, this features does give access to include relation in the relation, this feature is used a lot and is very interesting, but since it's has alot of complexity and limited.

With the help of @vincentchalamon, @soyuka & @torreytsui, we made some research on how to improve the subresources. How to reduce the complexity of the implementation, the management of collection is very important for us.

Thanks to @jewome62, it's now possible to populate an object recursively with the serializer, to normalize a DateTimeZone object, and to get an instanciated object from an associative array of values.

@soyuka did a lot to close stale issues, along with @vincentchalamon.

@gregoirehebert fixed the fact the cache was still purged even if there was no get operation on an ApiResource. and bring you a way to switch version for the documentation.

@Deuchnord for his part worked on the client generator, you'll be able soon to use mercure on the vuejs generated client.

@alanpoulain worked on multiple things about graphQL, documentation and mongodb, and the event system of API Platform:
 	
 	- Relay Input Object Mutations Specification was not fully respected: https://facebook.github.io/relay/graphql/mutations.htm#sec-Mutation-inputs.
    - Input messenger was not tested with MongoDB.
    - Improve the contributing documentation.
    - Issue when 2.4 has been merged.
    - Internal events see https://github.com/api-platform/core/pull/2506
    
    
@jfthuillier Worked on the documentation on how to override function in the admin. He also started a poc how to use the guesser from react-admin in API Platform Admin.

@antograssiot did work on multiple feature and fixtures: 
    
    Apply DenyAccessListener before deserialization
    Be more intelligent in determining property writable/readable link. 
    Adding behat tests
    WIP - Makes url generation strategy default Added an additional test for strict types validationvalue configurable
   
same for @toflar he did works on his own big fixtures, like some hard dependencies
   
    Added an additional test for strict types validation
    Removed hard dependencies on doctrine odm to run the tests
    [WIP] General batch endpoint 
    Added support for pagination parameters in subresource docs
    
@Nek did work on features and bugfixes:

    Ignore property that does not exist for interfaces (identifiers for interfaces)
    Fix error message in identifiers extractor 
    Resource resolver for inheritance
    
@soyuka did finish something @simperfit started improving ids management.        