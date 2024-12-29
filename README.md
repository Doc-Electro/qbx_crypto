# qbx_crypto

**Description:**
A simple modification of the standard `qbx_crypto`, allowing players to obtain money from cryptosticks instead of cryptocurrency.

## Table of Contents

- [Overview](#overview)
- [Installation](#installation)
- [Requirements](#requirements)
- [Usage](#usage)
- [Contributing](#contributing)
- [License](#license)

## Overview

`qbx_crypto` is a modified version of the `qbx-crypto` resource for [QBOX-Core] This modification allows players to receive direct cash rewards from cryptosticks, providing an alternative reward structure within the game.

## Installation

1. **Download the ZIP File:**
   Download the latest release as a ZIP file from the [GitHub repository](https://github.com/Doc-Electro/qbx_crypto).

   Alternatively, clone the repository using:
   ```bash
   git clone https://github.com/Doc-Electro/qbx_crypto.git
   ```

2. **Move Files:**
   Extract the ZIP file (or move the cloned folder) to the `resources` directory of your FiveM server.

3. **Add Resource to Server Configuration:**
   Add the following line to your `server.cfg`:
   ```
   ensure qbx_crypto
   ```

4. **Update Database:**
   Import the `qb-crypto.sql` file into your database to add the required tables and data.

## Requirements

- **QBX-Core Framework:** Ensure you have the latest version of [QBX-Core](https://github.com/qbcore-framework/qb-core) installed.
- **mhacking Resource:** This resource requires [mhacking](https://github.com/qbcore-framework/mhacking) for certain functionalities.

## Usage

Once installed, players can use cryptosticks to receive direct cash rewards. The functionality seamlessly integrates with the server's existing economy, offering an alternative way to obtain rewards.

The amount of money obtained from a cryptostick can be customized in the `server/main.lua` file on line 246:
```lua
local Amount = math.random(1000, 5000)
```
Adjust the values in `math.random` to set the minimum and maximum amounts.

## Contributing

Contributions to this project are welcome. Follow these steps to contribute:

1. Fork this repository.
2. Create a new branch for your feature or bug fix:
   ```bash
   git checkout -b feature/new-feature
   ```
3. Commit your changes:
   ```bash
   git commit -m "Add new feature"
   ```
4. Push to the branch:
   ```bash
   git push origin feature/new-feature
   ```
5. Open a Pull Request and describe your changes in detail.

## License

This project is licensed under the GPL-3.0 License. See the [LICENSE](https://github.com/Doc-Electro/qbx_crypto/blob/main/LICENSE) file for more information.

