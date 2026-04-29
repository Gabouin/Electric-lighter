![License](https://img.shields.io/badge/License-MIT-blue.svg)
![CAD](https://img.shields.io/badge/CAD-Fusion%20360-orange.svg)
![3D Printing](https://img.shields.io/badge/3D%20Printing-PLA-green.svg)
![Schematic](https://img.shields.io/badge/Schematic-KiCad-yellow.svg)


<table>
  <tr>
    <td width="17%">
      <img width=100% alt="image" src="https://github.com/user-attachments/assets/d4c7bb2a-7c48-4c4c-b114-118e6000fbbe" />
    </td>
    <td>
      <h1>Electric-lighter</h1>
      <p>
        A compact electric lighter built from salvaged electronics and a 3D-printed enclosure. Powered by a recycled vape Li-ion battery, it uses a nichrome       heating element to produce an arc-free, windproof flame. Ideal for starting campfires or any situation where a standard lighter falls short.
      </p>
    </td>
  </tr>
</table>


---

## Table of Contents

- [About the Project](#about-the-project)
- [Demo](#demo)
- [Bill of Materials](#bill-of-materials)
- [CAD Files](#cad-files)
- [CAD Preview](#cad-preview)
- [Wiring](#wiring)
- [Finished Build](#finished-build)
- [How to Build](#how-to-build)
- [License](#license)
- [Contributing](#contributing)

---

## About the Project

I found an old vape discarded on the ground and decided to repurpose its battery and charging module into something more useful. The result is a fully functional electric lighter housed in a custom 3D-printed enclosure.

**To use it:**
1. Charge via the USB-C port on the TP4056 module.
2. Press and hold the push button.
3. The nichrome heating element glows red-hot : use it to ignite tinder, paper, or anything else.

---

## Demo

[Watch the demo on YouTube Shorts](https://youtube.com/shorts/gVn74AAT994)

---

## Bill of Materials

| Item | Description | Source | Est. Price (USD) | Purchase Link |
|------|-------------|--------|-----------------|---------------|
| Li-ion Battery | 3.7 V · 1000 mAh — salvaged from found vape | Salvaged | $4.00 | [AliExpress](https://www.aliexpress.com/w/wholesale-18650-li-ion-battery.html) |
| TP4056 USB-C Module | USB-C charging/protection module | Salvaged / AliExpress | $0.50 | [AliExpress](https://www.aliexpress.com/w/wholesale-tp4056-usb-c.html) |
| Heating Element | Nichrome wire salvaged from old toaster | Salvaged | $0.50 | [AliExpress](https://www.aliexpress.com/w/wholesale-nichrome-heating-wire.html) |
| Push Button | 12 × 12 mm tactile push button | Salvaged | $0.10 | [AliExpress](https://www.aliexpress.com/w/wholesale-6x6mm-tactile-push-button.html) |
| Silicone Wire AWG 22 | Heat-resistant wire — ~30 cm red + black | Salvaged | $0.30 | [AliExpress](https://www.aliexpress.com/w/wholesale-silicone-wire-awg22.html) |
| Alligator Clips | For prototyping connections | Salvaged | $0.20 | [AliExpress](https://www.aliexpress.com/w/wholesale-alligator-clips.html) |
| PLA Filament | ~40 g for the enclosure (top + bottom) | Own stock | $0.80 | [AliExpress](https://www.aliexpress.com/w/wholesale-pla-filament-1kg.html) |
| M3 Screws + Inserts | M3 brass heat-set inserts × 4 + matching screws | Salvaged / Own stock | $0.50 | [AliExpress](https://www.aliexpress.com/w/wholesale-m3-heat-set-insert-brass.html) |

> **Total estimated cost: ~$6.91** (when salvaging the electronic components)

---

## CAD Files

All CAD files are available in multiple formats for maximum compatibility.

| Component | Fusion 360 | STEP | STL | 3MF (top) | 3MF (bottom) |
|-----------|-----------|------|-----|-----------|--------------|
| Full enclosure | `CAD/ELECTRIC LIGHTER.f3z` | `CAD/ELECTRIC LIGHTER.step` | `CAD/ELECTRIC LIGHTER.stl` | `3D printing/EL top part.3mf` | `3D printing/EL bottom part.3mf` |

> CAD software used: **Autodesk Fusion 360**
>
> Schematic files (KiCad): `KiCad schem/ELECTRIC LIGHTER.kicad_sch`, `KiCad schem/ELECTRIC LIGHTER.net`

---

## CAD Preview

<img width="780" alt="CAD enclosure" src="https://github.com/user-attachments/assets/5113c64e-cd9b-433e-ae8d-2bb7b434807a" />

---

## Wiring

The circuit is straightforward: the TP4056 module charges the Li-ion battery and provides over-charge/over-discharge protection. A push button connects the battery output directly to the nichrome heating element.

<table>
  <tr>
    <td align="center"><b>Wiring Diagram — Overview</b></td>
    <td align="center"><b>Wiring Diagram — Detail</b></td>
  </tr>
  <tr>
    <td><img width="400" alt="Wiring diagram overview" src="https://github.com/user-attachments/assets/9ce767e1-1db6-403d-bbf6-bb0a3bd62f55" /></td>
    <td><img width="200" alt="Wiring diagram detail" src="https://github.com/user-attachments/assets/3d47b3ca-f959-4605-90af-c45848d23aa8" /></td>
  </tr>
</table>

The built circuit before enclosing:

![Built circuit](https://github.com/user-attachments/assets/6ffc6ee7-df6f-4532-81b7-1d6471d2e09a)

---

## Finished Build

![Finished lighter](https://github.com/user-attachments/assets/2d547b7d-7cd5-4a53-b94d-dae346e632f1)

---

## How to Build

1. **Print the enclosure** — Print `EL top part.3mf` and `EL bottom part.3mf` using PLA. Install the four M3 brass heat-set inserts into the bottom shell with a soldering iron.
2. **Prepare the heating element** — Cut a short length of nichrome wire and attach it to two silicone wires using alligator clips or by soldering.
3. **Wire the electronics** — Follow the KiCad schematic: battery → TP4056 module (for charging) → push button → nichrome heating element. Use heat-resistant silicone wire throughout.
4. **Fit everything into the enclosure** — Place the battery, TP4056 module, push button, and heating element assembly inside the bottom shell.
5. **Close the enclosure** — Align the top shell and secure it with four M3 screws into the heat-set inserts.
6. **Charge and test** — Plug in a USB-C cable to charge the battery. Once charged, press and hold the button — the element should glow red within a second.

> ⚠️ **Safety note:** The nichrome element reaches very high temperatures instantly. Keep fingers clear of the element when the button is pressed, and never leave it unattended while active.

---

## License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## Contributing

Contributions, improvements, and remixes are welcome! Please read the [CONTRIBUTING.md](CONTRIBUTING.md) guide to get started.
