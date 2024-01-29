# x99ud5bifurcation
*UEFI Variables required to enable PCIE bifurcation on GIGABYTE x99 UD5*

If you reached this place, you should already be familiar with [UEFI Variable Tool](https://github.com/GeographicCone/UefiVarTool) and how to examine and modify your motherboard firmware.
Files in this repository are provided for reference only, they might not work even for similar GIGABYTE boards.

### As seen in GA X99 UD5 manual:
```
2 x PCI Express x16 slots, running at x16 (PCIE_1, PCIE_2)
* For optimum performance, if only one PCI Express graphics card is to be installed, be sure to install it in the PCIE_1 slot; if you are installing two PCI Express graphics cards, it is recommended that you install them in the PCIE_1 and PCIE_2 slots.

2 x PCI Express x16 slots, running at x8 (PCIE_3, PCIE_4)
* The PCIE_4 slot shares bandwidth with the PCIE_1 slot. When the PCIE_4 slot is populated, the PCIE_1 slot will operate at up to x8 mode.
* When an 28 lane CPU is installed, the PCIE_2 slot operates at up to x8 mode and the PCIE_3 operates at up to x4 mode.
(All PCI Express x16 slots conform to PCI Express 3.0 standard.)
```
![Marketing](https://github.com/interj/x99ud5bifurcation/assets/7340707/fe096937-c079-4a79-9266-7049f3dbaf42)
![Diagram](https://github.com/interj/x99ud5bifurcation/assets/7340707/a881f46e-8c7e-4da5-aec4-8eeea66065f7)


**Top x16 port (PCIE_1) is wired to share 8 lanes with the second port (PCIE_4) that has x8 wiring. Bifurcation doesn't seem possible on these two ports.**
