# 🤝 Contributing to Electric Lighter

Thank you for your interest in contributing to this project! Whether you want to improve the enclosure design, suggest electronics improvements, fix documentation, or share your own build — all contributions are welcome.

---

## Table of Contents

- [What Contributions Are Welcome](#what-contributions-are-welcome)
- [What Still Needs to Be Done](#what-still-needs-to-be-done)
- [How to Contribute](#how-to-contribute)
- [Submitting a Pull Request](#submitting-a-pull-request)
- [Reporting Issues](#reporting-issues)
- [Code of Conduct](#code-of-conduct)

---

## What Contributions Are Welcome

This is a hardware / maker project, so contributions can take many forms:

### Design & CAD
- Improvements or optimisations to the 3D-printed enclosure (top/bottom shells).
- Alternative enclosure designs (e.g., different button placement, rounded edges, belt-clip variant).
- New accessories or add-ons (e.g., safety cap, lanyard ring, carrying case).

### Electronics
- Alternative wiring diagrams or circuit improvements.
- Adding a low-battery LED indicator.
- Implementing a timer or auto-shutoff circuit to prevent overheating.
- Replacing the nichrome element with an alternative heating approach (e.g., ceramic element).
- PWM control to regulate element temperature.

### Documentation
- Fixing typos, grammar, or unclear instructions in the README or other docs.
- Adding step-by-step assembly photos or an illustrated build guide.
- Translating documentation into another language.
- Improving the KiCad schematic readability or adding component annotations.

### Bug Reports & Issues
- Reporting fitment problems with the 3D-printed enclosure.
- Pointing out errors in the wiring diagram or BOM (wrong values, incorrect links).
- Suggesting improvements to the build instructions.

---

## What Still Needs to Be Done

Here are open improvements that would greatly benefit the project. Feel free to pick one up:

- [ ] **Safety cap / cover** — Design a printed cap that covers the heating element when not in use.
- [ ] **Low-battery indicator** — Add a simple LED circuit that signals when the battery is nearly depleted.
- [ ] **Auto-shutoff** — Implement a timer (e.g., 555 circuit or small MCU) that cuts power to the element after a set time.
- [ ] **Improved wire management** — Redesign the enclosure interior to better route and retain wires.
- [X] **Charging indicator** — Surface the TP4056 status LEDs through the enclosure so charge state is visible without opening the case. --> printing in transparent filament solve that problem.

---

## 🚀 How to Contribute

### 1. Fork the repository

Click the **Fork** button at the top-right of the repository page to create your own copy.

### 2. Clone your fork

```bash
git clone https://github.com/<your-username>/Electric-lighter.git
cd Electric-lighter
```

### 3. Create a new branch

Use a descriptive branch name that summarises your change:

```bash
git checkout -b feat/safety-cap-design
# or
git checkout -b fix/bom-component-links
# or
git checkout -b docs/assembly-photos
```

### 4. Make your changes

- For **CAD changes**: Export the modified file in both `.f3z` / `.f3d` (Fusion 360) and `.step` formats and place them in the `CAD/` folder. Export print-ready files as `.3mf` into `3D printing/`.
- For **schematic changes**: Update the KiCad files in `KiCad schem/` and export an updated schematic image for the README.
- For **documentation changes**: Edit the relevant `.md` file directly.

### 5. Commit your changes

Write a clear, concise commit message:

```bash
git add .
git commit -m "feat: add safety cap enclosure for heating element"
```

### 6. Push and open a Pull Request

```bash
git push origin feat/safety-cap-design
```

Then open a Pull Request on GitHub against the `main` branch and describe:
- **What** you changed.
- **Why** you changed it.
- Any **known limitations** or things still to do.

---

## Submitting a Pull Request

To keep things consistent and easy to review, please follow these guidelines:

- Keep pull requests focused on a single topic. Separate unrelated changes into separate PRs.
- Include before/after photos or renders when modifying CAD files.
- Update `README.md` if your change affects the BOM, assembly steps, or wiring.
- Make sure file names follow the existing naming convention (uppercase project name prefix, e.g. `ELECTRIC LIGHTER — safety cap.step`).

---

## Reporting Issues

If you find a problem, please [open an issue](../../issues/new) and include:

- A clear description of the problem.
- Steps to reproduce it (e.g., "When printing the top shell at 0.2 mm layer height, the button hole is too tight").
- Photos, screenshots, or measurements if relevant.
- Your printer / slicer settings if the issue is print-related.

---

## Sharing Your Build

Have you built this project? I'd love to see it!

- Open an issue with the label **"Show and Tell"** and share your photos.
- Describe any modifications you made — your changes might inspire future improvements.

---

## Code of Conduct

This project follows a simple rule: **be respectful and constructive**. Everyone is welcome regardless of experience level. If you are new to maker projects, hardware, or GitHub — don't hesitate to ask questions in the issues.

---

Thank you for helping make this project better!
