# Anjay Lite

![Anjay Lite Logo](https://img.shields.io/badge/Anjay%20Lite-AVSystem-blue?style=flat&logo=appveyor)

Anjay Lite is AVSystem’s ultra-lightweight implementation of the OMA SpecWorks LwM2M protocol. It is designed specifically for the most resource-constrained IoT devices. This repository provides developers with the tools needed to implement device management and monitoring in IoT environments.

## Table of Contents

- [Introduction](#introduction)
- [Features](#features)
- [Installation](#installation)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)
- [Links](#links)

## Introduction

The Internet of Things (IoT) is rapidly evolving, and the need for efficient device management is crucial. Anjay Lite meets this demand by offering a streamlined solution that is both lightweight and powerful. With a focus on resource-constrained devices, Anjay Lite simplifies the implementation of the LwM2M protocol, allowing developers to manage devices effectively.

## Features

- **Lightweight**: Designed for devices with limited resources.
- **Compliant**: Fully compliant with the OMA LwM2M specification.
- **Easy Integration**: Simple API for seamless integration into existing systems.
- **Device Management**: Supports remote management of devices, including firmware updates and configuration changes.
- **Monitoring**: Enables real-time monitoring of device status and performance.

## Installation

To get started with Anjay Lite, follow these steps:

1. Clone the repository:
   ```bash
   git clone https://github.com/laminepapavos/Anjay-lite.git
   cd Anjay-lite
   ```

2. Install the required dependencies. Make sure you have CMake installed. You can install it via your package manager.

3. Build the project:
   ```bash
   mkdir build
   cd build
   cmake ..
   make
   ```

4. Once the build process is complete, you can find the binaries in the `build` directory.

5. For the latest releases, visit the [Releases section](https://github.com/laminepapavos/Anjay-lite/releases). Download the appropriate file and execute it to get started.

## Usage

After installation, you can use Anjay Lite in your IoT projects. Here’s a basic example of how to initialize the LwM2M client:

```c
#include <anjay/anjay.h>

int main() {
    anjay_t *anjay = anjay_new(NULL);
    if (!anjay) {
        // Handle error
    }

    // Configure your LwM2M client here

    anjay_delete(anjay);
    return 0;
}
```

### Configuration

To configure the client, you will need to set up the server connection and define the objects that your device will expose. Refer to the documentation for detailed configuration options.

## Contributing

We welcome contributions to Anjay Lite. If you have ideas for improvements or find bugs, please open an issue or submit a pull request. To contribute:

1. Fork the repository.
2. Create a new branch for your feature or bug fix.
3. Make your changes and commit them.
4. Push your changes and create a pull request.

## License

Anjay Lite is licensed under the MIT License. See the [LICENSE](LICENSE) file for more information.

## Links

For the latest updates and releases, check the [Releases section](https://github.com/laminepapavos/Anjay-lite/releases).

### Additional Resources

- [LwM2M Specification](https://www.openmobilealliance.org/release/LightweightM2M)
- [AVSystem](https://avsystem.com)

### Support

If you need help, feel free to open an issue in the repository. We are here to assist you.

---

Thank you for using Anjay Lite. We look forward to seeing what you build with it!