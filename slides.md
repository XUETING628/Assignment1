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

<!-- __AUDIO_INTRO_DO_NOT_TOUCH__ -->

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

## Control Chart for PartLength

:::{.cols}
:::{.col}
This control chart visually represents the process behavior of 'PartLength' for Machines 1, 2, and 3 under the specified conditions (Temperature 338K, Pressure 200kPa).

The chart helps to identify if the process is in statistical control, meaning that variation is only due to common causes and not special causes.
:::
:::{.col}
<iframe data-src='media/plots/control_chart_machine_123.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::

---

## Process Capability Chart for PartLength

:::{.cols}
:::{.col}
This process capability chart assesses if the process is capable of producing output within the specified limits. The target is 50, with a Lower Specification Limit (LSL) of 45 and an Upper Specification Limit (USL) of 55.

It helps to understand how well the process output fits between the customer's requirements.
:::
:::{.col}
<iframe data-src='media/plots/capability_chart_machine_123.html' width='100%' height='500px' style='border:none;'></iframe>
:::
:::

---

## Process Capability Metrics

:::{.cols}
:::{.col}
Based on the analysis for Machines 1, 2, and 3 at 338K Temperature and 200kPa Pressure, with a Target of 50, USL of 55, and LSL of 45, the key process capability indices are:

*   **Cp (Process Capability Index):** 2.200
*   **Cpk (Process Capability Index, Lower):** 1.891

These values indicate that the process is highly capable, as both Cp and Cpk are significantly greater than 1.33 (a commonly accepted minimum for a capable process).

*   **Cp** measures the potential capability, assuming the process is perfectly centered.
*   **Cpk** measures the actual capability, taking into account how centered the process is relative to the specification limits.
:::
:::{.col}
**Interpretation:**

With a Cp of 2.200, the process has a wide margin between its natural variation and the specification limits. A Cpk of 1.891 suggests that the process is well-centered and able to consistently produce parts within the specified range.

This is a strong indication of a robust manufacturing process for 'PartLength' under these conditions.
:::
:::
