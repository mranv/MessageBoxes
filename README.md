
# MessageBoxes

This repository contains implementations of the `MessageBoxA` and `MessageBoxW` functions in Rust, which are part of the Windows API for displaying message boxes. These implementations can be useful in various scenarios, such as debugging applications, displaying prompts, or creating simple user interfaces.

## Tools

### MessageBoxA

This module provides an implementation of the `MessageBoxA` function, which is used to display a message box with an ANSI string as the message text.

### MessageBoxW

This module provides an implementation of the `MessageBoxW` function, which is used to display a message box with a Unicode string as the message text.

## Usage

To use these modules, you can import them into your Rust project and call the respective functions with the appropriate parameters. For example:

```rust
use message_boxes::MessageBoxA;

fn main() {
    let message = "Hello, World!";
    let caption = "Message Box";
    MessageBoxA(None, message, caption, 0);
}
```

This code will display a message box with the text "Hello, World!" and the caption "Message Box".

You can customize the behavior of the message box by passing different flags or options to the function calls. Refer to the Windows API documentation for more information on the available options.

## Building

To build the project, ensure you have Rust and Cargo installed, then run:

```
$ cargo build --release or Use rust.c to compile it for windows.
```

The compiled binaries will be located in the `target/release` directory.

## Contributing

Contributions to this repository are welcome! If you find any issues or have ideas for improvements, please open an issue or submit a pull request.

## Disclaimer

These tools are provided for educational and research purposes only. They should be used only on systems or networks where you have explicit permission to perform security assessments or software development activities. Any unauthorized or unlawful use is strictly prohibited.
