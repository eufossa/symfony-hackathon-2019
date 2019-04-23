# Flysystem - Symfony integration achievements

> By Titouan Galopin (@tgalopin)

In January 2018, I stumbled upon a problem with autowiring: how can one easily and 
efficiently autowire different implementations of the same interface? In my 
specific case, the problem was linked to the Flysystem library, in which having 
multiple different filesystems can happen often.

This problem lead to a vast conversation throughout 2018 with Nicolas Grekas and 
ultimately was the reason to introduce an idea of "semantics" using the param 
annotation ([#27172](https://github.com/symfony/symfony/pull/27172)).

However, this implementation had many issues and was not well suited to 
solve the problem. It was later closed when the introduction of named aliases 
solved the problem much more elegantly 
([#28234](https://github.com/symfony/symfony/pull/28234)). This feature was released in 
Symfony 4.2, in November 2018, and the hackathon was even the occasion for 
Grégoire Paris to write its documentation 
([#11339](https://github.com/symfony/symfony-docs/pull/11339)).

Now that named aliases are available, a much better integration with Flysystem 
could be achieved. This is one of the things I worked on during this hackathon: 
creating this integration, as an official Symfony bundle for Flysystem.

You can learn more details about this integration in the dedicated blog post:
[https://titouangalopin.com/introducing-the-official-flysystem-bundle/](https://titouangalopin.com/introducing-the-official-flysystem-bundle/).
