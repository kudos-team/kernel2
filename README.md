# KudOS Kernel2
The second coming of the kernel bcos why not

## Setup
Run the following to install important things:

```
cargo install bootimage
```

Also for running and testing ensure you have Qemu installed.

## Doing stuff with the code
### Running in Qemu
```bash
cargo run
```

### Building
```bash
cargo bootimage
```

#### Building for a USB
```bash
cargo bootimage
dd if=target/x86_64-kudos/debug/bootimage-kudos.bin of=/dev/sdX && sync
```

(Replace `sdX` with the name fo your usb)
**This will overwrite anything already on that usb**
