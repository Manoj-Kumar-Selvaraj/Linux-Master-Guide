Power On
│
├── PSU signals stable power
├── CPU fetches reset vector → starts executing firmware (BIOS/UEFI)
│
├── SEC/PEI Phase → CPU, RAM init
├── POST → Test hardware
├── DXE Phase → Load firmware drivers
├── Build ACPI/SMBIOS tables
│
└── Boot Manager → Load Bootloader (e.g., GRUB)
       ↓
       Linux kernel takes over
