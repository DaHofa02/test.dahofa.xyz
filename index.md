---
layout: default
---

Text can be **bold**, _italic_, or ~~strikethrough~~.

[Link to another page](./another-page.html).

There should be whitespace between paragraphs.

There should be whitespace between paragraphs. We recommend including a README, or a file with information about your project.

# DaHofa

This is DAHOFA

## Programming

```js
// Javascript code with syntax highlighting.
var fun = function lang(l) {
  dateformat.i18n = require('./lang/' + l)
  return true;
}
```

```java
package xyz.dahofa.rotarycraft;

import net.neoforged.bus.api.IEventBus;
import net.neoforged.fml.ModContainer;
import net.neoforged.fml.common.Mod;
import net.neoforged.neoforge.common.NeoForge;
import xyz.dahofa.rotarycraft.api.lib.Names;
import xyz.dahofa.rotarycraft.common.registry.RCArmorMaterials;
import xyz.dahofa.rotarycraft.common.registry.RCBlocks;
import xyz.dahofa.rotarycraft.common.registry.RCCreativeModeTab;
import xyz.dahofa.rotarycraft.common.registry.RCItems;

// The value here should match an entry in the META-INF/neoforge.mods.toml file
@Mod(Names.MOD_ID)
public class RotaryCraftRerotated {
    // The constructor for the mod class is the first code that is run when your mod is loaded.
    // FML will recognize some parameter types like IEventBus or ModContainer and pass them in automatically.
    public RotaryCraftRerotated(ModContainer container, IEventBus modBus) {
        IEventBus forgeBus = NeoForge.EVENT_BUS;
        registerAllDeferredRegistryObjects(modBus);
    }

    private void registerAllDeferredRegistryObjects(IEventBus modBus) {
        RCItems.BLOCKS.register(modBus);
        RCItems.ITEMS.register(modBus);
        RCItems.TOOLS.register(modBus);
        RCItems.ORES.register(modBus);
        RCItems.ENCHANTED_TOOLS.register(modBus);

        RCBlocks.BLOCKS.register(modBus);

        RCArmorMaterials.ARMOR_MATERIALS.register(modBus);

        RCCreativeModeTab.TABS.register(modBus);
    }

}

```

#### Header 4

*   This is an unordered list following a header.
*   This is an unordered list following a header.
*   This is an unordered list following a header.

##### Header 5

1.  This is an ordered list following a header.
2.  This is an ordered list following a header.
3.  This is an ordered list following a header.

###### Header 6

| head1        | head two          | three |
|:-------------|:------------------|:------|
| ok           | good swedish fish | nice  |
| out of stock | good and plenty   | nice  |
| ok           | good `oreos`      | hmm   |
| ok           | good `zoute` drop | yumm  |

### There's a horizontal rule below this.

* * *

### Here is an unordered list:

*   Item foo
*   Item bar
*   Item baz
*   Item zip

### And an ordered list:

1.  Item one
1.  Item two
1.  Item three
1.  Item four

### And a nested list:

- level 1 item
  - level 2 item
  - level 2 item
    - level 3 item
    - level 3 item
- level 1 item
  - level 2 item
  - level 2 item
  - level 2 item
- level 1 item
  - level 2 item
  - level 2 item
- level 1 item

### Small image

![Octocat](https://github.githubassets.com/images/icons/emoji/octocat.png)

### Large image

![Branching](https://guides.github.com/activities/hello-world/branching.png)


### Definition lists can be used with HTML syntax.

<dl>
<dt>Name</dt>
<dd>Godzilla</dd>
<dt>Born</dt>
<dd>1952</dd>
<dt>Birthplace</dt>
<dd>Japan</dd>
<dt>Color</dt>
<dd>Green</dd>
</dl>

```
Long, single-line code blocks should not wrap. They should horizontally scroll if they are too long. This line should be long enough to demonstrate this.
```

```
The final element.
```
