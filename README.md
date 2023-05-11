# awesome-riscv

## Organzation:
- [chipsalliance](https://github.com/chipsalliance/): 
Chips Alliance is an organization that brings together industry leaders and university researchers to accelerate the development of open-source hardware and software solutions for semiconductor design. It was established in March 2019 as a project of the Linux Foundation and has grown to include more than 30 members, including Google, Western Digital, NXP Semiconductors, and SiFive. The organization aims to promote collaboration and innovation in the semiconductor industry by providing a platform for developers to share ideas, resources, and expertise. Chips Alliance focuses on developing open-source toolchains, verification IP, reference designs, and other infrastructure to support chip design projects based on RISC-V and other open architectures. By promoting open standards and collaboration, Chips Alliance hopes to accelerate innovation and reduce the cost and time-to-market of new chip designs.   
- [sifive](https://github.com/sifive): SiFive is a company that was founded in 2015 by Krste Asanović, Yunsup Lee, and Andrew Waterman, who were researchers from the University of California Berkeley. The company is known for introducing RISC-V to the world and being the first to produce a chip that implements the RISC-V ISA. SiFive released the Freedom Everywhere 310 SoC and the HiFive development board in 2016. SiFive is dedicated to transforming the future of computing by empowering all companies to deliver advanced solutions using RISC-V technology. According to their website, they are pioneers who have harnessed the limitless potential of RISC-V to define and shape what comes next in the world of computing.  
- [bluespec](https://github.com/bluespec): Bluespec is a semiconductor design tools company founded in June 2003 by MIT professor Arvind. Arvind had previously founded Sandburst in 2000, which produced chips for 10Gbit Ethernet routers. Bluespec has two product lines and provides advanced synthesis tools such as Electronic System Level (ESL) synthesis for ASIC and FPGA hardware designers and architects. In addition, Bluespec also offers processor IP and development tools in the RISC-V processor field to help customers achieve the highest level of quality, performance, and innovation in their applications.  
- [pulp](https://github.com/pulp-platform/): PULP (Parallel Ultra-Low-Power) is an open-source multi-core computing platform part of the of the ongoing collaboration between ETH Zurich and the University of Bologna - started in 2013.  
- [openhwgroup](https://github.com/openhwgroup): The OpenHW Group is a non-profit organization that was established in June 2019 with the goal of developing open-source hardware for embedded systems. The group is comprised of leaders from the semiconductor industry, academia, and the broader open-source community, and its mission is to create high-quality, low-cost processor IP cores and related ecosystem components that can be used in commercial and open-source projects. The OpenHW Group's focus is on developing and promoting the use of open-source hardware based on the RISC-V ISA and related technologies. They seek to provide a robust and predictable design process for hardware developers by creating specifications and related tools that allow for greater innovation and collaboration in the industry. Their goal is to create a new paradigm for silicon design that leverages the power of open-source development methodologies and helps to reduce the complexity and cost of hardware design. The OpenHW Group encourages the adoption of open-source hardware solutions across a wide range of markets and applications, from Internet of Things (IoT) devices to high-performance computing systems.  
- [lowRISC](https://github.com/lowRISC): lowRISC is a non-profit company based in Cambridge, UK that focuses on collaborative engineering to develop and maintain open-source silicon designs and tools, particularly in the context of the RISC-V processor architecture. The company aims to provide a neutral platform for multi-partner projects that deliver high-quality IP and tools, enabling shared investment in pre-competitive technologies and open standards, thereby providing a solid foundation for the rapid development cycles of next-generation silicon products. As an active participant in the RISC-V ecosystem, lowRISC stewards the OpenTitan project, which is focused on developing an open-source security framework for use in silicon designs.  
- [SpinalHDL](https://github.com/SpinalHDL): SpinalHDL is an open-source hardware description language (HDL) that is used for designing digital circuits. It provides a more concise and powerful syntax compared to traditional HDLs like VHDL and Verilog. SpinalHDL generates VHDL or Verilog files in a compatible format for EDA (Electronic Design Automation) tools. Unlike HLS (High-Level Synthesis) approaches, SpinalHDL focuses on creating designs through simple elements like flip-flops, gates, and if/case statements. It is not based on the event-driven paradigm. SpinalHDL has several advantages over traditional HDLs such as being less verbose and providing higher levels of abstraction with less complexity. It can be used as an alternative to VHDL or Verilog for designing complex digital circuits.   
- [YosysHQ](https://github.com/YosysHQ/): YosysHQ is the organization responsible for maintaining the open-source EDA (Electronic Design Automation) tool Yosys and related projects such as nextpnr, Project IceStorm, Project Trellis, and more. YosysHQ is made up of a team of developers who are pushing the boundaries of EDA in interesting and unexpected ways and making these tools and methodologies available for professionals, hobbyists, and academics alike. Yosys is a framework for Verilog RTL synthesis and currently has extensive Verilog-2005 support, providing a basic set of synthesis algorithms for various application domains. Through YosysHQ, the development of Yosys and related open-source hardware tools and projects is being propelled forward, promoting collaboration, innovation, and accessibility in the realm of EDA.

## Open Source Core Implementations

|Repository|Language|isa|microarch|Target|License|star|
|-|-|-|-|-|-|-|
|[Rocket@chipsalliance](https://github.com/chipsalliance/rocket-chip)|Scala,Chisel|rv32ima|5? stage|ASIC|BSD| ![](https://img.shields.io/github/stars/chipsalliance/rocket-chip?label=★)
[boom](https://github.com/riscv-boom/riscv-boom)|Scala,Chisel|RV64GC|out-of-order|FPGA,ASIC|BSD,Apache-2|![](https://img.shields.io/github/stars/riscv-boom/riscv-boom)
|[XiangShan](https://github.com/OpenXiangShan/XiangShan)|Scala,Chisel|RV64GCBK|Superscalar|ASIC|Mulan|![](https://img.shields.io/github/stars/OpenXiangShan/XiangShan?label=★)
|[Flute@bluespec](https://github.com/bluespec/Flute)|haskell,Bluespec|RV/64I[a][c][m][f][d]|5-stage in-order|ASIC|Apache|![](https://img.shields.io/github/stars/bluespec/Flute?label=★)
|[Piccolo@bluespec](https://github.com/bluespec/Piccolo)|haskell,Bluespec|RV/64I[a][c][m][f][d]|3-stage in-order|ASIC|Apache|![](https://img.shields.io/github/stars/bluespec/Piccolo?label=★)
|[Toooba@bluespec](https://github.com/bluespec/Toooba)|haskell,Bluespec|RV/64I[a][c][m][f][d]|superscalar, deep, out-of-order|ASIC|Apache|![](https://img.shields.io/github/stars/bluespec/Piccolo?label=★)
|[snitch@pulp](https://github.com/pulp-platform/snitch)|SystemVerilog|rv32{i,e}|1 stage||Apache-2.0|![](https://img.shields.io/github/stars/pulp-platform/snitch?label=★)
|[CV32E40P@pulp](https://github.com/openhwgroup/cv32e40p)|SystemVerilog|rv32imcf|4 stage|FPGA,ASIC|Solderpad| ![](https://img.shields.io/github/stars/openhwgroup/cv32e40p?label=★)
|[cva6@pulp](https://github.com/openhwgroup/cva6)|SystemVerilog|rv64gc|6 stage|FPGA,ASIC|Solderpad | ![](https://img.shields.io/github/stars/openhwgroup/cva6?label=★)
|[Ibex@pulp](https://github.com/lowRISC/ibex)|SystemVerilog|rv32imc|2 stage|ASIC|Apache2| ![](https://img.shields.io/github/stars/lowRISC/ibex?label=★)
|[PicoRV32@YosysHQ](https://github.com/YosysHQ/picorv32)|Verilog|rv32{i,e}[m][c]|?|FPGA,ASIC|ISC| ![](https://img.shields.io/github/stars/YosysHQ/picorv32?label=★)
|[VexRiscv](https://github.com/SpinalHDL/VexRiscv)|Scala,SpinalHDL|rv32i[m][c][a]|2-5 stage|FPGA|MIT| ![](https://img.shields.io/github/stars/SpinalHDL/VexRiscv?label=★)
|[NaxRiscv](https://github.com/SpinalHDL/NaxRiscv)|Scala,SpinalHDL|rv32/64imasu|out-of-order, superscalar, register renaming|FPGA|MIT| ![](https://img.shields.io/github/stars/SpinalHDL/NaxRiscv?label=★)
|[Minerva](https://github.com/lambdaconcept/minerva)|Python,nMigen|rv32im|6 stage|FPGA|BSD| ![](https://img.shields.io/github/stars/lambdaconcept/minerva?label=★)
|[riscv-mini](https://github.com/ucb-bar/riscv-mini)|Scala,Chisel|rv32i|3 stage|ASIC|BSD| ![](https://img.shields.io/github/stars/ucb-bar/riscv-mini?label=★)
|[SERV](https://github.com/olofk/serv)|Verilog|rv32|0-calories|FPGA|ISC| ![](https://img.shields.io/github/stars/olofk/serv?label=★)
|[SweRV](https://github.com/chipsalliance/Cores-SweRV)|SystemVerilog|rv32imc|9-stage, dual-issue, superscalar|ASIC|Apache2| ![](https://img.shields.io/github/stars/chipsalliance/Cores-SweRV?label=★)
|[wyvernSemi](https://github.com/wyvernSemi/riscV)|Verilog|rv32imafdc|5 stage|FPGA|GPL3| ![](https://img.shields.io/github/stars/wyvernSemi/riscV?label=★)
|[NEORV32](https://github.com/stnolting/neorv32)|VHDL|rv32[i/e][a][c][m][u]x[Zbb]... |2 stage|FPGA | BSD3 | ![](https://img.shields.io/github/stars/stnolting/neorv32?label=★)
|[vroom](https://github.com/MoonbaseOtago/vroom)|Verilog|rv64imafdchb[v]|OOO, 7+ stage, SMT-2|ASIC|GPL3| ![](https://img.shields.io/github/stars/MoonbaseOtago/vroom?label=★)
|[FWRISC-S](https://github.com/Featherweight-IP/fwrisc)|SystemVerilog|rv32i[mc]||FPGA|Apache2| ![](https://img.shields.io/github/stars/Featherweight-IP/fwrisc?label=★)

## Verification
- [riscv-formal](https://github.com/YosysHQ/riscv-formal)  
- [riscv-dv](https://github.com/chipsalliance/riscv-dv)

## Instruction Set Simulator
- [spike](https://github.com/riscv/riscv-isa-sim)  
- [riscv-ovpsim](https://github.com/riscv/riscv-ovpsim)  
- [whisper](https://github.com/westerndigitalcorporation/swerv-ISS)  
- [sail-riscv](https://github.com/rems-project/sail-riscv)

## todo

- [ ] list microarch
- [ ] list performance(coremark score, IPC)
- [ ] list area(gate number, lut number, or area in some process)
- [ ] list power

