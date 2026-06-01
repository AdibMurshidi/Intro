---
title-slide: false
bibliography: references.bib
csl: vancouver.csl
citeproc: true
theme: serif
background-color: "#ffffff"
transition: slide
navigationMode: linear
hash: true
---

:::: {.columns}
::: {.column width="50%"}

## Sample slides
#### PlaceHolderName
#### Universiti Malaysia Perlis
#### [placeholder@email.com](mailto:placeholder@email.com)

<audio id="bg-music" src="media/audio/sb.m4a" loop></audio>

<div id="audio-credit"
     style="position: absolute; bottom: 40px; right: 20px; font-size: 0.6em; opacity: 0.6;">
  Music: “Adrift” by Scott Buckley (CC BY 4.0)
</div>

<script>
  document.addEventListener('DOMContentLoaded', () => {
    const audio = document.getElementById('bg-music');
    const credit = document.getElementById('audio-credit');

    // hide credit by default
    credit.style.display = 'none';

    const test = new Audio('media/audio/bgm.mp3');

    test.addEventListener('canplaythrough', () => {
      // bgm.mp3 exists → use it, keep credit hidden
      audio.src = 'media/audio/bgm.mp3';
    }, { once: true });

    test.addEventListener('error', () => {
      // bgm.mp3 missing → sb.m4a will play → show credit
      credit.style.display = 'block';
    }, { once: true });

    document.addEventListener('click', () => {
      if (Reveal.getIndices().h === 0) {
        audio.volume = 0.5;
        audio.play();
      }
    }, { once: true });

    Reveal.on('slidechanged', (event) => {
      if (event.indexh > 0) { audio.pause(); }
      else { audio.play(); }
    });
  });
</script>

:::

::: {.column width="50%"}
![](media/pics/logo1.png)
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide one
**Key Concepts:**
- Energy conservation per @carnot1824.
- $\Delta U = Q - W$
:::

::: {.column width="50%"}
![](media/pics/sample.png)
:::
::::

---

<span class="slide-title" data-title="My Hidden Slide Name"></span>

![](media/pics/wide.jpeg)

---

:::: {.columns}
::: {.column width="50%"}
### The Master Equation
The fundamental relation of thermodynamics:

$$\Delta U = Q - W$$

The work done $W$ is positive when the system expands against an external pressure.
:::

::: {.column width="50%"}
<video data-src="media/videos/sample.mp4" data-autoplay loop muted width="100%"></video>
:::

::::

---

:::: {.columns}
::: {.column width="50%"}
### Visualizing the Gas Law
**Interactive Model:**

- P, V, and T relationships.
- Use the slider to adjust pressure.
- Observe the phase boundary.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/sample.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

---

# Bibliography
<div id="refs"></div>

---

:::: {.columns}
::: {.column width="50%"}
### Distribution of Age

This histogram visualizes the distribution of ages within the `bigclass` dataset.
:::

::: {.column width="50%"}
<iframe 
  data-src="media/plots/age_histogram.html" 
  width="100%" 
  height="500px" 
  style="border:none;" 
  scrolling="no">
</iframe>
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 1: Control Chart for Machine 1
This control chart visualizes the measurements from Machine 1 under specific conditions, indicating process stability over time.
:::

::: {.column width="50%"}
<img src="media/plots/machine1_control_chart.png" width="100%" height="500px" style="border:none;">
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 2: Process Capability for Machine 1
This histogram shows the distribution of measurements for Machine 1 relative to the Upper and Lower Specification Limits (USL/LSL), alongside a fitted normal distribution.
:::

::: {.column width="50%"}
<img src="media/plots/machine1_capability_chart.png" width="100%" height="500px" style="border:none;">
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 3: Cpk Calculation for Machine 1
The Cpk value for Machine 1 under the specified conditions is calculated to assess its process capability.

```
Machine 1 Cpk: 2.37
```
:::

::: {.column width="50%"}
### Slide 4: Capability Assessment for Machine 1
Based on the calculated Cpk, the process capability of Machine 1 is:

```
The machine is capable under these conditions (Cpk >= 1.33).
```
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 5: Control Chart for Machine 2
This control chart visualizes the measurements from Machine 2 under specific conditions, indicating process stability over time.
:::

::: {.column width="50%"}
<img src="media/plots/machine2_control_chart.png" width="100%" height="500px" style="border:none;">
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 6: Process Capability for Machine 2
This histogram shows the distribution of measurements for Machine 2 relative to the Upper and Lower Specification Limits (USL/LSL), alongside a fitted normal distribution.
:::

::: {.column width="50%"}
<img src="media/plots/machine2_capability_chart.png" width="100%" height="500px" style="border:none;">
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 7: Cpk Calculation for Machine 2
The Cpk value for Machine 2 under the specified conditions is calculated to assess its process capability.

```
Machine 2 Cpk: 1.32
```
:::

::: {.column width="50%"}
### Slide 8: Capability Assessment for Machine 2
Based on the calculated Cpk, the process capability of Machine 2 is:

```
The machine is NOT capable under these conditions (Cpk < 1.33).
```
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 9: Control Chart for Machine 3
This control chart visualizes the measurements from Machine 3 under specific conditions, indicating process stability over time.
:::

::: {.column width="50%"}
<img src="media/plots/machine3_control_chart.png" width="100%" height="500px" style="border:none;">
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 10: Process Capability for Machine 3
This histogram shows the distribution of measurements for Machine 3 relative to the Upper and Lower Specification Limits (USL/LSL), alongside a fitted normal distribution.
:::

::: {.column width="50%"}
<img src="media/plots/machine3_capability_chart.png" width="100%" height="500px" style="border:none;">
:::
::::

---

:::: {.columns}
::: {.column width="50%"}
### Slide 11: Cpk Calculation for Machine 3
The Cpk value for Machine 3 under the specified conditions is calculated to assess its process capability.

```
Machine 3 Cpk: 0.81
```
:::

::: {.column width="50%"}
### Slide 12: Capability Assessment for Machine 3
Based on the calculated Cpk, the process capability of Machine 3 is:

```
The machine is NOT capable under these conditions (Cpk < 1.33).
```
:::
::::
