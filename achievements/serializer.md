# Symfony Serializer Refactoring Plan

The symfony/serializer component has several normalizer implementations which are rather redundant and hard to maintain. The idea is to refactor the whole process of translating between array and objects and back and rely on PropertyAccess for the logic of how to interact with objects. The discussion is summarized at https://github.com/symfony/symfony/issues/30818.

EUFOSSA Hackathon helps us a lot to validate this discussion, and began the refactoring of the serializer, here is a detailed list on what we have achieved in regards to the plan during this two days:

## Tests - In review

We refactored the tests so that we can ensure a consistent behaviour and test the new normalizer when it is implemented. In that process, we found a couple of bugs that we fixed in Symfony 3.4 where applicable, and 4.2 for newer features.

See https://github.com/symfony/symfony/pull/30888

## Properties extraction - Merged

A new extension point was provided to be able to extract properties from an object (and not only for a class). This is needed in order to implement future behaviour that need the data of the object to filter the property list.

A default implementation using the `PropertyListExtractorInterface` was provided.

This new extension point has been added under the `@experimental` flag in order to be safe about BC policy if we need to change something

See https://github.com/symfony/symfony/pull/30904

## Instantiator - WIP

A new interface, and default implementation was added in order to instantiate objects when denormalizing. This can provide a new extension point to allow creating object without constructors, or using doctrine to instantiate an object like it's done in API Platform.

There is still some points to cover in order to be BC on the behaviour of the current normalizers.

See https://github.com/symfony/symfony/pull/30956

## Accessor and mutator extraction - In review

A pull request was created some days / week ago in order to extract read and write information on a property for a class. Extra work was added to this pull request in order to use this new system into the property access component.

See https://github.com/symfony/symfony/pull/30704

## New normalizer - WIP

A draft pull request was created in order to see the big picture about this new normalizer system.

See https://github.com/symfony/symfony/pull/30960

## Properties extraction implementations - WIP

Some implementations were done on the new extraction system, a draft PR was created where it currently support:

 * Allowing attributes (`attributes` context key in existing normalizer)
 * Ignoring attributes (`ignored_attributes` context key in existing normalizer)
 
See https://github.com/symfony/symfony/pull/30980

# Final words

Other features and fixes were done on the serializer, like adding the possibility to populate object on childs, and fixes about inccorrect cache when using ignored attributes.

Thanks to all people that have work on this, it's not done yet and will be continued but we make some huge steps forward having a rock solid normalization flow.
