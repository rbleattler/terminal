---
title: Windows Terminal Rendering Settings
description: Learn how to customize rendering settings within Windows Terminal.
ms.date: 04/14/2021
ms.topic: how-to
---

# Rendering settings in Windows Terminal

The properties listed below affect the entire terminal window, regardless of the profile settings. These should be placed at the root of your [settings.json file](../install.md#settings-json-file).

If you are thinking about changing the rendering settings, additional information is provided on the [Troubleshooting page](./../troubleshooting.md#the-text-is-blurry) to help guide you.

## Redraw entire screen when display updates

When this set to `true`, the terminal will redraw the entire screen each frame. When set to `false`, it will render only the updates to the screen between frames.

**Property name:** `experimental.rendering.forceFullRepaint`

**Necessity:** Optional

**Accepts:** `true`, `false`

**Default value:** `false`

<br />

___

## Use software rendering

When this is set to `true`, the terminal will use the software renderer (a.k.a. WARP) instead of the hardware one.

**Property name:** `experimental.rendering.software`

**Necessity:** Optional

**Accepts:** `true`, `false`

**Default value:** `false`

<br />

___

## Enable unfocused acrylic

When this is set to `true`, the terminal will attempt to use acrylic even when the window is unfocused. This will only work if acrylic is enabled in the OS, and in your profile. When set to `false`, acrylic will only be used when the window is focused (even if `useAcrylic` is set to `true` in a profile's `unfocusedAppearance`).

**Property name:** `compatibility.enableUnfocusedAcrylic`

**Necessity:** Optional

**Accepts:** `true`, `false`

**Default value:** `true`

> [!IMPORTANT]
> This feature is only available in [Windows Terminal Preview](https://aka.ms/terminal-preview).
