# Default HID Descriptor

## Raw HID Descriptor

```
05 01 09 0E A1 01 85 01 05 0D 09 21 A1 02 09 00
A1 00 05 09 09 01 15 00 25 01 35 00 45 01 65 00
55 00 75 01 95 01 81 02 05 0D 09 33 81 02 09 00
A1 02 95 06 81 03 05 01 09 37 26 FF 7F 45 00 75
10 95 01 81 06 C1 00 09 30 15 00 25 00 65 11 55
0E 81 42 09 31 81 42 05 0D 09 48 15 3A 25 3A 35
3A 45 3A 55 0F 75 08 81 03 05 0E 09 01 A1 02 09
24 15 00 25 FF 35 00 45 00 65 00 55 00 91 42 09
21 15 01 25 07 91 42 09 25 26 D0 07 75 10 91 42
C1 00 05 0D 09 00 A1 02 05 01 09 48 15 00 26 10
0E 46 10 0E B1 02 C1 00 05 0E 09 01 A1 02 09 24
25 FF 45 00 75 08 B1 42 09 20 15 01 25 07 B1 42
09 28 25 0A B1 42 09 25 26 D0 07 75 10 B1 42 15
00 25 01 45 01 75 01 95 18 B1 03 85 02 09 22 17
37 00 01 00 27 37 00 01 00 45 00 75 20 95 01 B1
02 09 11 A1 02 05 0A 09 03 15 00 75 08 B1 02 09
04 B1 02 09 05 B1 02 C1 00 05 0E 09 10 A1 02 05
0A 09 03 15 03 25 03 36 03 10 46 03 10 B1 02 09
04 15 04 25 04 36 04 10 46 04 10 B1 02 09 05 15
05 25 05 B1 02 C1 00 C1 00 C1 00 C1 00 C1 00
```

## Parsed HID Descriptor

