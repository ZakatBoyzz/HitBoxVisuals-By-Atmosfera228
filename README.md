# Hitbox Visuals — Minecraft 1.21.4 (Fabric)

A client-side Fabric mod source project for Minecraft Java 1.21.4 / Java 21.

## Controls
- **H by default** — toggle hitboxes.
- **K by default** — open the mod settings.
- Both actions are registered as normal Minecraft keybindings. Change them in **Options → Controls → Key Binds**, under the **Hitbox Visuals** category.
- The settings screen displays the current bindings, including any keys you assign yourself.

## Visibility rules
- Players without invisibility: show a hitbox only when a raycast can see part of the player; fully occluded players are skipped.
- Invisible players with at least one equipped armor piece: same visibility rule; no through-wall rendering.
- Invisible players with no equipped armor: never show a hitbox.
- There is no through-walls mode.

## Features currently included
- Configurable outline/fill and hover colors using a palette.
- Fill toggle and transparency cycle.
- Hover color change.
- Settings persist in `.minecraft/config/hitboxvisuals.json`.

## Build
Requires JDK 21, Gradle 8.x, and internet access to resolve Fabric/Minecraft dependencies.

From this folder run:

```bat
gradle build
```

The resulting mod JAR should appear in `build/libs/`.

**Build status note:** this environment did not have Gradle installed and could not access the internet to download it, so the project has not been compiled or tested here. Do not treat this ZIP as a finished JAR.
