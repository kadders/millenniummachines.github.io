# FMJ Assembly

![](../img/fmj_assembly/fmj_assembly.png)

!!! note "FMJ"
    The Full Metal Jacket is an optional reinforcement for the Z-Axis that improves its' rigidity and strength significantly. If you're looking to cut metals, then you should think about installing the FMJ from the get-go.

!!! tip annotate "Standard Assembly"
    The following information applies _only_ if you are building your Milo with FMJ plates. If you do not have FMJ plates and instead use 3D-printed column joining plates, please follow [Installing the Column Plates](./60_z_axis_assembly.md#installing-the-column-plates) instead.

*[FMJ]: Full Metal Jacket

## FMJ Sourcing
FMJs cannot be made on Milo due to their size - so you will need to acquire them via different means.

<!-- Check the [Sourcing Guide](../../bom/sourcing_guide.md) for FMJ kits. !-->

If self-sourcing, FMJs should be laser-cut, ideally from Mild Steel, which gives you the best bang for your buck.

FMJs can extend your Z clearance, the maximum work-piece and work-holding height that can move under the Z-column overhang. The stock clearance is 60mm, and with the maximum size FMJ, this can be extended to 120mm.

If using the FMJ to extend your clearance, you will need to increase the length of the `A` and `B` extrusions (detailed in [Identifying Extrusions](#identifying-extrusions)) by the difference from the standard clearance. For 120mm clearance, you will need 320mm C-Beams (`120-60 + 260 = 320mm`).

The designs are available in the [User Mods Repository](https://github.com/MillenniumMachines/UserMods/tree/main/Millennium-Milo-V1.5-MODS/Techmorphic/Techmorphic-FMJ-para-plates) - the Fusion360 file is parametric, so you will need to check and set your parameters for length and bolt hole sizes before exporting for cutting.

Services like SendCutSend in the US or Fractory in the EU can produce FMJs at a reasonable price, and they offer discounts for bulk runs.

Remember that a set of FMJs contains _two_ plates, one for either side of the Z column.

If obtaining these plates with a non-durable surface finish (Mild Steel for example), you must paint the raw FMJs to protect them from corrosion. We find sprayed truck-bed liner or appliance enamel provides suitable coating durability, but feel free to experiment with other high-durability coatings.

---

## Identifying Extrusions

This section of the build contains several C-beams that are close together. To help you identify which parts are which, lay out your extrusions like the diagram below. The next steps will then highlight which extrusions are used for each step.

!!! info "Components Required"
    ```
    A: Openbuilds 4080x260mm C-Beam
    B: Openbuilds 4080x260mm C-Beam
    C: Openbuilds 4080x250mm C-Beam
    D: Openbuilds 4080x120mm C-Beam
    ```

!!! tip
    The lengths shown are for a standard 60mm clearance build. A 120mm clearance build will have A & B be 60mm longer.

![](../img/z_axis_assembly/y_axis_step_42.png){: .shadow}

---

Extrusions `A` and `B` are the main Z-column extrusions.

![](../img/z_axis_assembly/y_axis_step_43.png){: .shadow}

---

## Z-Axis Rail Assembly

!!! info annotate "Components Required"
    ```
    8 x M3x10mm SHCS
    2 x MGN15 Rail 250mm
    ```

Install the Z rails with only the lower carriages installed onto the `C` extrusion using M3x10mm SHCS.

Make sure the end-most and centre-most bolt holes in each rail are used.

![](../img/fmj_assembly/fmj_step_0.png){: .shadow}

!!! tip
    You can use the rail alignment guides to stop the lower carriages from falling off the vertical rail!

!!! tip annotate "Aligning the Rails"
    Repeat the alignment procedure described for the Y-Axis to ensure your rails are aligned with each other and the extrusion. 

!!! tip annotate "Lubricating the Rails"
    If you didn't lubricate all of the rails when assembling the Y-Axis, ensure these rails are also lubricated as described in the Y-Axis section.

## Column Assembly

Place extrusions `A` and `B` facing each other, creating an internal channel. This is where the ballast box can be installed (later, calm down cowboy!).

Select extrusion `D`.

![](../img/z_axis_assembly/y_axis_step_45.png){: .shadow}

---

Place extrusion `D` at the top of the column with the channel facing _outwards_ (away from extrusions `A` and `B`).

---

Select extrusion `C`.

![](../img/z_axis_assembly/y_axis_step_44.png){: .shadow}

---

Place extrusion `C` on the front of `D`, again with the channel (and rails!) facing _outwards_.

![](../img/fmj_assembly/fmj_step_1.png){: .shadow}

---

!!! tip
    The lower edge of extrusion `C` should be `18mm` above the lower edge of `D`, making room for the lower bearing block.

![](../img/z_axis_assembly/y_axis_step_51.png){: .shadow}

---

## FMJ Installation

!!! info annotate "Components Required"
    ```
    68 x M5x10mm BHCS
    2 x FMJ Plate (1)
    ```
1. :material-factory: See [FMJ Sourcing](#fmj-sourcing) above.

!!! warning
    The length of the M5 BHCS bolts used to attach the FMJ to the column depends on the thickness of your FMJ. The bolts specified here are for a plate thickness of 6mm, which is currently the most common choice and is supplied as standard with the LDO kit.

    If your FMJ plates are not 6mm thick, you should aim for an M5 BHCS that is 4-6mm longer than your plates are thick.

Take one of your FMJ plates and line up the bottom edge of the FMJ shoulder with the bottom edge of the `C` extrusion.

![](../img/fmj_assembly/fmj_step_2.png){: .shadow}

---
![](../img/fmj_assembly/fmj_step_3.png){: .shadow}

---

Bolt the FMJ plate to the extrusion using the M5x10 BHCS.

![](../img/fmj_assembly/fmj_step_4.png){: .shadow}

!!! tip
    The bottom 4 holes will remain without a bolt at this stage.

!!! warning "BE SAFE, LOCK IT!"
    These machines vibrate intensely when running, and fasteners are bound to back out. Don't be afraid to add a little bit of medium-strength threadlock to all your screws to avoid this problem.

!!! hint
    If using spring T-nuts for assembly, having a thin, long, and semi-flexible tool to help guide the nuts into place is a godsend!

---

Turn your half-assembled column over and repeat with the other FMJ plate. Take care to line the second FMJ up with the first!

!!! hint
    Loosely bolt the second FMJ into place, then push the base of the FMJs against a known flat surface so that they are both flush.
    Tighten the second FMJ while in this position so that the plates stay aligned.

---

!!! note
    The cut-outs in the FMJ are for fitting cable hooks and drag-chain mounts. This can be done now, or later when routing cabling and drag-chains.

![](../img/fmj_assembly/fmj_step_5.png){: .shadow}


[Next Chapter: Z-Axis Lower Bearing block](./60_z_axis_assembly.md#lower-bearing-block)