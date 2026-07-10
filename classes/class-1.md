---
layout: class
title: Haas Certification
permalink: /classes/class-1/
sitemap: false
---

## Overview

Placeholder overview for Class One. Replace this with a short description of what the class is about and why it matters.

## What's Covered

- Placeholder topic 1
- Placeholder topic 2
- Placeholder topic 3

## Curriculum Files

### Mill Test Drawing

<div class="file-embed">
  <div class="file-embed-label">Mill Test.pdf</div>
  <iframe src="{{ '/classes/class-1-haas-certification/curriculum/Haas Cert/Mill Inch Package (Haas Certification)/Mill Test.pdf' | relative_url }}"></iframe>
</div>

### O2001 Program

<details markdown="1">
<summary>View O2001 program.NC</summary>

```
%
O2001(TEST)

(MATERIAL - ALUMINUM INCH)
(T1|2"  FACE MILL|H1|D1|TOOL DIA. - 2.)
(T2|1/2 FLAT ENDMILL|H2|D2|TOOL DIA. - .5)
(T3|NO. 7 DRILL|H3|D3|TOOL DIA. - .201)
(T4|3/8 CHAMFER MILL|H4|D4|TOOL DIA. - .375)
(T5|1/4-20 TAPRH|H5|D5|TOOL DIA. - .25)

G20
G0 G17 G40 G49 G80 G90
(FACING OPERATION)
T1 M6
G187 P2 E.025
G0 G90 G54 X-2.7 Y1.4999 S8100 M3
G43 H1 Z.25
M8
Z.2
G1 Z0. F100.
X1.6 F81.
Y.5
X-1.6
Y-.5
X1.6
Y-1.4999
X-2.6
G0 Z.25
M5
G91 G28 Z0. M9
M01
(RELIEF PROFILE)
T2 M6
G187 P2 E.025
G0 G90 G54 X.075 Y-1.875 S8100 M3
G43 H2 Z.5
M8
Z.2
G1 Z-.3 F100.
Y-1.5 F129.6
Y-1.075
X-.075
Y-1.5
Y-1.875
X.075
Z-.6 F100.
Y-1.5 F129.6
Y-1.075
X-.075
Y-1.5
Y-1.875
G0 Z.5
(OUTSIDE PROFILE)
G187 P2 E.025
X-1.7935 Y.6585
Z.2
G1 Z-.3 F100.
X-1.6685 Y.875 F129.6
G3 X-1.635 Y1. I-.2165 J.125
G2 X-1.25 Y1.385 I.385 J0.
G1 X1.25
G2 X1.635 Y1. I0. J-.385
G1 Y-1.
G2 X1.25 Y-1.385 I-.385 J0.
G1 X.635
G2 X.4512 Y-1.3088 I0. J.26
G1 X.4012 Y-1.2588
G2 X.325 Y-1.075 I.1838 J.1838
G1 Y-.865
G3 X.285 Y-.825 I-.04 J0.
G1 X-.285
G3 X-.325 Y-.865 I0. J-.04
G1 Y-1.075
G2 X-.4012 Y-1.2588 I-.26 J0.
G1 X-.4512 Y-1.3088
G2 X-.635 Y-1.385 I-.1838 J.1838
G1 X-1.25
G2 X-1.635 Y-1. I0. J.385
G1 Y1.
G3 X-1.6685 Y1.125 I-.25 J0.
G1 X-1.7935 Y1.3415
Y.6585
Z-.6 F100.
X-1.6685 Y.875 F129.6
G3 X-1.635 Y1. I-.2165 J.125
G2 X-1.25 Y1.385 I.385 J0.
G1 X1.25
G2 X1.635 Y1. I0. J-.385
G1 Y-1.
G2 X1.25 Y-1.385 I-.385 J0.
G1 X.635
G2 X.4512 Y-1.3088 I0. J.26
G1 X.4012 Y-1.2588
G2 X.325 Y-1.075 I.1838 J.1838
G1 Y-.865
G3 X.285 Y-.825 I-.04 J0.
G1 X-.285
G3 X-.325 Y-.865 I0. J-.04
G1 Y-1.075
G2 X-.4012 Y-1.2588 I-.26 J0.
G1 X-.4512 Y-1.3088
G2 X-.635 Y-1.385 I-.1768 J.1768
G1 X-1.25
G2 X-1.635 Y-1. I0. J.385
G1 Y1.
G3 X-1.6685 Y1.125 I-.25 J0.
G1 X-1.7935 Y1.3415
X-1.7835 Y.6585 F80.
X-1.6585 Y.875
G3 X-1.625 Y1. I-.2165 J.125
G2 X-1.25 Y1.375 I.375 J0.
G1 X1.25
G2 X1.625 Y1. I0. J-.375
G1 Y-1.
G2 X1.25 Y-1.375 I-.375 J0.
G1 X.635
G2 X.4582 Y-1.3018 I0. J.25
G1 X.4082 Y-1.2518
G2 X.335 Y-1.075 I.1768 J.1768
G1 Y-.865
G3 X.285 Y-.815 I-.05 J0.
G1 X-.285
G3 X-.335 Y-.865 I0. J-.05
G1 Y-1.075
G2 X-.4082 Y-1.2518 I-.25 J0.
G1 X-.4582 Y-1.3018
G2 X-.635 Y-1.375 I-.1768 J.1768
G1 X-1.25
G2 X-1.625 Y-1. I0. J.375
G1 Y1.
G3 X-1.6585 Y1.125 I-.25 J0.
G1 X-1.7835 Y1.3415
G0 Z.5
(CENTER POCKET)
G187 P2 E.025
X-.3802 Y-.0011 Z.25
Z.05
G1 X-.0393 Y-.0005 Z.0381 F113.4
X-.7893 Y-.0018 Z.0119
X-.0393 Y-.0005 Z-.0143
X-.7893 Y-.0018 Z-.0405
X-.0393 Y-.0005 Z-.0667
X-.7893 Y-.0018 Z-.0929
X-.0393 Y-.0005 Z-.119
X-.7893 Y-.0018 Z-.1452
X-.0393 Y-.0005 Z-.1714
X-.7893 Y-.0018 Z-.1976
X-.0393 Y-.0005 Z-.2238
X-.7893 Y-.0018 Z-.25
X-.7907 Y-.0524
X.7907
G3 X.84 Y0. I-.0032 J.0524
X.7907 Y.0524 I-.0525 J0.
G1 X-.7907
X.7875 Y-.0625
F80.
G3 X.85 Y0. I0. J.0625 F113.4
X.7875 Y.0625 I-.0625 J0.
G1 X-.7875
G3 X-.85 Y0. I0. J-.0625
X-.7875 Y-.0625 I.0625 J0.
G1 X.7875
G0 Z.25
M5
G91 G28 Z0. M9
M01
(DRILL HOLE FOR TAP)
T3 M6
G187 P2 E.025
G0 G90 G54 X-.98 Y.85 S8100 M3
G43 H3 Z.2
M8
G99 G83 Z-1. R.2 Q.15 F48.6
X.98
Y-.85
X-.98
G80
M5
G91 G28 Z0. M9
M01
(1/4-20 TAP)
T5 M6
G187 P2 E.025
G0 G90 G54 X-.98 Y.85 S1200 M3
G43 H5 Z.1
M8
G99 G84 Z-.625 R.1 F60.
X.98
Y-.85
X-.98
G80
M5
G91 G28 Z0. M9
M01
(DEBUR)
T4 M6
G187 P2 E.025
G0 G90 G54 X-1.4489 Y1.325 S8100 M3
G43 H4 Z.5
M8
Z.2
G1 Z-.04 F100.
X-1.3163 Y1.1925 F113.4
G3 X-1.25 Y1.165 I.0663 J.0663
G1 X1.25
G2 X1.415 Y1. I0. J-.165
G1 Y-1.
G2 X1.25 Y-1.165 I-.165 J0.
G1 X.635
G2 X.6067 Y-1.1533 I0. J.04
G1 X.5567 Y-1.1033
G2 X.545 Y-1.075 I.0283 J.0283
G1 Y-.865
G3 X.285 Y-.605 I-.26 J0.
G1 X-.285
G3 X-.545 Y-.865 I0. J-.26
G1 Y-1.075
G2 X-.5567 Y-1.1033 I-.04 J0.
G1 X-.6067 Y-1.1533
G2 X-.635 Y-1.165 I-.0283 J.0283
G1 X-1.25
G2 X-1.415 Y-1. I0. J.165
G1 Y1.
G2 X-1.25 Y1.165 I.165 J0.
G3 X-1.1837 Y1.1925 I0. J.0938
G1 X-1.0511 Y1.325
G0 Z.5
X.5886 Y-.1125
Z.2
G1 Z-.04 F100.
X.7212 Y-.245 F113.4
G3 X.7875 Y-.2725 I.0663 J.0663
X1.06 Y0. I0. J.2725
X.7875 Y.2725 I-.2725 J0.
G1 X-.7875
G3 X-1.06 Y0. I0. J-.2725
X-.7875 Y-.2725 I.2725 J0.
G1 X.7875
G3 X.8538 Y-.245 I0. J.0938
G1 X.9864 Y-.1125
G0 Z.5
(DEBUR)
G187 P2 E.025
X-.98 Y-.8588
Z.2
G1 Z-.04 F100.
Y-.765 F113.4
G3 X-1.065 Y-.85 I0. J-.085
X-.98 Y-.935 I.085 J0.
X-.895 Y-.85 I0. J.085
X-.98 Y-.765 I-.085 J0.
G1 Y-.8588
G0 Z.5
X.98
Z.2
G1 Z-.04 F100.
Y-.765 F113.4
G3 X.895 Y-.85 I0. J-.085
X.98 Y-.935 I.085 J0.
X1.065 Y-.85 I0. J.085
X.98 Y-.765 I-.085 J0.
G1 Y-.8588
G0 Z.5
Y.8413
Z.2
G1 Z-.04 F100.
Y.935 F113.4
G3 X.895 Y.85 I0. J-.085
X.98 Y.765 I.085 J0.
X1.065 Y.85 I0. J.085
X.98 Y.935 I-.085 J0.
G1 Y.8413
G0 Z.5
X-.98
Z.2
G1 Z-.04 F100.
Y.935 F113.4
G3 X-1.065 Y.85 I0. J-.085
X-.98 Y.765 I.085 J0.
X-.895 Y.85 I0. J.085
X-.98 Y.935 I-.085 J0.
G1 Y.8413
G0 Z.5
M5
G91 G28 Z0. M9
G28 Y0.
M30
%
```

