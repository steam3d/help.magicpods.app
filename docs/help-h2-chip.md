# Functions behavior with H2 chip

Unlike the H1 chip, the H2 chip introduces changes to how the headphones operate:

* The headphones can detect whether they are connected to an Apple or non-Apple device.
* Only one earbud (usually the first one removed from the case) is considered `active` and reports information such as in-ear detection or battery level.

These changes affect the behavior of certain features:

| Feature                  | Behavior Details                                            |
| ------------------------ | ----------------------------------------------------------- |
| Ear detection            | Works only when the `active` earbud is removed from the ear |
| Auto switch sound output | Works with a slight delay                                   |

!!! Tip
    To access advanced features — such as noise control, accurate battery level, enhanced ear detection, conversation awareness, and more — install [MagicAAP](https://magicpods.app/magicaap/) driver.