```
███████╗██╗   ██╗██████╗ ███████╗██████╗
██╔════╝██║   ██║██╔══██╗██╔════╝██╔══██╗
███████╗██║   ██║██████╔╝█████╗  ██████╔╝
╚════██║██║   ██║██╔═══╝ ██╔══╝  ██╔══██╗
███████║╚██████╔╝██║     ███████╗██║  ██║
╚══════╝ ╚═════╝ ╚═╝     ╚══════╝╚═╝  ╚═╝
██████╗  ██████╗ ██╗    ██╗███████╗██████╗ ███████╗
██╔══██╗██╔═══██╗██║    ██║██╔════╝██╔══██╗██╔════╝
██████╔╝██║   ██║██║ █╗ ██║█████╗  ██████╔╝███████╗
██╔═══╝ ██║   ██║██║███╗██║██╔══╝  ██╔══██╗╚════██║
██║     ╚██████╔╝╚███╔███╔╝███████╗██║  ██║███████║
╚═╝      ╚═════╝  ╚══╝╚══╝ ╚══════╝╚═╝  ╚═╝╚══════╝
```

### What is JCB Super Powers?
The Joomla Component Builder (JCB) Super Power features are designed to enhance JCB's functionality and streamline the development process. These Super Powers enable developers to efficiently manage and share their custom powers across multiple JCB instances through repositories hosted on [https://git.vdm.dev/[username]/[repository-name]](https://git.vdm.dev). JCB Super Powers are managed using a combination of layers, events, tasks, methods, switches, and algorithms, which work together to provide powerful customization and extensibility options. More details on JCB Super Powers can be found in the [Super Powers Documentation](https://git.vdm.dev/joomla/super-powers/wiki).

In summary, JCB Super Powers offer a flexible and efficient way to manage and share functionalities between JCB instances. By utilizing a sophisticated system of layers, events, tasks, methods, switches, and algorithms, developers can seamlessly integrate JCB core powers and their custom powers. For more information on how to work with JCB Super Powers, refer to the [Super Powers User Guide](https://git.vdm.dev/joomla/super-powers/wiki).

### What can I find here?
This repository contains an index (see below) of all the approved powers within the JCB GUI. During the compilation of a component, these powers are automatically added to the repository, ensuring a well-organized and accessible collection of functionalities.

# Index of powers

- **Namespace**: [VDM\Psr\Cache](#vdm-psr-cache)

  - **interface CacheItemInterface** | [Details](src/171fcb39-ae27-4c2b-b091-2f70b824288b) | [Code](src/171fcb39-ae27-4c2b-b091-2f70b824288b/code.php) | [Settings](src/171fcb39-ae27-4c2b-b091-2f70b824288b/settings.json) | Super__171fcb39_ae27_4c2b_b091_2f70b824288b__Power

# Class Diagrams

## VDM Psr Cache
> namespace VDM\Psr\Cache
```uml
@startuml

namespace VDM\Psr\Cache #DarkCyan {


  interface CacheItemInterface  #Lavender {
    + getKey() : string
    + get() : mixed
    + isHit() : bool
    + set() : static
    + expiresAt() : static
    + expiresAfter() : static
  }
}


@enduml
```


---
```
     ██╗ ██████╗  ██████╗ ███╗   ███╗██╗      █████╗
     ██║██╔═══██╗██╔═══██╗████╗ ████║██║     ██╔══██╗
     ██║██║   ██║██║   ██║██╔████╔██║██║     ███████║
██   ██║██║   ██║██║   ██║██║╚██╔╝██║██║     ██╔══██║
╚█████╔╝╚██████╔╝╚██████╔╝██║ ╚═╝ ██║███████╗██║  ██║
 ╚════╝  ╚═════╝  ╚═════╝ ╚═╝     ╚═╝╚══════╝╚═╝  ╚═╝
 ██████╗ ██████╗ ███╗   ███╗██████╗  ██████╗ ███╗   ██╗███████╗███╗   ██╗████████╗
██╔════╝██╔═══██╗████╗ ████║██╔══██╗██╔═══██╗████╗  ██║██╔════╝████╗  ██║╚══██╔══╝
██║     ██║   ██║██╔████╔██║██████╔╝██║   ██║██╔██╗ ██║█████╗  ██╔██╗ ██║   ██║
██║     ██║   ██║██║╚██╔╝██║██╔═══╝ ██║   ██║██║╚██╗██║██╔══╝  ██║╚██╗██║   ██║
╚██████╗╚██████╔╝██║ ╚═╝ ██║██║     ╚██████╔╝██║ ╚████║███████╗██║ ╚████║   ██║
 ╚═════╝ ╚═════╝ ╚═╝     ╚═╝╚═╝      ╚═════╝ ╚═╝  ╚═══╝╚══════╝╚═╝  ╚═══╝   ╚═╝
██████╗ ██╗   ██╗██╗██╗     ██████╗ ███████╗██████╗
██╔══██╗██║   ██║██║██║     ██╔══██╗██╔════╝██╔══██╗
██████╔╝██║   ██║██║██║     ██║  ██║█████╗  ██████╔╝
██╔══██╗██║   ██║██║██║     ██║  ██║██╔══╝  ██╔══██╗
██████╔╝╚██████╔╝██║███████╗██████╔╝███████╗██║  ██║
╚═════╝  ╚═════╝ ╚═╝╚══════╝╚═════╝ ╚══════╝╚═╝  ╚═╝
```
> Build with [Joomla Component Builder](https://git.vdm.dev/joomla/Component-Builder)

