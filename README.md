## 🔑 Permissions

### 🛡️ Admin
| Permission | Description |
|---|---|
| `lotuschat.admin` | Full access to all LotusChat features |
| `lotuschat.command` | Access to the `/lc` command |
| `lotuschat.reload` | Reload the plugin via `/lc reload` |

### 💬 Chat
| Permission | Description |
|---|---|
| `lotuschat.chat.colors` | Use color codes (`&0`–`&f`) in chat messages |
| `lotuschat.chat.formats` | Use format codes (`&k`–`&r`) in chat messages |

### 🎨 ChatColor
| Permission | Description |
|---|---|
| `lotuschat.chatcolor` | Open the `/chatcolor` GUI menu |
| `lotuschat.chatcolor.set` | Use `/chatcolor set` to change another player's color |
| `lotuschat.chatcolor.*` | Access to all colors, formats, hex and custom colors |
| `lotuschat.chatcolor.and0` | Select Black (`&0`) as chat color |
| `lotuschat.chatcolor.and1` | Select Dark Blue (`&1`) as chat color |
| `lotuschat.chatcolor.and2` | Select Dark Green (`&2`) as chat color |
| `lotuschat.chatcolor.and3` | Select Dark Aqua (`&3`) as chat color |
| `lotuschat.chatcolor.and4` | Select Dark Red (`&4`) as chat color |
| `lotuschat.chatcolor.and5` | Select Dark Purple (`&5`) as chat color |
| `lotuschat.chatcolor.and6` | Select Gold (`&6`) as chat color |
| `lotuschat.chatcolor.and7` | Select Gray (`&7`) as chat color |
| `lotuschat.chatcolor.and8` | Select Dark Gray (`&8`) as chat color |
| `lotuschat.chatcolor.and9` | Select Blue (`&9`) as chat color |
| `lotuschat.chatcolor.anda` | Select Green (`&a`) as chat color |
| `lotuschat.chatcolor.andb` | Select Aqua (`&b`) as chat color |
| `lotuschat.chatcolor.andc` | Select Red (`&c`) as chat color |
| `lotuschat.chatcolor.andd` | Select Light Purple (`&d`) as chat color |
| `lotuschat.chatcolor.ande` | Select Yellow (`&e`) as chat color |
| `lotuschat.chatcolor.andf` | Select White (`&f`) as chat color |
| `lotuschat.chatcolor.formats` | Select text formats (bold, italic, etc.) in the GUI |

### 🌈 Hex & Custom Colors
| Permission | Description |
|---|---|
| `lotuschat.chatcolor.hex` | Open the Hex Colors submenu |
| `lotuschat.chatcolor.hex.*` | Access **all** preset hex colors defined in `chatcolor.yml` |
| `lotuschat.chatcolor.hex.custom` | Enter a custom solid hex color via chat input |
| `lotuschat.chatcolor.hex.custom-gradient` | Enter a custom hex gradient via chat input |
| `lotuschat.chatcolor.custom` | Open the Custom Colors submenu |
| `lotuschat.chatcolor.custom.*` | Access **all** custom color patterns defined in `chatcolor.yml` |

To grant access to a **specific** hex color or custom pattern, use the key defined in `chatcolor.yml`:

**Hex colors** — key is the entry name under `hex-color-menu.colors`:
| Permission | Description |
|---|---|
| `lotuschat.chatcolor.hex.sky_blue` | Access to the Sky Blue hex color |
| `lotuschat.chatcolor.hex.deep_purple` | Access to the Deep Purple hex color |
| `lotuschat.chatcolor.hex.coral` | Access to the Coral hex color |
| `lotuschat.chatcolor.hex.mint` | Access to the Mint hex color |
| `lotuschat.chatcolor.hex.gold_hex` | Access to the Gold hex color |
| `lotuschat.chatcolor.hex.ocean_gradient` | Access to the Ocean gradient |
| `lotuschat.chatcolor.hex.sunset_gradient` | Access to the Sunset gradient |
| `lotuschat.chatcolor.hex.forest_gradient` | Access to the Forest gradient |
| `lotuschat.chatcolor.hex.candy_gradient` | Access to the Candy gradient |

**Custom colors** — key is the entry name under `custom-color-menu.colors`:
| Permission | Description |
|---|---|
| `lotuschat.chatcolor.custom.rainbow` | Access to the Rainbow pattern |
| `lotuschat.chatcolor.custom.gradient_red_yellow` | Access to the Red-Yellow gradient pattern |
| `lotuschat.chatcolor.custom.gradient_blue_aqua` | Access to the Blue-Aqua gradient pattern |
| `lotuschat.chatcolor.custom.gradient_green` | Access to the Green gradient pattern |
| `lotuschat.chatcolor.custom.pink_purple` | Access to the Pink-Purple pattern |

> If you add new colors in `chatcolor.yml`, their permission node will automatically follow the same pattern: `lotuschat.chatcolor.hex.<key>` or `lotuschat.chatcolor.custom.<key>`.

### 💌 Messaging
| Permission | Description |
|---|---|
| `lotuschat.msg` | Use `/msg`, `/r`, `/msgignore` and `/msgtoggle` |
| `lotuschat.msg.bypass` | Send messages to players who have DMs disabled |
| `lotuschat.spy` | See all private messages between players (social spy) |

### 📦 Chat Display
| Permission | Description |
|---|---|
| `lotuschat.display.cooldown.bypass` | Bypass the cooldown for all display triggers |

> All individual display permissions (e.g. `lotuschat.display.item`, `lotuschat.display.inventory`, `lotuschat.display.stats`, etc.) are defined directly in `chatdisplay.yml` per display entry and **registered automatically at runtime**. Adding a new custom display requires no changes to `plugin.yml`.

### 📢 Chat Channel
| Permission | Description |
|---|---|
| `lotuschat.chatchannel.<id>` | Access to the channel with the matching id (defined in `chatchannel.yml`) |

### 🔒 Chat Filter & Formats
| Permission | Description |
|---|---|
| `lotuschat.filter.bypass` | Bypass the URL and word filter entirely |
| `lotuschat.format.<id>` | Apply the chat format with the matching id (defined in `chatformat.yml`) |

### 🔧 Internal
| Permission | Description |
|---|---|
| `lotuschat.internal` | Internal permission used for inventory, ender chest and item snapshot commands |
