## ✅ Precompiled VIA Firmware (.UF2) for RP2040 Keyboards

This repository contains a collection of **precompiled VIA-compatible `.uf2` firmware files** for popular custom keyboards that use RP2040 microcontrollers, such as the [**Blok RP2040 Controller**](https://boardsource.xyz/products/blok-rp2040-controller-for-the-keyboards) by [Boardsource](https://boardsource.xyz).

If you're setting up or flashing a keyboard like the [Unicorne](https://boardsource.xyz/products/unicorne), [Corne](https://boardsource.xyz/products/corne), [Lily Pad](https://boardsource.xyz/products/lily-pad), [Lily58](https://boardsource.xyz/products/lily58),  or [Sweep](https://boardsource.xyz/products/crab-broom-choc-ferris-sweep), these `.uf2` files will save you time and frustration. Each file is:

- **VIA-Ready** — no need to manually load layouts, ready for easy plug-and-play remapping
- **Precompiled for RP2040**, replacing traditional Pro Micros controllers
- Built Using **QMK firmware**
- Compatible with Blok-based builds and other RP2040 based builds
- Tested during extensive keyboard assembly at Boardsource, these maps simply work!

All files here are intended to work with the **VIA Configuration Tool** ([usevia.app](https://usevia.app)) for easy, drag-and-drop key remapping, no compilation or JSON imports required.

We’ve already done the hard work of configuring and compiling QMK for RP2040-based split keyboards. Just download the correct `.uf2` file, put your board into bootloader mode, and flash it. The process usually takes under a minute.

👉 **Need Help Flashing? Follow This Guide:**
[How to Flash a Keyboard With a .UF2 File](https://boardsource.xyz/blogs/guides/flashing_a_uf2)

---

### Want to Contribute?

If you've compiled a working `.uf2` for an RP2040 keyboard, especially with VIA support, feel free to submit a PR. Just make sure it's tested and named clearly.

---

| Keyboard Name                                                             | File Type     | Download link                                                                                                          |
| ------------------------------------------------------------------------- | ------------- | ---------------------------------------------------------------------------------------------------------------------- |
| [Corne SMT / Unicorne ](https://boardsource.xyz/products/unicorne)        | VIA .UF2      | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/boardsource_corne_smt_via.uf2)             |
| [Corne Kit (DIY)](https://boardsource.xyz/products/corne)                       | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/crkbd_rev1_via_blok.uf2)                   |
| [Lily58 SMT / Lily Pad](https://boardsource.xyz/products/lily-pad)            | VIA .UF2      | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/lily58_SMT_via.uf2)                        |
| [Lily58 Kit (DIY)](https://boardsource.xyz/products/lily58)                     | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/boardsource_lily58_avr_via_blok.uf2)       |
| [Sweep v2 (DIY)](https://boardsource.xyz/products/crab-broom-choc-ferris-sweep) | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/ferris_sweep_via_blok.uf2)                 |
| Microdox v2                                                               | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/boardsource_microdox_v2_via_blok.uf2)      |
| Reviung 41                                                                | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/reviung_reviung41_via_blok.uf2)            |
| Rhymestone                                                                | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/marksard_rhymestone_rev1_default_blok.uf2) |
| Sessanta                                                                  | Blok VIA .UF2 | [Download](https://raw.githubusercontent.com/boardsource/via_files/main/via/boardsource_sessanta_via_blok.uf2)         |


<div itemscope itemtype="https://schema.org/FAQPage">
<h2>Flashing FAQ</h2>

  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question" style="margin-bottom: 1.5em;">
    <h2 itemprop="name">What is VIA and how does it work with split keyboards?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <p itemprop="text">
        <a href="https://usevia.app" target="_blank">VIA</a> is a real-time keyboard configurator that lets you change your layout instantly without reflashing firmware. With precompiled VIA-enabled firmware and RP2040 controllers like our <a href="https://boardsource.xyz/products/blok-rp2040-controller-for-the-keyboards" target="_blank">Blok</a>, VIA supports seamless real-time remapping even on split keyboards like the <a href="https://boardsource.xyz/products/lily58" target="_blank">Lily58</a> and <a href="https://boardsource.xyz/products/corne" target="_blank">Corne</a>.
      </p>
    </div>
  </div>

  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question" style="margin-bottom: 1.5em;">
    <h2 itemprop="name">What is the Blok and why do I need special firmware for it?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <p itemprop="text">
        The <a href="https://boardsource.xyz/products/blok-rp2040-controller-for-the-keyboards" target="_blank">Blok</a> is Boardsource’s custom RP2040-based controller designed to replace Pro Micros. Since most keyboards are designed around ATmega32u4 (Pro Micro), using the Blok (RP2040) requires changes in the QMK build. We’ve done that work for you and compiled `.UF2` files which work out of the box with VIA enabled.
      </p>
    </div>
  </div>

  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question" style="margin-bottom: 1.5em;">
    <h2 itemprop="name">How do I flash a .UF2 VIA firmware file to my keyboard?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <p itemprop="text">
        To flash a `.UF2` file, you’ll first need to enter bootloader mode. On RP2040-based boards (like those using the Blok or setting up an SMT PCB) this is usually done by holding the <strong>BOOT</strong> button while pressing <strong>RESET</strong>. Once in bootloader, a drive named <code>RPI-RP2</code> or similar will appear. Drag your `.UF2` file into the drive that appears in order to flash the firmware. It is the same process as adding a file to a flash drive. For detailed instructions, read our full guide: <a href="https://boardsource.xyz/blogs/guides/flashing_a_uf2" target="_blank">How to Flash a Keyboard with .UF2</a>.
      </p>
    </div>
  </div>

  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question" style="margin-bottom: 1.5em;">
    <h2 itemprop="name">What is a “Blok VIA .UF2” file?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <p itemprop="text">
        A “Blok VIA .UF2” is a precompiled firmware file built with QMK, designed specifically for keyboards using the <a href="https://boardsource.xyz/products/blok-rp2040-controller-for-the-keyboards" target="_blank">Blok RP2040 Controller</a>. It replaces the need for a Pro Micro and includes VIA support, allowing instant key remapping with the VIA app. Just flash it and you're good to go!
      </p>
    </div>
  </div>

  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question" style="margin-bottom: 1.5em;">
    <h2 itemprop="name">Is my keyboard supported by VIA?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <p itemprop="text">
        If you're using a Boardsource keyboard like the <a href="https://boardsource.xyz/products/lily58" target="_blank">Lily58</a>,<a href="https://boardsource.xyz/products/corne" target="_blank">Corne</a>, <a href="https://boardsource.xyz/products/unicorne" target="_blank">Unicorne</a>, <a href="https://boardsource.xyz/products/lily-pad" target="_blank">Lily Pad</a>, or <a href="https://boardsource.xyz/products/crab-broom-choc-ferris-sweep" target="_blank">Sweep</a>, and flash the provided `.uf2` file, it’s VIA-compatible out of the box. We've ensured all of our products have VIA maps available. For other boards, please refer directly to the VIA Documentation related to <a href="https://caniusevia.com/docs/supported_keyboards" target="_blank">support keyboards</a>.
      </p>
    </div>
  </div>

  <div itemscope itemprop="mainEntity" itemtype="https://schema.org/Question">
    <h2 itemprop="name">Can I contribute other VIA .UF2 files to this repo?</h2>
    <div itemscope itemprop="acceptedAnswer" itemtype="https://schema.org/Answer">
      <p itemprop="text">
        Yes! If you've compiled a working VIA-enabled `.UF2` for a keyboard that uses RP2040, feel free to submit a pull request. Just be sure the firmware is tested and named clearly.
      </p>
    </div>
  </div>
</div>
