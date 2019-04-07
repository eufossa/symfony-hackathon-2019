# Symfony Messenger achievements

|                          | Total |
| ------------------------ | ----- |
| Merged Pull Requests     |  14   |
| Opened PRs (remaining)   |   4   |
| Closed Issues            |  12   |


We managed to create, test and merge numerous features, including (not exhaustive):

- Configuration of AMQP transport is now much more flexible thanks to the `AmqpStamp` (https://github.com/symfony/symfony/pull/30008 & https://github.com/symfony/symfony/pull/30913). It also allows us to bind multiple queues to a single exchange 🚀
- In case of multiple handlers for a given message, we track which handler has been successfully executed to when retrying, we will only re-run the failed handler(s) (https://github.com/symfony/symfony/pull/30020).
- An new (`in-memory://`) transport has been introduced (https://github.com/symfony/symfony/pull/29097).
- The very fresh Doctrine transport has been improved (https://github.com/symfony/symfony/pull/30858, https://github.com/symfony/symfony/pull/30805).

Even more impressive, we have managed to start tackling the following topics (expected to be merged within the following days):

- Message routing control at handler level, allowing much more complex and customised asynchronous setups (https://github.com/symfony/symfony/pull/30958).
- Incredible "failed messages" management feature which drastically improves the "ops" experience after failures (https://github.com/symfony/symfony/pull/30970).
- Redis transport relying on streams (https://github.com/symfony/symfony/pull/30917).
