# JCB! Super Powers

### What Are JCB Super Powers?
In simple terms, **JCB Super Powers are PHP classes** — but managed entirely from the Joomla Component Builder (JCB) interface.

You can use JCB to create your own:
- **Classes**
- **Interfaces**
- **Abstract classes**
- **Traits**
- **Final classes**

These are full-featured PHP code units that you define visually in the JCB GUI. JCB then takes care of:
- Proper **namespacing**
- Correct **file placement**
- Seamless **project integration**

Every Super Power is treated as a reusable unit of logic. It can be automatically injected into any part of your JCB-powered component, or used in other components or codebases via a **SPK** (Super Power Key).

Even better — you can use **dynamic placeholders** like [[[`NamespacePrefix`]]] or [[[`ComponentNamespace`]]] in your Super Power code Namespace. These automatically adapt when reused in different projects, making your logic portable and future-proof.

> In short: **Super Powers turn JCB into a PHP code factory** — giving you the power of advanced PHP with none of the manual file management.

To learn how to create, manage, and use Super Powers, see the  
[Super Powers Documentation →](https://git.vdm.dev/joomla/super-powers/wiki)

### What Can I Find Here?
This repository acts as a **central registry of approved Super Powers** specific to this JCB instance.  
Only the Super Powers that have been explicitly assigned to this repository are listed here.

In JCB, you can organize your Super Powers across multiple repositories.  
For example, we have separate repositories for:

- [GITEA](https://git.vdm.dev/joomla/gitea)-related classes
- [OpenAI](https://git.vdm.dev/joomla/openai) integrations
- Core [Super Power](https://git.vdm.dev/joomla/super-powers) collection
- and many more...

Each repository maintains its own index, and only the powers assigned to that specific repository will appear in its list.
#### How to Use These Super Powers
If you want to use any of the classes listed here in your own component logic, simply reference their **SPK** (Super Power Key):

```
Super---[unique-guid]---Power
```

> Replace each `---` with `___` when using the key inside your code.

JCB will automatically resolve this SPK during compilation, placing the associated class in the correct location with the correct namespace based on your component context.  
This makes your logic both **reusable** and **component-aware**, without hardcoding anything.

---
# Index of powers

- **Namespace**: [VDM\Psr\Cache](#vdm-psr-cache)

  - **interface CacheItemInterface** | [Details](src/171fcb39-ae27-4c2b-b091-2f70b824288b) | [Raw](src/171fcb39-ae27-4c2b-b091-2f70b824288b/code.power) | [Settings](src/171fcb39-ae27-4c2b-b091-2f70b824288b/settings.json) | SPK: `Super---171fcb39_ae27_4c2b_b091_2f70b824288b---Power`
> remember to replace the `---` with `___` in the SPK to activate that Power in your code

### All used in [Joomla Component Builder](https://www.joomlacomponentbuilder.com) - [Source](https://git.vdm.dev/joomla/Component-Builder) - [Mirror](https://github.com/vdm-io/Joomla-Component-Builder) - [Download](https://git.vdm.dev/joomla/pkg-component-builder/releases)

---
[![Joomla Volunteer Portal](https://img.shields.io/badge/-Joomla-gold?logo=joomla)](https://volunteers.joomla.org/joomlers/1396-llewellyn-van-der-merwe "Join Llewellyn on the Joomla Volunteer Portal: Shaping the Future Together!") [![Octoleo](https://img.shields.io/badge/-Octoleo-black?logo=linux)](https://git.vdm.dev/octoleo "--quiet") [![Llewellyn](https://img.shields.io/badge/-Llewellyn-ffffff?logo=gitea)](https://git.vdm.dev/Llewellyn "Collaborate and Innovate with Llewellyn on Git: Building a Better Code Future!") [![Telegram](https://img.shields.io/badge/-Telegram-blue?logo=telegram)](https://t.me/Joomla_component_builder "Join Llewellyn and the Community on Telegram: Building Joomla Components Together!") [![Mastodon](https://img.shields.io/badge/-Mastodon-9e9eec?logo=mastodon)](https://joomla.social/@llewellyn "Connect and Engage with Llewellyn on Joomla Social: Empowering Communities, One Post at a Time!") [![X (Twitter)](https://img.shields.io/badge/-X-black?logo=x)](https://x.com/llewellynvdm "Join the Conversation with Llewellyn on X: Where Ideas Take Flight!") [![GitHub](https://img.shields.io/badge/-GitHub-181717?logo=github)](https://github.com/Llewellynvdm "Build, Innovate, and Thrive with Llewellyn on GitHub: Turning Ideas into Impact!") [![YouTube](https://img.shields.io/badge/-YouTube-ff0000?logo=youtube)](https://www.youtube.com/@OctoYou "Explore, Learn, and Create with Llewellyn on YouTube: Your Gateway to Inspiration!") [![n8n](https://img.shields.io/badge/-n8n-black?logo=n8n)](https://n8n.io/creators/octoleo "Effortless Automation and Impactful Workflows with Llewellyn on n8n!") [![Docker Hub](https://img.shields.io/badge/-Docker-grey?logo=docker)](https://hub.docker.com/u/llewellyn "Llewellyn on Docker: Containerize Your Creativity!") [![Open Collective](https://img.shields.io/badge/-Donate-green?logo=opencollective)](https://opencollective.com/joomla-component-builder "Donate towards JCB: Help Llewellyn financially so he can continue developing this great tool!") [![GPG Key](https://img.shields.io/badge/-GPG-blue?logo=gnupg)](https://git.vdm.dev/Llewellyn/gpg "Unlock Trust and Security with Llewellyn's GPG Key: Your Gateway to Verified Connections!")