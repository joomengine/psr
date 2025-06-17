### JCB! Power
# interface CacheItemInterface (Details)
> namespace: **VDM\Psr\Cache**

```uml
@startuml

interface CacheItemInterface  #Lavender {
  + getKey() : string
  + get() : mixed
  + isHit() : bool
  + set(mixed $value) : static
  + expiresAt(?\DateTimeInterface $expiration) : static
  + expiresAfter(int|\DateInterval|null $time) : static
}

note right of CacheItemInterface::getKey
  Returns the key for the current cache item.
The key is loaded by the Implementing Library, but should be available to
the higher level callers when needed.
The key string for this cache item.

  return: string
end note

note right of CacheItemInterface::get
  Retrieves the value of the item from the cache associated with this object's key.
The value returned must be identical to the value originally stored by set().
If isHit() returns false, this method MUST return null. Note that null
is a legitimate cached value, so the isHit() method SHOULD be used to
differentiate between "null value was found" and "no value was found."
The value corresponding to this cache item's key, or null if not found.

  return: mixed
end note

note right of CacheItemInterface::isHit
  Confirms if the cache item lookup resulted in a cache hit.
Note: This method MUST NOT have a race condition between calling isHit()
and calling get().
True if the request resulted in a cache hit. False otherwise.

  return: bool
end note

note right of CacheItemInterface::set
  Sets the value represented by this cache item.
The $value argument may be any item that can be serialized by PHP,
although the method of serialization is left up to the Implementing
Library.
The serializable value to be stored.
The invoked object.

  return: static
end note

note right of CacheItemInterface::expiresAt
  Sets the expiration time for this cache item.
The point in time after which the item MUST be considered expired.
If null is passed explicitly, a default value MAY be used. If none is set,
the value should be stored permanently or for as long as the
implementation allows.
The called object.

  return: static
end note

note right of CacheItemInterface::expiresAfter
  Sets the expiration time for this cache item.
The period of time from the present after which the item MUST be considered
expired. An integer parameter is understood to be the time in seconds until
expiration. If null is passed explicitly, a default value MAY be used.
If none is set, the value should be stored permanently or for as long as the
implementation allows.
The called object.

  return: static
end note

@enduml
```

The **Power** feature in JCB allows you to write PHP classes and their implementations,
making it easy to include them in your Joomla project. JCB handles linking, autoloading,
namespacing, and folder structure creation for you.

By using the **SPK** (Super Power Key) in your custom code (replacing the class name
in your code with the SPK), JCB will automatically pull the Power from the repository
into your project. This makes it available in your JCB instance, allowing you to edit
and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in
namespacing to prevent collisions and improve reusability across different JCB systems.

You can also set the **JCB powers path** globally or per component under the
**Dynamic Integration** tab, providing flexibility and maintainability.

To add this specific Power to your project in JCB:

> Simply use this SPK:
```
Super---171fcb39_ae27_4c2b_b091_2f70b824288b---Power
```
> Remember to replace the `---` with `___` to activate this Power in your code.

### Used in [Joomla Component Builder](https://www.joomlacomponentbuilder.com) - [Source](https://git.vdm.dev/joomla/Component-Builder) - [Mirror](https://github.com/vdm-io/Joomla-Component-Builder) - [Download](https://git.vdm.dev/joomla/pkg-component-builder/releases)

---
[![Joomla Volunteer Portal](https://img.shields.io/badge/-Joomla-gold?logo=joomla)](https://volunteers.joomla.org/joomlers/1396-llewellyn-van-der-merwe "Join Llewellyn on the Joomla Volunteer Portal: Shaping the Future Together!") [![Octoleo](https://img.shields.io/badge/-Octoleo-black?logo=linux)](https://git.vdm.dev/octoleo "--quiet") [![Llewellyn](https://img.shields.io/badge/-Llewellyn-ffffff?logo=gitea)](https://git.vdm.dev/Llewellyn "Collaborate and Innovate with Llewellyn on Git: Building a Better Code Future!") [![Telegram](https://img.shields.io/badge/-Telegram-blue?logo=telegram)](https://t.me/Joomla_component_builder "Join Llewellyn and the Community on Telegram: Building Joomla Components Together!") [![Mastodon](https://img.shields.io/badge/-Mastodon-9e9eec?logo=mastodon)](https://joomla.social/@llewellyn "Connect and Engage with Llewellyn on Joomla Social: Empowering Communities, One Post at a Time!") [![X (Twitter)](https://img.shields.io/badge/-X-black?logo=x)](https://x.com/llewellynvdm "Join the Conversation with Llewellyn on X: Where Ideas Take Flight!") [![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github)](https://github.com/Llewellynvdm "Build, Innovate, and Thrive with Llewellyn on GitHub: Turning Ideas into Impact!") [![YouTube](https://img.shields.io/badge/-YouTube-ff0000?logo=youtube)](https://www.youtube.com/@OctoYou "Explore, Learn, and Create with Llewellyn on YouTube: Your Gateway to Inspiration!") [![n8n](https://img.shields.io/badge/-n8n-black?logo=n8n)](https://n8n.io/creators/octoleo "Effortless Automation and Impactful Workflows with Llewellyn on n8n!") [![Docker Hub](https://img.shields.io/badge/-Docker-grey?logo=docker)](https://hub.docker.com/u/llewellyn "Llewellyn on Docker: Containerize Your Creativity!") [![Open Collective](https://img.shields.io/badge/-Donate-green?logo=opencollective)](https://opencollective.com/joomla-component-builder "Donate towards JCB: Help Llewellyn financially so he can continue developing this great tool!") [![GPG Key](https://img.shields.io/badge/-GPG-blue?logo=gnupg)](https://git.vdm.dev/Llewellyn/gpg "Unlock Trust and Security with Llewellyn's GPG Key: Your Gateway to Verified Connections!")