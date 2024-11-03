# Minimal Official Setup Requirements

In order for Surface Dial On Screen functionality to work on official devices, the following must be met:

- Surface Dial Paired over BT
- SurfaceDialFilter.sys installed onto the Surface Dial HID Collection 01 (HID over BT)
- IPTS Digitizer exporting // 045E: Microsoft Vendor ID - FF09: Digitizer Collection, Under IPTS, Col0A, UP:FF09, U:0100

The Filter driver waits for the arrival of HID Device Interface bound to 045E: Microsoft Vendor ID - FF09: Digitizer Collection, Under IPTS, Col0A, UP:FF09, U:0100

Once arrived, it queries 4 values that will be inserted into the [Overwritten HID Descriptor](OverwrittenHIDDescriptor.md) of the Surface Dial itself.

These values are the (X,Y) dimensions of the digitizer itself.