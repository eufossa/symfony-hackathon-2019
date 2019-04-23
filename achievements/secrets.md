# Symfony Secrets

The EU-FOSSA hackathon was the opportunity to discuss and define a simple
and flexible solution to use sensitive informations (like passwords,
authentication keys, ...) in a Symfony application.

It solves the following common issue:

> How to define new sensitive parameters without exposing them in a
  repository, nor configuring manually a server each time the projet requires
  a new env variable

Thanks to [@mpdude](https://github.com/mpdude), [@tobion](https://github.com/tobion),
[@nicolas-grekas](https://github.com/nicolas-grekas) and [@jderusse](https://github.com/jderusse),
we defined the use cases that would be covered by that new feature, we designed the main
interfaces and ended with a working Proof of Concept.

This subject was in initialized in [the RFC issue](https://github.com/symfony/symfony/issues/27351),
during the hackathon, [@mpdude](https://github.com/mpdude) wrote
[a nice blog post](https://www.webfactory.de/blog/storing-secrets-for-symfony-applications)
diging into that topic.