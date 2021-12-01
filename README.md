# DRAFT: ArcOS
An Operating System to be built from the ground up with RISC V hardware.

## Design
- Novusk - The base 'hypervisor' containing code for bare metal execution, drivers, bootloaders, block devices. No filesystems, scheduling, etc. A bare metal hypervisor that runs multiple VMs.
- Ardaku - A unikernel system to link to and run on novusk. Sandboxed environment for apps to run without a user/kernel divide. Executes virtual code that gets converted to code on Novusk/RV.
- Carbon - The software suite

## Style & Layout
- Submodules for major things
- Be as clear as possible, add a 'doc' file to each dir to describe its contents. LATER: use a doc generator to compile html
- Keep it simple, stupid and It Just Works

