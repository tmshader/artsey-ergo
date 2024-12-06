---
layout: home
---

{% assign cacheBust = site.time | date:'?v=%s' %}
![Image]({{ "/images/artsey_ergo-3D_blender_angled.png" | absolute_url | append: cacheBust }})

[![ZMK Build](https://github.com/tmshader/artsey-ergo/actions/workflows/build.yml/badge.svg)](https://github.com/tmshader/artsey-ergo/actions/workflows/build.yml)

[![Pages Build](https://github.com/tmshader/artsey-ergo/actions/workflows/kibot.yml/badge.svg)](https://github.com/tmshader/artsey-ergo/actions/workflows/kibot.yml)

![GitHub last commit](https://img.shields.io/github/last-commit/tmshader/artsey-ergo?link=https%3A%2F%2Fgithub.com%2Ftmshader%2Fartsey-ergo)

## Table of contents

- [Table of contents](#table-of-contents)
  - [Render Angled](#render-angled)
  - [Render Top](#render-top)
  - [Render Bottom](#render-bottom)
  - [Schematic](#schematic)
    - [Monochrome](#monochrome)
    - [Light](#light)
  - [Assembly](#assembly)
    - [Gerber viewer on tracespace.io](#gerber-viewer-on-tracespaceio)
  - [Interactive BOM](#interactive-bom)
  - [BOM](#bom)
  - [Downloads](#downloads)
    - [JLCPCB](#jlcpcb)
    - [Panelized JLCPCB](#panelized-jlcpcb)
    - [3D Step](#3d-step)
- [Report](#report)
  - [ERC](#erc)
  - [DRC](#drc)

### Render Angled

![Image]({{ "/images/artsey_ergo-3D_blender_angled.png" | absolute_url | append: cacheBust }})

### Render Top

![Image]({{ "/images/artsey_ergo-3D_blender_top.png" | absolute_url | append: cacheBust }})

### Render Bottom

![Image]({{ "/images/artsey_ergo-3D_blender_bottom.png" | absolute_url | append: cacheBust }})

### Schematic

#### Monochrome

- [Schematic Monochrome PDF]({{ "/documents/artsey_ergo-schematic-mono.pdf" | absolute_url | append: cacheBust }})

#### Light

- [Schematic Light PDF]({{ "/documents/artsey_ergo-schematic-default.pdf" | absolute_url | append: cacheBust }})

### Assembly

#### Gerber viewer on tracespace.io

[JLCPCB Gerber](https://tracespace.io/view/?boardUrl={{ "export/artsey_ergo-JLCPCB.zip" | absolute_url | append: cacheBust }})

[Panelized JLCPCB Gerber](https://tracespace.io/view/?boardUrl={{ "export/artsey_ergo-panel-JLCPCB.zip" | absolute_url | append: cacheBust }})

### Interactive BOM

Check component locations by hovering over a specific component.
The visual elements might not be precise enough for pcb review but can be very useful since it's possible to pan and zoom.
Not all BOM columns are available here, for datasheet links see BOM below.

[IBOM HTML]({{ "/export/artsey_ergo-ibom.html" | absolute_url | append: cacheBust }})

### BOM

All components with Values, References, Sheetpath and Links to the datasheet.

[BOM HTML]({{ "/export/artsey_ergo-bom.html" | absolute_url | append: cacheBust }})

### Downloads

#### JLCPCB

- [JLCPCB Zip]({{ "export/artsey_ergo-JLCPCB.zip" | absolute_url | append: cacheBust }})
- [JLCPCB BOM CSV]({{ "export/artsey_ergo_bom_jlc.csv" | absolute_url | append: cacheBust }})
- [JLCPCB CPL CSV]({{ "export/artsey_ergo_cpl_jlc.csv" | absolute_url | append: cacheBust }})

#### Panelized JLCPCB

- [Panelized JLCPCB Zip]({{ "export/artsey_ergo-panel-JLCPCB.zip" | absolute_url | append: cacheBust }})
- [Panelized JLCPCB BOM CSV]({{ "export/artsey_ergo-panel_bom_jlc.csv" | absolute_url | append: cacheBust }})
- [Panelized JLCPCB CPL CSV]({{ "export/artsey_ergo-panel_cpl_jlc.csv" | absolute_url | append: cacheBust }})

#### 3D Step

- [3D Step]({{ "/artsey_ergo-3D.step" | absolute_url | append: cacheBust }})

## Report

### ERC

{% include_relative erc_validation.md %}

### DRC

{% include_relative drc_validation.md %}

{ % include _ relative artsey_ergo-report.md % }