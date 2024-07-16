```
██████╗  ██████╗ ██╗    ██╗███████╗██████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝
```
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

The Power feature in JCB allows you to write PHP classes and their implementations, making it easy to include them in your Joomla project. JCB handles linking, autoloading, namespacing, and folder structure creation for you.

By using the SPK (Super Power Key) in your custom code (replacing the class name in your code with the SPK), JCB will automatically pull the power from the repository into your project. This makes it available in your JCB instance, allowing you to edit it and include the class in your generated Joomla component.

JCB uses placeholders like [[[`NamespacePrefix`]]] and [[[`ComponentNamespace`]]] in namespacing to prevent collisions and improve reusability across different JCB systems. You can also set the **JCB powers path** globally or per component under the **Dynamic Integration** tab, providing flexibility and easy maintainability.

To add this specific Power to your project in JCB:

> simply use this SPK
```
Super---171fcb39_ae27_4c2b_b091_2f70b824288b---Power
```
> remember to replace the `---` with `___` to activate this Power in your code

---
```
     ██╗ ██████╗██████╗
     ██║██╔════╝██╔══██╗
     ██║██║     ██████╔╝
██   ██║██║     ██╔══██╗
╚█████╔╝╚██████╗██████╔╝
 ╚════╝  ╚═════╝╚═════╝
```
> Build with [Joomla Component Builder](https://git.vdm.dev/joomla/Component-Builder)

