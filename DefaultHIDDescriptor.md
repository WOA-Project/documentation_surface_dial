# Default HID Descriptor

## Raw HID Descriptor

```
05 01 09 0E A1 01 85 01 05 0D 09 21 A1 02 15 00
25 01 75 01 95 01 A1 00 05 09 09 01 81 02 05 0D
09 33 81 02 95 06 81 03 A1 02 05 01 09 37 16 01
80 26 FF 7F 75 10 95 01 81 06 35 00 46 10 0E 15
00 26 10 0E 09 48 B1 02 45 00 C0 55 0E 65 11 46
00 00 26 00 00 09 30 81 42 09 31 46 00 00 26 00
00 81 42 05 0D 09 48 15 3A 25 3A 75 08 55 0F 35
3A 45 3A 81 03 55 00 65 00 35 00 45 00 05 0E 09
01 A1 02 15 00 26 FF 00 09 24 B1 42 09 24 91 42
15 01 25 07 09 20 B1 42 09 21 91 42 25 0A 09 28
B1 42 75 10 26 D0 07 09 25 B1 42 09 25 91 42 85
02 75 20 17 37 00 01 00 27 37 00 01 00 09 22 B1
02 09 11 A1 02 05 0A 95 03 09 03 09 04 09 05 75
08 15 00 25 FF B1 02 C0 05 0E 09 10 A1 02 05 0A
95 01 15 03 25 03 36 03 10 46 03 10 09 03 B1 02
15 04 25 04 36 04 10 46 04 10 09 04 B1 02 15 05
25 05 36 04 10 46 04 10 09 05 B1 02 35 00 45 00
C0 C0 C0 C0 C0
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
0x15, 0x00,        //     Logical Minimum (0)
0x25, 0x01,        //     Logical Maximum (1)
0x75, 0x01,        //     Report Size (1)
0x95, 0x01,        //     Report Count (1)
0xA1, 0x00,        //     Collection (Physical)
0x05, 0x09,        //       Usage Page (Button)
0x09, 0x01,        //       Usage (0x01)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x05, 0x0D,        //       Usage Page (Digitizer)
0x09, 0x33,        //       Usage (Touch)
0x81, 0x02,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x95, 0x06,        //       Report Count (6)
0x81, 0x03,        //       Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0xA1, 0x02,        //       Collection (Logical)
0x05, 0x01,        //         Usage Page (Generic Desktop Ctrls)
0x09, 0x37,        //         Usage (Dial)
0x16, 0x01, 0x80,  //         Logical Minimum (-32767)
0x26, 0xFF, 0x7F,  //         Logical Maximum (32767)
0x75, 0x10,        //         Report Size (16)
0x95, 0x01,        //         Report Count (1)
0x81, 0x06,        //         Input (Data,Var,Rel,No Wrap,Linear,Preferred State,No Null Position)
0x35, 0x00,        //         Physical Minimum (0)
0x46, 0x10, 0x0E,  //         Physical Maximum (3600)
0x15, 0x00,        //         Logical Minimum (0)
0x26, 0x10, 0x0E,  //         Logical Maximum (3600)
0x09, 0x48,        //         Usage (0x48)
0xB1, 0x02,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x45, 0x00,        //         Physical Maximum (0)
0xC0,              //       End Collection
0x55, 0x0E,        //       Unit Exponent (-2)
0x65, 0x11,        //       Unit (System: SI Linear, Length: Centimeter)
0x46, 0x00, 0x00,  //       Physical Maximum (0)
0x26, 0x00, 0x00,  //       Logical Maximum (0)
0x09, 0x30,        //       Usage (X)
0x81, 0x42,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State)
0x09, 0x31,        //       Usage (Y)
0x46, 0x00, 0x00,  //       Physical Maximum (0)
0x26, 0x00, 0x00,  //       Logical Maximum (0)
0x81, 0x42,        //       Input (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State)
0x05, 0x0D,        //       Usage Page (Digitizer)
0x09, 0x48,        //       Usage (0x48)
0x15, 0x3A,        //       Logical Minimum (58)
0x25, 0x3A,        //       Logical Maximum (58)
0x75, 0x08,        //       Report Size (8)
0x55, 0x0F,        //       Unit Exponent (-1)
0x35, 0x3A,        //       Physical Minimum (58)
0x45, 0x3A,        //       Physical Maximum (58)
0x81, 0x03,        //       Input (Const,Var,Abs,No Wrap,Linear,Preferred State,No Null Position)
0x55, 0x00,        //       Unit Exponent (0)
0x65, 0x00,        //       Unit (None)
0x35, 0x00,        //       Physical Minimum (0)
0x45, 0x00,        //       Physical Maximum (0)
0x05, 0x0E,        //       Usage Page (Reserved 0x0E)
0x09, 0x01,        //       Usage (0x01)
0xA1, 0x02,        //       Collection (Logical)
0x15, 0x00,        //         Logical Minimum (0)
0x26, 0xFF, 0x00,  //         Logical Maximum (255)
0x09, 0x24,        //         Usage (0x24)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x24,        //         Usage (0x24)
0x91, 0x42,        //         Output (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x15, 0x01,        //         Logical Minimum (1)
0x25, 0x07,        //         Logical Maximum (7)
0x09, 0x20,        //         Usage (0x20)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x21,        //         Usage (0x21)
0x91, 0x42,        //         Output (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x25, 0x0A,        //         Logical Maximum (10)
0x09, 0x28,        //         Usage (0x28)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x75, 0x10,        //         Report Size (16)
0x26, 0xD0, 0x07,  //         Logical Maximum (2000)
0x09, 0x25,        //         Usage (0x25)
0xB1, 0x42,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x09, 0x25,        //         Usage (0x25)
0x91, 0x42,        //         Output (Data,Var,Abs,No Wrap,Linear,Preferred State,Null State,Non-volatile)
0x85, 0x02,        //         Report ID (2)
0x75, 0x20,        //         Report Size (32)
0x17, 0x37, 0x00, 0x01, 0x00,  //         Logical Minimum (65590)
0x27, 0x37, 0x00, 0x01, 0x00,  //         Logical Maximum (65590)
0x09, 0x22,        //         Usage (0x22)
0xB1, 0x02,        //         Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x09, 0x11,        //         Usage (0x11)
0xA1, 0x02,        //         Collection (Logical)
0x05, 0x0A,        //           Usage Page (Ordinal)
0x95, 0x03,        //           Report Count (3)
0x09, 0x03,        //           Usage (0x03)
0x09, 0x04,        //           Usage (0x04)
0x09, 0x05,        //           Usage (0x05)
0x75, 0x08,        //           Report Size (8)
0x15, 0x00,        //           Logical Minimum (0)
0x25, 0xFF,        //           Logical Maximum (-1)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0xC0,              //         End Collection
0x05, 0x0E,        //         Usage Page (Reserved 0x0E)
0x09, 0x10,        //         Usage (0x10)
0xA1, 0x02,        //         Collection (Logical)
0x05, 0x0A,        //           Usage Page (Ordinal)
0x95, 0x01,        //           Report Count (1)
0x15, 0x03,        //           Logical Minimum (3)
0x25, 0x03,        //           Logical Maximum (3)
0x36, 0x03, 0x10,  //           Physical Minimum (4099)
0x46, 0x03, 0x10,  //           Physical Maximum (4099)
0x09, 0x03,        //           Usage (0x03)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x15, 0x04,        //           Logical Minimum (4)
0x25, 0x04,        //           Logical Maximum (4)
0x36, 0x04, 0x10,  //           Physical Minimum (4100)
0x46, 0x04, 0x10,  //           Physical Maximum (4100)
0x09, 0x04,        //           Usage (0x04)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x15, 0x05,        //           Logical Minimum (5)
0x25, 0x05,        //           Logical Maximum (5)
0x36, 0x04, 0x10,  //           Physical Minimum (4100)
0x46, 0x04, 0x10,  //           Physical Maximum (4100)
0x09, 0x05,        //           Usage (0x05)
0xB1, 0x02,        //           Feature (Data,Var,Abs,No Wrap,Linear,Preferred State,No Null Position,Non-volatile)
0x35, 0x00,        //           Physical Minimum (0)
0x45, 0x00,        //           Physical Maximum (0)
0xC0,              //         End Collection
0xC0,              //       End Collection
0xC0,              //     End Collection
0xC0,              //   End Collection
0xC0,              // End Collection

// 277 bytes
```