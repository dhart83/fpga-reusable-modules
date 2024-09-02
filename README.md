# FPGA Reusable Modules

## Overview

Welcome to the `fpga-reusable-modules` repository! This repository is a collection of reusable FPGA modules designed to streamline the development process for FPGA projects. Whether you're a professional FPGA developer or an enthusiast, these modules provide a solid foundation for various digital design tasks, allowing you to focus on the unique aspects of your projects.

## Included Modules

This repository contains a variety of FPGA modules that can be reused across different projects. The modules cover a range of functionality, including communication interfaces (e.g., UART, I2C, SPI), clock management (e.g., clock dividers), and other commonly needed digital components.

Each module is self-contained and can be easily integrated into your FPGA designs. Detailed information about each module, including usage instructions, port descriptions, and example code, can be found in the individual `README.md` files located within each module's directory.

## Supported FPGA Platforms

The VHDL code provided in this repository is designed to be vendor-agnostic and should work across most FPGA platforms, including but not limited to:

- **Xilinx** (e.g., Artix-7, Spartan-6)
- **Intel** (formerly Altera)
- **Lattice Semiconductor**
- **Microsemi** (formerly Actel)

### About Constraints Files

While the VHDL modules are platform-independent, some modules may include constraints files (e.g., `.xdc` for Xilinx). These constraints files are specific to the Basys3 board, but they can be adapted for other FPGA platforms as needed. If you are using a different FPGA board, please create or modify the constraints file to suit your specific hardware setup.

## Installation and Usage

To integrate these modules into your FPGA project, follow these steps:

1. **Clone the Repository:**

   ```bash
   git clone https://github.com/dhart83/fpga-reusable-modules.git
   ```

2. **Add the Required Module(s) to Your Project:**

   Navigate to the directory containing the desired module and copy the source files (`.vhdl`, `.vhd`, etc.) to your project’s source directory. Alternatively, you can include the module as a Git submodule:

   ```bash
   git submodule add https://github.com/dhart83/fpga-reusable-modules.git path/to/your_project/module_name
   ```

3. **Include and Instantiate the Module:**

   In your top-level design file, include the module and instantiate it with the appropriate port connections.

4. **Configure Constraints:**

   If using a module with a provided .xdc file (for Basys3), include it in your project to correctly map the signals to your FPGA's I/O pins. For other boards, you'll need to create or adapt a constraints file.

## Licensing

This project is licensed under the MIT License. The MIT License is a permissive license that allows you to freely use, modify, and distribute this code, provided that you include the original copyright notice in any substantial portions of the code.

For more details, see the [LICENSE](LICENSE) file.
