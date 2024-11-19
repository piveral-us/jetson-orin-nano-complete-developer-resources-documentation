# Nvidia Jetson Orin Nano Documentation Hub
Complete Developer Resources &amp; The Official Documentation on Nvidia Jetson Orin Nano
![NVIDIA Jetson Orin Nano](https://nvidia-jetson.piveral.com/wp-content/uploads/2024/11/Nvidia_jetson_orin_nano_.jpg "NVIDIA Jetson Orin Nano")

## Why This Hub Exists

Picture this: You're in the middle of an exciting project, everything's flowing perfectly, and suddenly you need to check a specific GPIO pinout or find that one crucial SDK command. Instead of opening multiple tabs and diving into endless documentation searches, imagine having everything at your fingertips - organized, accessible, and ready when you need it.

We've all been there - bouncing between NVIDIA's documentation, GitHub repositories, forum posts, and community guides, trying to piece together the information we need. It's frustrating, time-consuming, and frankly, unnecessary.

Your focus should be on building, creating, and innovating - not hunting down documentation.
Here's the markdown formatted output following the structure and titles from the HTML:

## Official Docs for Orin Nano
**[Jetson Orin Nano Getting Started Guide](https://developer.nvidia.com/embedded/learn/get-started-jetson-orin-nano-devkit)**

Your essential first stop for setting up your Jetson Orin Nano Developer Kit. You’ll find everything needed for initial setup, from unboxing to first boot. The guide walks you through microSD card preparation, system image flashing, and first-time configuration. It clearly identifies all hardware ports and connections on your developer kit, lists what’s included in your box, and what additional components you’ll need to purchase. If you’re just unboxing your Orin Nano or preparing for your purchase, this documentation ensures you’ll have everything ready for a smooth start.


**[Initial Setup Guide](https://www.jetson-ai-lab.com/initial_setup_jon.html)**

A detailed walkthrough that takes you from unboxing to running JetPack 6.0 on your Orin Nano. You’ll find a complete inventory checklist of required components, clear instructions for firmware updates, and step-by-step SD card flashing procedures. The guide is particularly valuable if you have a device manufactured before May 2024, as it includes the critical firmware update process. It also covers both monitor-attached and headless setup options, ensuring you can get started regardless of your preferred configuration method.

**[Jetson Orin Nano Series Pinmux](https://developer.nvidia.com/downloads/jetson-orin-nx-and-orin-nano-series-pinmux-config-template)** [Spreadsheet]

Your go-to resource for planning custom carrier board designs with the Orin Nano module. This interactive spreadsheet helps you configure pin multiplexing without conflicts or errors. When designing your custom hardware, you’ll simply edit the highlighted cells to select pin configurations, and the spreadsheet automatically flags potential issues like duplicate signal assignments or missing configurations. It’s directly linked to the official Orin product datasheet and includes built-in error checking to prevent common design mistakes.

**[Jetson Orin Nano Carrier Board Specification](https://developer.nvidia.com/downloads/assets/embedded/secure/jetson/orin_nano/docs/jetson_orin_nano_devkit_carrier_board_specification_sp.pdf)** [PDF]

Your essential reference for hardware integration and custom development with the Orin Nano carrier board. This comprehensive technical document details every connector, pin assignment, and interface on your developer kit. You’ll find detailed pinouts for all standard connectors (USB, DisplayPort, Ethernet), expansion headers (40-pin GPIO, camera connectors), and power specifications. The document is particularly valuable for hardware engineers designing custom carrier boards or integrating peripherals, as it includes mechanical specifications, power diagrams, and critical implementation notes. Whether you’re connecting cameras, designing add-on boards, or working with power management, this specification ensures you have the precise technical details needed for reliable hardware integration.
 
**[Orin Nano Hardware Specs](https://developer.nvidia.com/embedded/learn/jetson-orin-nano-devkit-user-guide/hardware_spec.html)**

Your comprehensive guide to the physical layout and connectivity options of your Orin Nano Developer Kit. You’ll find detailed information about every port, connector, and expansion option on the board, including precise specifications for the microSD slot, USB ports, display outputs, and camera connections. The documentation is particularly valuable when planning your hardware setup, as it clarifies important details like USB-C limitations (data-only, no display output), power specifications for USB ports (3A per stack), and camera connector requirements.

**[Orin Nano Series Design Guide](https://developer.nvidia.com/downloads/jetson-orin-nx-series-nano-series-design-guide)** [PDF]

The official reference for hardware design aspects when creating custom carrier boards or products using Orin NX/Nano modules. It contains crucial information about signal routing, component selection, and design rules that must be followed to ensure reliable operation. This document is indispensable for engineers working on custom Jetson Orin NX/Nano hardware designs, as it provides the technical specifications needed to properly implement the module interfaces and ensure compatibility.


**[Jetson Orin Nano Series Thermal Design Guide](https://developer.nvidia.com/downloads/jetson-orin-nx-orin-nano-series-thermal-design-guide)** [PDF]

The official guide for thermal design considerations when integrating the Jetson Orin NX or Nano modules into your system. This comprehensive document covers critical thermal specifications, design requirements, and implementation guidelines. You’ll find detailed thermal performance data for different power modes, component placement maps, and specific guidance for heat sink design and mounting. The guide is particularly valuable for hardware engineers and system designers who need to ensure proper thermal management of their Orin-based systems. It includes thermal resistance calculations, temperature limits, fan control algorithms, and detailed mechanical mounting specifications to help you create an effective cooling solution.


**[Jetson Orin Series SoC Technical Reference Manual](https://developer.nvidia.com/downloads/orin-series-soc-technical-reference-manual/)** [PDF]

The official technical guide to the internal architecture and programming of the NVIDIA Orin SoC. This detailed manual covers the logical organization and control of core hardware components, focusing on modules that interface with external devices or control fundamental chip operations. You’ll find essential information about memory architecture, boot processes, CPU complex, GPU architecture, and multimedia subsystems. Each section provides programming guidelines, register descriptions, and functional overviews. This is super helpful when you need to understand low-level hardware details or develop drivers for custom hardware interfacing with your Orin Nano. 


**[Jetson Orin Nano Series Pin and Function Names Guide Application Note](https://developer.nvidia.com/downloads/assets/embedded/secure/jetson/orin_nx/docs/jetson_orin_nx_orin_nano_pin_function_names_guide_da-11434-001_v1.0.pdf)** [PDF]

The official reference guide for understanding pin assignments and signal names across different documentation levels of the Jetson Orin Nano. It helps you trace how pin names and functions are represented from the chip level through to the module and carrier board level. The guide can be helpful when you’re designing custom carrier boards or working with the 40-pin header, as it shows you how the same signals are referenced differently in various technical documents like the datasheet, technical reference manual, and design guides. It includes practical examples of pin mapping and helps resolve any confusion about signal naming conventions across different documentation sources.

### Software and Development
**[Jetpack SDK](https://developer.nvidia.com/embedded/jetpack)**

Your essential software suite for developing on the Jetson Orin Nano. JetPack provides everything you need in one comprehensive package: the operating system (Jetson Linux), AI/ML tools, and development libraries. With JetPack 6.1, you’ll get the latest Ubuntu 22.04-based system with Linux kernel 5.15, along with cutting-edge AI tools like CUDA 12.6, TensorRT 10.3, and cuDNN 9.3. The SDK includes optimized libraries for computer vision, multimedia processing, and GPU computing. You’ll find three installation methods to suit your needs: SD card image flashing, SDK Manager, or Debian package installation.

**[Jetson Linux Driver Package](https://developer.nvidia.com/embedded/jetson-linux-r3541)**

The fundamental building block for creating a customized system on the Jetson Orin Nano. This Board Support Package (BSP) provides everything you need for low-level system development, including the Linux kernel, bootloader, drivers, and Ubuntu-based root filesystem. For the Orin Nano specifically, you’ll find the essential Linux Kernel 5.10, UEFI-based bootloader, and special NVIDIA drivers optimized for the platform. The package is particularly important when you need to customize the operating system, develop kernel modules, or require precise control over system initialization. 

**[Software Setup](https://developer.nvidia.com/embedded/learn/jetson-orin-nano-devkit-user-guide/software_setup.html)**

The official guide for setting up the software on your Jetson Orin Nano. It outlines two main approaches: the straightforward microSD card method and an advanced setup using SDK Manager. For beginners, you’ll find the default microSD card setup process that gets you started quickly by simply flashing an image and powering on. For advanced users, it details the optional SDK Manager workflow that offers more flexibility in choosing storage options (microSD, NVMe SSD, or USB drive) and installing specific JetPack components. The guide includes step-by-step instructions for both methods, including hardware connections, Force Recovery Mode setup, and the complete installation process. Essential for anyone looking to properly configure their Jetson Orin Nano’s software environment, whether for basic development or custom installations.

**[Orin Nano Boot Flow](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/AR/BootArchitecture/JetsonOrinSeriesBootFlow.html)**

The official guide to understanding how your Jetson Orin device boots up from power-on to operating system. This documentation walks you through the complete boot sequence, explaining each critical component’s role and responsibilities. You’ll learn about the BootROM’s initial hardware initialization, the security services provided by PSCROM, MB1’s system configuration tasks, and MB2’s role in flashing and device detection. The guide pays special attention to the UEFI implementation, which replaced CBoot as the CPU bootloader, explaining its standardized interfaces and secure boot mechanisms. For developers working on custom boot solutions or troubleshooting boot issues, you’ll find detailed boot flow diagrams and component interactions that help you understand exactly what happens at each stage of the boot process.

**[Complete list of supported software features](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SO/JetsonOrinSeries.html)**

The official guide guide to all software capabilities available on your Jetson Orin Nano. This documentation covers everything from low-level bootloader operations to high-level system features. You’ll find detailed specifications for hardware interfaces including UART, I2C, SPI, and GPIO configurations. The guide is particularly valuable when you’re working with peripheral connections, as it details supported communication protocols and their specific features. For networking and storage, you’ll find complete information about Ethernet capabilities, PCIe configurations, and supported storage interfaces. Whether you’re developing a computer vision application or setting up a complex I/O system, this document helps you understand exactly what your Orin Nano can do and how to implement each feature correctly.

**[Flashing Support on Nvidia Orin Nano](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/FlashingSupport.html)**

This is the official guide covering all flashing methods and options, with two main tools at your disposal: flash.sh for basic flashing of bootloader and kernel, and l4t_initrd_flash.sh for faster flashing using recovery initial ramdisk. You’ll find detailed instructions for flashing to different storage types – from internal eMMC to external NVMe SSDs and USB drives. The guide is particularly valuable for understanding partition-specific flashing, NFS root setup, and mass flashing multiple devices. For development environments, it includes critical information about bootloader updates, secure boot configurations, and troubleshooting failed updates. 

## Collection of Troubleshooting Guides on Nvidia Orin Nano
**[Check all the Orin Nano Troubleshooting Guides](https://nvidia-jetson.piveral.com/nvidia-jetson-orin-nano/)**

Your comprehensive troubleshooting manual for the Jetson Orin Nano, regularly updated with the latest solutions. When you encounter issues, this collection provides detailed fixes across all major areas of development. You’ll find specific solutions for camera integration challenges, boot problems, flashing procedures, hardware issues, kernel customization, and CUDA development. The guide is particularly valuable for its practical, solution-focused approach, covering everything from basic setup problems to advanced development challenges. Whether you’re debugging camera frame rates, resolving boot loops, or optimizing CUDA applications, you’ll find step-by-step solutions backed by real-world experience. 

### Other Technical Documentation on Orin Nano
- **[Overlay files for new memory support (PCN210100)](https://developer.nvidia.com/downloads/embedded/l4t/r35_release_v4.1/overlay_pcn210361_pcn210100_r35.4.1.tbz2)**
- **[Display Configuration](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/Kernel/DisplayConfigurationAndBringUp/OrinDisplayconfig.html)**
- **[h364 Software Encoding in Orin Nano](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/Multimedia/SoftwareEncodeInOrinNano.html)**
- **[Secure Boot on Orin Nano](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/Security/SecureBoot.html)**
- **[PCIe Endpoint Mode on Orin Nano](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/Communications/PcieEndpointMode.html)**
- **[Power and performance management features](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/SD/PlatformPowerAndPerformance/JetsonOrinNanoSeriesJetsonOrinNxSeriesAndJetsonAgxOrinSeries.html)**
- **[Orin Nano Module adaption/porting guide](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/HR/JetsonModuleAdaptationAndBringUp/JetsonOrinNxNanoSeries.html)**
- **[Board automation and UART debugging usage](https://docs.nvidia.com/jetson/archives/r35.4.1/DeveloperGuide/text/AT/BoardAutomation.html)**
- **[How to Power ON/OFF & Force Recovery Mode](https://developer.nvidia.com/embedded/learn/jetson-orin-nano-devkit-user-guide/howto.html)**
- **[Install Jetson Software with SDK Manager](https://docs.nvidia.com/sdk-manager/install-with-sdkm-jetson/index.html)**
- **[Top level cmake files for Vulkan SC Samples](https://developer.nvidia.com/downloads/embedded/l4t/r35_release_v4.1/vulkan-sc-samples.zip)**
- **[Deepstream_python_apps](https://github.com/NVIDIA-AI-IOT/deepstream_python_apps)**
- **[Jetson Orin Nano Module 3D CAD STEP model](https://developer.nvidia.com/downloads/jetson-orin-nx-series-jetson-orin-nano-module-3d-cad-step-model)**
- **[Jetson Orin Nano Developer Kit 3D CAD STEP model](https://developer.nvidia.com/downloads/assets/embedded/secure/jetson/orin_nano/docs/jetson_orin_nano_devkit_3d_step_model.zip/)**


## Github Repos
AI Vision & Segmentation
- **[NanoSAM](https://github.com/NVIDIA-AI-IOT/nanosam)** – Real-time Segment Anything (SAM) model optimized for NVIDIA Jetson Orin platforms
- **[Hello AI World Demos](https://github.com/dusty-nv/jetson-inference)** – Collection of DNN inference examples and tutorials for Jetson platforms
- **[NanoOWL](https://github.com/NVIDIA-AI-IOT/nanoowl)** – Optimized OWL-ViT implementation for real-time object detection on Jetson Orin

Simulation & Integration
- **[Isaac Sim with Isaac ROS Integration](https://github.com/kabilan2003/NVIDIA-Isaac-Sim-and-Isaac-ROS-Integration-on-Jetson-Orin-Nano)** – Guide for integrating NVIDIA Isaac Sim with Isaac ROS on Jetson Orin Nano

Performance & Optimization
- **[Jetson Benchmark](https://github.com/NVIDIA-AI-IOT/jetson_benchmarks)** – Performance benchmarking tools and results for Jetson platforms
- **[Whisper_trt](https://github.com/NVIDIA-AI-IOT/whisper_trt)** – TensorRT optimization for OpenAI’s Whisper speech recognition model
- **[torch2trt](https://github.com/NVIDIA-AI-IOT/torch2trt)** – PyTorch to TensorRT converter for optimizing deep learning models

## Contacting Nvidia for Technical Support
- **[Live Chat Support](https://nvidia.custhelp.com/app/chat/chat_launch/)** – Direct communication channel with NVIDIA technical support
- **[Orin Nano Discussion Forum](https://forums.developer.nvidia.com/c/agx-autonomous-machines/jetson-embedded-systems/jetson-orin-nano/632)** – Community forum for technical discussions, troubleshooting, and updates
- **[FAQ Page](https://developer.nvidia.com/embedded/faq)** – Comprehensive collection of frequently asked questions and answers about Jetson platforms
