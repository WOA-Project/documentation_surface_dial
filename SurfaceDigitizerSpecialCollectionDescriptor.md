# Surface Digitizer Special Collection Descriptor

## Parameters

```
XPhysicalMax: { 0x63, 0x0C }
XLogicalMax:  { 0x80, 0x25 }

YPhysicalMax: { 0x42, 0x08 }
YLogicalMax:  { 0x20, 0x1C }
```

## Raw HID Descriptor

```
06 09 FF 0A 00 01 A1 01 85 50 09 00 A1 00 15 00
25 01 35 00 45 01 65 00 55 00 75 01 95 08 81 03
0A 01 01 26 FF FF 45 00 75 10 95 01 81 02 05 0D
09 01 A1 02 09 42 25 01 45 01 75 01 81 02 81 03
09 47 81 02 95 0D 81 03 09 51 26 FF FF 45 00 75
10 95 01 81 02 05 01 09 30 26 80 25 46 63 0C 65
11 55 0E 95 02 81 02 09 31 26 20 1C 46 42 08 81
02 05 0D 09 48 26 80 25 46 63 0C 95 01 81 02 09
49 26 20 1C 46 42 08 81 02 C1 00 09 54 25 FF 45
00 65 00 55 00 75 08 81 02 25 01 45 01 75 01 95
18 81 03 09 56 27 FF FF FF 0F 45 00 75 20 95 01
81 02 C1 00 C1 00
```

## Parsed HID Descriptor

```
0x06, 0x09, 0xFF,  // Usage Page (Vendor Defined 0xFF09)
0x0A, 0x00, 0x01,  // Usage (0x0100)
0xA1, 0x01,        // Collection (Application)
0x85, 0x50,        //   Report ID (80)
0x09, 0x00,        //   Usage (0x00)
0xA1, 0x00,        //   Collection (Physical)
0x15, 0x00,        //     Logical Minimum (0)
0x25, 0x01,        //     Logical Maximum (1)
0x35, 0x00,        //     Physical Minimum (0)
0x45, 0x01,        //     Physical Maximum (1)
0x65, 0x00,        //     Unit (None)
0x55, 0x00,        //     Unit Exponent (0)
0x75, 0x01,        //     Report Size (1)
0x95, 0x08,        //     Report Count (8)
0x81, 0x03,        //     Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x0A, 0x01, 0x01,  //     Usage (0x0101)
0x26, 0xFF, 0xFF,  //     Logical Maximum (-1)
0x45, 0x00,        //     Physical Maximum (0)
0x75, 0x10,        //     Report Size (16)
0x95, 0x01,        //     Report Count (1)
0x81, 0x02,        //     Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x0D,        //     Usage Page (Digitizer)
0x09, 0x01,        //     Usage (Digitizer)
0xA1, 0x02,        //     Collection (Logical)
0x09, 0x42,        //       Usage (Tip Switch)
0x25, 0x01,        //       Logical Maximum (1)
0x45, 0x01,        //       Physical Maximum (1)
0x75, 0x01,        //       Report Size (1)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x81, 0x03,        //       Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x47,        //       Usage (0x47)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x95, 0x0D,        //       Report Count (13)
0x81, 0x03,        //       Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x51,        //       Usage (0x51)
0x26, 0xFF, 0xFF,  //       Logical Maximum (-1)
0x45, 0x00,        //       Physical Maximum (0)
0x75, 0x10,        //       Report Size (16)
0x95, 0x01,        //       Report Count (1)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x01,        //       Usage Page (Generic Desktop Ctrls)
0x09, 0x30,        //       Usage (X)
0x26, 0x80, 0x25,  //       Logical Maximum (9600)
0x46, 0x63, 0x0C,  //       Physical Maximum (3171)
0x65, 0x11,        //       Unit (System: SI Linear, Length: Centimeter)
0x55, 0x0E,        //       Unit Exponent (-2)
0x95, 0x02,        //       Report Count (2)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x31,        //       Usage (Y)
0x26, 0x20, 0x1C,  //       Logical Maximum (7200)
0x46, 0x42, 0x08,  //       Physical Maximum (2114)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x0D,        //       Usage Page (Digitizer)
0x09, 0x48,        //       Usage (0x48)
0x26, 0x80, 0x25,  //       Logical Maximum (9600)
0x46, 0x63, 0x0C,  //       Physical Maximum (3171)
0x95, 0x01,        //       Report Count (1)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x49,        //       Usage (0x49)
0x26, 0x20, 0x1C,  //       Logical Maximum (7200)
0x46, 0x42, 0x08,  //       Physical Maximum (2114)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0xC1, 0x00,        //     End Collection
0x09, 0x54,        //     Usage (0x54)
0x25, 0xFF,        //     Logical Maximum (-1)
0x45, 0x00,        //     Physical Maximum (0)
0x65, 0x00,        //     Unit (None)
0x55, 0x00,        //     Unit Exponent (0)
0x75, 0x08,        //     Report Size (8)
0x81, 0x02,        //     Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x25, 0x01,        //     Logical Maximum (1)
0x45, 0x01,        //     Physical Maximum (1)
0x75, 0x01,        //     Report Size (1)
0x95, 0x18,        //     Report Count (24)
0x81, 0x03,        //     Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x56,        //     Usage (0x56)
0x27, 0xFF, 0xFF, 0xFF, 0x0F,  //     Logical Maximum (268435454)
0x45, 0x00,        //     Physical Maximum (0)
0x75, 0x20,        //     Report Size (32)
0x95, 0x01,        //     Report Count (1)
0x81, 0x02,        //     Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0xC1, 0x00,        //   End Collection
0xC1, 0x00,        // End Collection

// 182 bytes
```