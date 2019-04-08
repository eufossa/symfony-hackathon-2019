# Doctrine Project achievements

## Automatic releases

We managed to automate the release and maintenance process for most of
the projects under [Doctrine organisation](https://github.com/doctrine/).

The result of our design and implementation is currently available for
public review in the [`doctrine/automatic-releases`](https://github.com/doctrine/automatic-releases)
repository.

Thanks to this development, we will (over the next few weeks) be able to:

- merge multiple dozen pull requests that have been pending due to
  current maintenance availability restrictions
- automatically prepare releases for those merges
- automatically port these patches into newer versions of `doctrine/*`
  libraries.

In addition to that, we will reduce the learning curve needed for new
maintainers to join the project.

## DoctrineBundle achievements

For the DoctrineBundle we focused on finishing integration of new features for
Symfony 4.3, like transports for the Messenger component and a loader
for validation of entities based on Doctrine Mappings. Among the new features is
better support for configuring caches, and lazy-loading entity listeners by
default.

A group of people discussed possible options to split the bundle in two parts
for integration of DBAL and ORM as separate bundles. This would make using DBAL
only more seamless, especially in combination with Symfony Flex recipes.
