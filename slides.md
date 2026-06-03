
---

## Control Chart for PartLength (Machine 1)

::{".cols"}
::{".col"}
This control chart visually represents the process behavior of 'PartLength' for **Machine 1** under the specified conditions (Temperature 338K, Pressure 200kPa).

The chart helps to identify if the process is in statistical control, meaning that variation is only due to common causes and not special causes.
::{/col}
::{".col"}
<iframe data-src='media/plots/control_chart_machine_1.html' width='100%' height='500px' style='border:none;'></iframe>
::{/col}
::{/cols}

---

## Process Capability Chart for PartLength (Machine 1)

::{".cols"}
::{".col"}
This process capability chart assesses if the process is capable of producing output within the specified limits for **Machine 1**. The target is 50, with a Lower Specification Limit (LSL) of 45 and an Upper Specification Limit (USL) of 55.

It helps to understand how well the process output fits between the customer's requirements.
::{/col}
::{".col"}
<iframe data-src='media/plots/capability_chart_machine_1.html' width='100%' height='500px' style='border:none;'></iframe>
::{/col}
::{/cols}

---

## Process Capability Metrics (Machine 1)

::{".cols"}
::{".col"}
Based on the analysis for **Machine 1** at 338K Temperature and 200kPa Pressure, with a Target of 50, USL of 55, and LSL of 45, the key process capability indices are:

*   **Cp (Process Capability Index):** 3.211
*   **Cpk (Process Capability Index, Lower):** 2.171

These values indicate that the process is {'highly capable' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else 'not fully capable' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and (cp_scalar <= 1.33 or cpk_scalar <= 1.33)) else 'N/A'}

as both Cp and Cpk are {'significantly' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else ''} greater than 1.33 (a commonly accepted minimum for a capable process).

*   **Cp** measures the potential capability, assuming the process is perfectly centered.
*   **Cpk** measures the actual capability, taking into account how centered the process is relative to the specification limits.
::{/col}
::{".col"}
**Interpretation for Machine 1:**

With a Cp of 3.211, the process has a wide margin between its natural variation and the specification limits. A Cpk of 2.171 suggests that the process is well-centered and able to consistently produce parts within the specified range.

This is a {'strong' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else 'moderate' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and (cp_scalar > 1 or cpk_scalar > 1)) else 'weak'} indication of a robust manufacturing process for 'PartLength' under these conditions.
::{/col}
::{/cols}

---

## Control Chart for PartLength (Machine 2)

::{".cols"}
::{".col"}
This control chart visually represents the process behavior of 'PartLength' for **Machine 2** under the specified conditions (Temperature 338K, Pressure 200kPa).

The chart helps to identify if the process is in statistical control, meaning that variation is only due to common causes and not special causes.
::{/col}
::{".col"}
<iframe data-src='media/plots/control_chart_machine_2.html' width='100%' height='500px' style='border:none;'></iframe>
::{/col}
::{/cols}

---

## Process Capability Chart for PartLength (Machine 2)

::{".cols"}
::{".col"}
This process capability chart assesses if the process is capable of producing output within the specified limits for **Machine 2**. The target is 50, with a Lower Specification Limit (LSL) of 45 and an Upper Specification Limit (USL) of 55.

It helps to understand how well the process output fits between the customer's requirements.
::{/col}
::{".col"}
<iframe data-src='media/plots/capability_chart_machine_2.html' width='100%' height='500px' style='border:none;'></iframe>
::{/col}
::{/cols}

---

## Process Capability Metrics (Machine 2)

::{".cols"}
::{".col"}
Based on the analysis for **Machine 2** at 338K Temperature and 200kPa Pressure, with a Target of 50, USL of 55, and LSL of 45, the key process capability indices are:

*   **Cp (Process Capability Index):** 1.429
*   **Cpk (Process Capability Index, Lower):** 1.187

These values indicate that the process is {'highly capable' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else 'not fully capable' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and (cp_scalar <= 1.33 or cpk_scalar <= 1.33)) else 'N/A'}

as both Cp and Cpk are {'significantly' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else ''} greater than 1.33 (a commonly accepted minimum for a capable process).

*   **Cp** measures the potential capability, assuming the process is perfectly centered.
*   **Cpk** measures the actual capability, taking into account how centered the process is relative to the specification limits.
::{/col}
::{".col"}
**Interpretation for Machine 2:**

With a Cp of 1.429, the process has a wide margin between its natural variation and the specification limits. A Cpk of 1.187 suggests that the process is well-centered and able to consistently produce parts within the specified range.

This is a {'strong' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else 'moderate' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and (cp_scalar > 1 or cpk_scalar > 1)) else 'weak'} indication of a robust manufacturing process for 'PartLength' under these conditions.
::{/col}
::{/cols}

---

## Control Chart for PartLength (Machine 3)

::{".cols"}
::{".col"}
This control chart visually represents the process behavior of 'PartLength' for **Machine 3** under the specified conditions (Temperature 338K, Pressure 200kPa).

The chart helps to identify if the process is in statistical control, meaning that variation is only due to common causes and not special causes.
::{/col}
::{".col"}
<iframe data-src='media/plots/control_chart_machine_3.html' width='100%' height='500px' style='border:none;'></iframe>
::{/col}
::{/cols}

---

## Process Capability Chart for PartLength (Machine 3)

::{".cols"}
::{".col"}
This process capability chart assesses if the process is capable of producing output within the specified limits for **Machine 3**. The target is 50, with a Lower Specification Limit (LSL) of 45 and an Upper Specification Limit (USL) of 55.

It helps to understand how well the process output fits between the customer's requirements.
::{/col}
::{".col"}
<iframe data-src='media/plots/capability_chart_machine_3.html' width='100%' height='500px' style='border:none;'></iframe>
::{/col}
::{/cols}

---

## Process Capability Metrics (Machine 3)

::{".cols"}
::{".col"}
Based on the analysis for **Machine 3** at 338K Temperature and 200kPa Pressure, with a Target of 50, USL of 55, and LSL of 45, the key process capability indices are:

*   **Cp (Process Capability Index):** 2.908
*   **Cpk (Process Capability Index, Lower):** 2.132

These values indicate that the process is {'highly capable' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else 'not fully capable' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and (cp_scalar <= 1.33 or cpk_scalar <= 1.33)) else 'N/A'}

as both Cp and Cpk are {'significantly' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else ''} greater than 1.33 (a commonly accepted minimum for a capable process).

*   **Cp** measures the potential capability, assuming the process is perfectly centered.
*   **Cpk** measures the actual capability, taking into account how centered the process is relative to the specification limits.
::{/col}
::{".col"}
**Interpretation for Machine 3:**

With a Cp of 2.908, the process has a wide margin between its natural variation and the specification limits. A Cpk of 2.132 suggests that the process is well-centered and able to consistently produce parts within the specified range.

This is a {'strong' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cp_scalar > 1.33 and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and cpk_scalar > 1.33) else 'moderate' if (cp_val is not None and (isinstance(cp_scalar, float) and not pd.isna(cp_scalar)) and cpk_val is not None and (isinstance(cpk_scalar, float) and not pd.isna(cpk_scalar)) and (cp_scalar > 1 or cpk_scalar > 1)) else 'weak'} indication of a robust manufacturing process for 'PartLength' under these conditions.
::{/col}
::{/cols}
