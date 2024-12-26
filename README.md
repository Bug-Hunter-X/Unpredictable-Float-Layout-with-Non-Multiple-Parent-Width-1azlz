# Unpredictable Float Layout with Non-Multiple Parent Width

This repository demonstrates an uncommon CSS bug related to the unpredictable behavior of floating elements when the parent container's width is not a multiple of the child's width.  The bug manifests in some browsers, leading to unexpected gaps or overlaps in the layout.

## Bug Description

The provided CSS code uses the `float` property to position elements.  However, when the parent container's width is not perfectly divisible by the children's widths (in this case, 50%), the resulting layout is inconsistent and unreliable across different browsers and rendering engines. This inconsistency arises from how browsers handle floating elements and their interaction with the parent container's available space.

## Solution

The recommended solution involves avoiding relying solely on floats for layout in such scenarios.  Using flexbox or grid provides more predictable and consistent results regardless of the parent container's dimensions.  The solution file demonstrates the correct implementation using flexbox.