```
0x05, 0x01,        // Usage Page (Generic Desktop Ctrls)
0x09, 0x0E,        // Usage (0x0E)
0xA1, 0x01,        // Collection (Application)
0x85, 0x01,        //   Report ID (1)
0x05, 0x0D,        //   Usage Page (Digitizer)
0x09, 0x21,        //   Usage (Puck)
0xA1, 0x02,        //   Collection (Logical)
0x09, 0x00,        //     Usage (Undefined)
0xA1, 0x00,        //     Collection (Physical)
0x05, 0x09,        //       Usage Page (Button)
0x09, 0x01,        //       Usage (0x01)
0x15, 0x00,        //       Logical Minimum (0)
0x25, 0x01,        //       Logical Maximum (1)
0x35, 0x00,        //       Physical Minimum (0)
0x45, 0x01,        //       Physical Maximum (1)
0x65, 0x00,        //       Unit (None)
0x55, 0x00,        //       Unit Exponent (0)
0x75, 0x01,        //       Report Size (1)
0x95, 0x01,        //       Report Count (1)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x0D,        //       Usage Page (Digitizer)
0x09, 0x33,        //       Usage (Touch)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x09, 0x00,        //       Usage (Undefined)
0xA1, 0x02,        //       Collection (Logical)
0x95, 0x06,        //         Report Count (6)
0x81, 0x03,        //         Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x01,        //         Usage Page (Generic Desktop Ctrls)
0x09, 0x37,        //         Usage (Dial)
0x26, 0xFF, 0x7F,  //         Logical Maximum (32767)
0x45, 0x00,        //         Physical Maximum (0)
0x75, 0x10,        //         Report Size (16)
0x95, 0x01,        //         Report Count (1)
0x81, 0x06,        //         Input (Data,Var,Rel,No Wrap,Linear,Preferred State,No Null Position)
0xC1, 0x00,        //       End Collection
0x09, 0x30,        //       Usage (X)
0x15, 0x00,        //       Logical Minimum (0)
0x25, 0x00,        //       Logical Maximum (0)
0x65, 0x11,        //       Unit (System: SI Linear, Length: Centimeter)
0x55, 0x0E,        //       Unit Exponent (-2)
0x81, 0x42,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State)
0x09, 0x31,        //       Usage (Y)
0x81, 0x42,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State)
0x05, 0x0D,        //       Usage Page (Digitizer)
0x09, 0x48,        //       Usage (0x48)
0x15, 0x3A,        //       Logical Minimum (58)
0x25, 0x3A,        //       Logical Maximum (58)
0x35, 0x3A,        //       Physical Minimum (58)
0x45, 0x3A,        //       Physical Maximum (58)
0x55, 0x0F,        //       Unit Exponent (-1)
0x75, 0x08,        //       Report Size (8)
0x81, 0x03,        //       Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x0E,        //       Usage Page (Reserved 0x0E)
0x09, 0x01,        //       Usage (0x01)
0xA1, 0x02,        //       Collection (Logical)
0x09, 0x24,        //         Usage (0x24)
0x15, 0x00,        //         Logical Minimum (0)
0x25, 0xFF,        //         Logical Maximum (-1)
0x35, 0x00,        //         Physical Minimum (0)
0x45, 0x00,        //         Physical Maximum (0)
0x65, 0x00,        //         Unit (None)
0x55, 0x00,        //         Unit Exponent (0)
0x91, 0x42,        //         Output (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x21,        //         Usage (0x21)
0x15, 0x01,        //         Logical Minimum (1)
0x25, 0x07,        //         Logical Maximum (7)
0x91, 0x42,        //         Output (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x25,        //         Usage (0x25)
0x26, 0xD0, 0x07,  //         Logical Maximum (2000)
0x75, 0x10,        //         Report Size (16)
0x91, 0x42,        //         Output (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0xC1, 0x00,        //       End Collection
0x05, 0x0D,        //       Usage Page (Digitizer)
0x09, 0x00,        //       Usage (Undefined)
0xA1, 0x02,        //       Collection (Logical)
0x05, 0x01,        //         Usage Page (Generic Desktop Ctrls)
0x09, 0x48,        //         Usage (0x48)
0x15, 0x00,        //         Logical Minimum (0)
0x26, 0x10, 0x0E,  //         Logical Maximum (3600)
0x46, 0x10, 0x0E,  //         Physical Maximum (3600)
0xB1, 0x02,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0xC1, 0x00,        //       End Collection
0x05, 0x0E,        //       Usage Page (Reserved 0x0E)
0x09, 0x01,        //       Usage (0x01)
0xA1, 0x02,        //       Collection (Logical)
0x09, 0x24,        //         Usage (0x24)
0x25, 0xFF,        //         Logical Maximum (-1)
0x45, 0x00,        //         Physical Maximum (0)
0x75, 0x08,        //         Report Size (8)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x20,        //         Usage (0x20)
0x15, 0x01,        //         Logical Minimum (1)
0x25, 0x07,        //         Logical Maximum (7)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x28,        //         Usage (0x28)
0x25, 0x0A,        //         Logical Maximum (10)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x25,        //         Usage (0x25)
0x26, 0xD0, 0x07,  //         Logical Maximum (2000)
0x75, 0x10,        //         Report Size (16)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x15, 0x00,        //         Logical Minimum (0)
0x25, 0x01,        //         Logical Maximum (1)
0x45, 0x01,        //         Physical Maximum (1)
0x75, 0x01,        //         Report Size (1)
0x95, 0x18,        //         Report Count (24)
0xB1, 0x03,        //         Feature (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x85, 0x02,        //         Report ID (2)
0x09, 0x22,        //         Usage (0x22)
0x17, 0x37, 0x00, 0x01, 0x00,  //         Logical Minimum (65590)
0x27, 0x37, 0x00, 0x01, 0x00,  //         Logical Maximum (65590)
0x45, 0x00,        //         Physical Maximum (0)
0x75, 0x20,        //         Report Size (32)
0x95, 0x01,        //         Report Count (1)
0xB1, 0x02,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x09, 0x11,        //         Usage (0x11)
0xA1, 0x02,        //         Collection (Logical)
0x05, 0x0A,        //           Usage Page (Ordinal)
0x09, 0x03,        //           Usage (0x03)
0x15, 0x00,        //           Logical Minimum (0)
0x75, 0x08,        //           Report Size (8)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x09, 0x04,        //           Usage (0x04)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x09, 0x05,        //           Usage (0x05)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0xC1, 0x00,        //         End Collection
0x05, 0x0E,        //         Usage Page (Reserved 0x0E)
0x09, 0x10,        //         Usage (0x10)
0xA1, 0x02,        //         Collection (Logical)
0x05, 0x0A,        //           Usage Page (Ordinal)
0x09, 0x03,        //           Usage (0x03)
0x15, 0x03,        //           Logical Minimum (3)
0x25, 0x03,        //           Logical Maximum (3)
0x36, 0x03, 0x10,  //           Physical Minimum (4099)
0x46, 0x03, 0x10,  //           Physical Maximum (4099)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x09, 0x04,        //           Usage (0x04)
0x15, 0x04,        //           Logical Minimum (4)
0x25, 0x04,        //           Logical Maximum (4)
0x36, 0x04, 0x10,  //           Physical Minimum (4100)
0x46, 0x04, 0x10,  //           Physical Maximum (4100)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x09, 0x05,        //           Usage (0x05)
0x15, 0x05,        //           Logical Minimum (5)
0x25, 0x05,        //           Logical Maximum (5)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0xC1, 0x00,        //         End Collection
0xC1, 0x00,        //       End Collection
0xC1, 0x00,        //     End Collection
0xC1, 0x00,        //   End Collection
0xC1, 0x00,        // End Collection

// 319 bytes
```