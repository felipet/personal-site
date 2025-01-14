+++
title = "About"
date = "2025-01-09"
update = "2025-01-14"
description = "A long description about me"
hideComments = true
weight = 1
Toc = true

+++

# Education

## Master's Degree on Data Science and Computer Engineering

I obtained my Master's degree on [Data Science and Computer Engineering](https://masteres.ugr.es/datcom/) with a final mark of 9.587 out of 10 from the [University of Granada](https://www.ugr.es/en) (Spain). My Master's thesis focused on the design of a SoC-FPGA architecture for high-performance synchronisation applications. In particular, that design aimed to design a White-Rabbit slave node on a system based on Zynq-7000 devices.

The thesis is available on my [Github](https://github.com/felipet/memoria_tfm) space, but is written in Spanish.

    September,2016 to July,2017

## Bachelor Degree on Computer Science

I obtained my Bachelor degree on [Computer Science](https://grados.ugr.es/informatica/informacion/presentacion) with mention on Computer Engineering (specialisation) with a final mark of 8.376 out of 10 from the [University of Granada](https://www.ugr.es/en) (Spain). I chose most of the optional lessons related to digital HW design. My Bachelor thesis focused on the optimisation of a conjugate gradient algorithm for the simulation of spill evolution over a mass of water. Mainly, I beat Intel's Fortran compiler thanks to deep analysis of the organisation of the data (sparse matrices) and the manual usage of AVX instructions via inline assembly code. I also explored the possibility of increasing the performance using GPUs with CUDA.

    October,2010 to September,2015

# Professional Career

## Back-end Developer (freelance)

After eight years working on projects related to digital HW design, I took the decision to steer my professional career towards SW development. The primary motivations behind this strategic shift were twofold:

- I no longer found the same fulfilment in working with FPGAs as I did previously, as I was unable to identify projects that offered a stimulating challenge. FPGA designs are costly, and companies are prioritising integration over innovation, which does not align with my interests.
- Working conditions in the SW programming sector are superior. Upon my return to Spain, I realised that I'd had to lower my expectations compared to salaries/conditions found in other European countries. However, I observed that this is no longer the case for software developers. Companies have to compete against other companies for employees in a global market, thanks to remote-working. So they end offering better conditions to SW guys because they can accept positions from abroad. This is not happening in the digital design. Remote work is a chimera, and local companies don't have to compete with their European counterparts, despite living expenses in Spain being comparable (or even higher). Historically, living costs were lower in Spain, but living in cities such as Madrid or Barcelona compared is getting more expensive than abroad, whilst the salaries are kept lower.

I have been interested in the Rust programming language a few years ago, and this was the best chance I would have to steer my career towards it. So I improved my SW programming skill-set, and started to develop a few projects as freelance.

**My focus is finance and back-end services.** You may find all my projects in my [GitHub](https://github.com/felipet/) page, but I'd highlight these ones:

- [IbexShortBot](https://felipe.nubecita.eu/projects/shortbot/): A Telegram bot written in Rust that simplifies monitoring short positions against companies of the Ibex35.
- [La Coctelera](https://felipe.nubecita.eu/projects/lacoctelera/): A back-end service written in Rust that provides a collaborative open data base for cocktails.
- [Mailjet Client](https://crates.io/crates/mailjet_client): A client for sending mails using Mailjet's API written in Rust.

    January, 2024 up to the present

## System Administrator at Nubecita

I maintain a web server that I use to host websites for artists and other people interested on having a personal web site. I also offer data backup services, photo galleries (Piwigo), a private VPNs, and host my own services such as the IbexShortBot or La Coctelera.

    November, 2023 up to the present

## RTL Engineer at [CLUE Technologies](https://www.clue.aero/)

At Clue Technologies, I was part of the RTL team as head of the Xilinx-based developments. I played the role of
technical lead of a task force for the design and development of one of the in-house boards, which was based on a
Zynq UltraScale+.

The most valuable experience that I gained during my stay at Clue was how to apply the quality assurance guidelines, specially the DO0254 (Airborne Electronic Hardware) to my developments, and how many of my previous development flows could be improved by that.

Besides that, I would also remark the following:

- Design and development of SW/RTL tests for in-house PCBs.
- Definition of requirements.
- Generation of documentation.
- Design, development and test of RTL code.
- HW debugging in the laboratory.
- Maintenance and development of helper SW tools for the automatization of the FPGA development workflow.
- Integration of our development workflow in a CI system based on Gitlab.
- Mentoring of junior colleagues.

My most remarkable achievements were:

- Design and implementation of a bring-up FPGA architecture for testing a new in-house board based on a Zynq
  US+.
- Improve the organization, communication and goal definition for the task force that I was leading.

		July, 2022 to October, 2023


## Embedded Engineer at the European Spallation Source

{{< figure style="width:45%; border-radius:5%; display:block; margin-left: auto; margin-right: auto;" src="/img/ess_hw_show.jpg" alt="profile picture" position="center" >}}

At ESS, I was part of the Hardware & Integration Group for the Integrated Control System division. My scope of work was split in three different areas:

- Development & support of the ESS's fast acquisition platform based on MicroTCA and IOxOS Tosca framework.
- Head of the development and support of the base MicroTCA hardware platform for delivering to system owners in the accelerator.
- Management of the Estonian in-kind contribution to the ESS.

**What I achieved:**

- I improved the reliability of the IOxOS platform and helped our stakeholders using the platform for their projects.
- I designed and implemented a system for a fast deployment & test of MicroTCA systems.
- I highly improved the overall quality of the Estonian in-kind contribution and achieved the delivery of a useful
  standalone system that targeted the gap between the slow and the fast control system.
- I made the integration and further development of the open MRF IP core for the delivered system from Estonia.

**Most remarkable lessons learnt:**

- I had the opportunity to lead an international team within the scope of the Estonian in-kind contribution to the
  project. Certainly, this was something out of my comfort zone, but I'm quite satisfied with the overall result, and I'm glad I could lead the project from a difficult situation to a successful closing with all the final deliverables.
- I strongly developed my leader skills, and learnt many different ways to reach agreements even under high
  presure.
- I really enjoyed being part of such a big science project, in which I could learn a lot of aspects of the physics
  behind a particle accelerator, or its control and timing system.
- I gained a lot of experience on acquisition systems based on FPGAs, the microTCA technology and the MRF
  timing system.

**Link to open-source developed projects:**

- https://github.com/felipet/ess-gendev-tools
- https://github.com/icshwi/ess-openevr
- https://github.com/icshwi/mch_config
- https://github.com/felipet/picoEVR



    	September, 2018 to September, 2021

## Ph.D. Student at the University of Granada

I joined the timing group at the University of Granada as a result of my interest in the White Rabbit (WR) technology. I strived to increase the number of devices that could be fully synchronized (accuracy below 1 ns) in a daisy-chain network of WR devices.

**During my stay, I developed the following skills:**

- Increase my knowledge of the PTP protocol, White Rabbit and synchronization networks in general.
- Learn about the characterization of the noise sources of an electronic device and its contribution to the
  performance of the system. In particular, I used phase noise measurements, and the Allan Deviation (and
  variants) statistics.
- Developed my knowledge in C programming for embedded devices, sw/hw partitioning, Xilinx's SoC platform,
  VHDL.
- Use of laboratory equipment such as DSOs, noise analysers, signal generators, and so on.
- Learn about control loops for systems VCXO, PLL and DAC components.
- Established links with other international labs.

**My achievements:**

- I optimized the control loop of a WR device to achieve up to 22 devices fully connected and synchronized in a
  row (previously, no more than 10-12 was possible).
- I defined a model to find the maximum number of nodes that could be connected in a row (when using my
  previous results). The result was about 700 nodes.
- I defined a series of changes to the firmware of the studied device to improve the accuracy of the
  synchronisation for long chains of devices.
- Together with my workmates, I achieved the publication of several scientific papers in high impact journals.

**Publications:**

- F. Torres-González, J. Díaz, E. Marín-López and R. Rodriguez-Gómez, "Scalability analysis of the white-rabbit
  technology for cascade-chain networks," 2016 IEEE International Symposium on Precision Clock Synchronization for Measurement, Control, and Communication (ISPCS), 2016, pp. 1-6.
- F. Girela-López, F. Torres-González and J. Díaz, "Ethernet time-transfer based on low frequency white rabbit
  solution," 2017 Joint Conference of the European Frequency and Time Forum and IEEE International Frequency Control Symposium (EFTF/IFCS), 2017, pp. 186-189.
- F. Girela-López, F. Torres-González and J. Díaz, "Ultra-accurate Ethernet time-transfer with programmable
  carrier-frequency based on White Rabbit solution," 2017 IEEE International Symposium on Precision Clock
  Synchronization for Measurement, Control, and Communication (ISPCS), 2017, pp. 1-6, doi: 10.1109/ISPCS.
  2017.8056745.
- M. Jiménez-López, F. Torres-González, J. L. Gutiérrez-Rivas, M. Rodríguez-Álvarez and J. Díaz, "A Fully
  Programmable White-Rabbit Node for the SKA Telescope PPS Distribution System," in IEEE Transactions on
  Instrumentation and Measurement, vol. 68, no. 2, pp. 632-641, Feb. 2019.
- J. L. Gutierrez-Rivas, F. Torres-Gonzalez, E. Ros and J. Diaz, "Enhancing White Rabbit Synchronization Stability and Scalability using P2P Transparent and Hybrid Clocks," in IEEE Transactions on Industrial Informatics.


	 	November, 2015 to August, 2018

## Embedded Engineer at [Seven Solutions](http://sevensols.com/)

I was enrolled in the departments of engineering, and production & test of hardware equipment.

**The main skills acquired were:**

- Design and development of hardware tests (custom PCBs, FMC based boards, VME based boards, µTCA based boards) using VHDL, C, Python and Bash.
- Hardware testing and in-house repair.
- Data acquisition software development (C and Python).
- Low-level driver development for the FPGA firmware.
- Hardware development (VHDL) for Xilinx FPGAs and SoCs.

Link to the open-source library developed within the framework of the hardware tests: https://github.com/felipet/py7slib.


	 September,2014 to July, 2016

## Research Fellow (part time) at University of Granada

The main focus of the position was the introduction of synchronization protocols based on Ethernet networks.
The most relevant topics covered were:
- Synchronization protocols (White-Rabbit).
- Embedded system design and development based on Xilinx FPGAs and embedded processors.
- Management and automation of laboratory equipment, such as digital oscilloscopes, time counters, spectrum analyser, etc.

**Achievements:**
- A tool for the auto-calibration of WR devices: https://github.com/felipet/wrcalibration

    September,2014 to April, 2015

## Internship at [Fidesol](https://www.fidesol.org/)

**The main competencies acquired:**

- Embedded OS development (Firefox OS) for the SocamFS project (Linux drivers and kernel modules).
- Web development (Razor Franework and C#) for the Ábaco project.
- Data Base development (TSQL)for the Ábaco project.


		January, 2014 to August,2014



