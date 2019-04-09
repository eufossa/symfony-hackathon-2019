# Symfony Security

On the subject of security we had some great discussions and research about the state of the
Symfony Security component as it is now. It has not received much love over the past years and
as such has quite some parts that would benefit from a fundamental overhaul. We had a good
look at what competing frameworks offer in this respect, mainly Java Spring Security as it
was the original inspiration for the component, and combined our thought on that with the
results of a recently conducted survey amongst Symfony developers of what they would like to
see.

As a result of the above we now have a central RFC issue tracking the wishlists and a global
task of what we should strive to achieve before Symfony 5.0 as it will cause some breakage.

[Click here for the RFC issue](https://github.com/symfony/symfony/issues/30914).

We also introduced a new password hasher built on top of [Libsodium](https://libsodium.gitbook.io/doc/), 
a software library implementing the `Argon2` function, winner of the [Password Hashing
Competition](https://password-hashing.net/).

[Click here for the Pull Request](https://github.com/symfony/symfony/pull/31019).