</details>

### Summer Camp Reference

<div class="file-embed">
  <div class="file-embed-label">CNC Mill Level 1.pdf</div>
  <iframe src="{{ '/classes/class-1-haas-certification/curriculum/Haas Summer Camp/CNC Mill Level 1.pdf' | relative_url }}"></iframe>
</div>

### Downloads

<ul class="file-links">
  <li>
    <a href="{{ '/classes/class-1-haas-certification/curriculum/Haas Cert/Haas Certification Basic Operator Test Template _ 71019.xlsx' | relative_url }}">Haas Certification Basic Operator Test Template</a>
    <span class="file-type">.xlsx</span>
  </li>
  <li>
    <a href="{{ '/classes/class-1-haas-certification/curriculum/Haas Cert/Mill Inch Package (Haas Certification)/Haas Cert Operator Mill (Inch) Set-up sheet.doc' | relative_url }}">Mill (Inch) Set-up Sheet</a>
    <span class="file-type">.doc</span>
  </li>
  <li>
    <a href="{{ '/classes/class-1-haas-certification/curriculum/Haas Cert/Mill Inch Package (Haas Certification)/Mill Test.SLDDRW' | relative_url }}">Mill Test Drawing (SolidWorks)</a>
    <span class="file-type">.SLDDRW</span>
  </li>
</ul>

## Logistics

- **Format:** Placeholder (e.g. in-person, online, hybrid)
- **Duration:** Placeholder (e.g. 8 weeks, 1 semester)
- **Prerequisites:** Placeholder (e.g. none, or list requirements)

## Who It's For

Placeholder description of the ideal student for Class One.

<div class="cta-block">
  <h3>Interested in Haas Certification?</h3>
  <p>Placeholder call-to-action text — add enrollment info, contact details, or a signup link here.</p>
  <a class="cta-button" href="#">Get Started</a>
</div>
