# Solana Wallet Checker: Track Addresses and Monitor Activity

Need to monitor activity on specific Solana addresses? **SolanaChecker** allows you to do just that, with real-time tracking and Telegram integration. Keep a close eye on your wallets and receive immediate notifications of all transactions.

<p align="left">
    <img src="/asset/trace.webp" />
</p>

## Key Features

1.  **Solana Address Balance Check:** Verify your current Solana balance.

<p align="left">
    <img src="/asset/launch.webp" />
</p>

2.  **Token Security Analysis:** Evaluate token security.

<p align="left">
    <img src="/asset/template.webp" />
</p>

3.  **Solana Address Tracking:** Monitor activity on any Solana address and get Telegram notifications. This is a core function.

4.  **Wallet Data from Mnemonic:** Extract wallet info from a seed phrase.

<p align="left">
    <img src="/asset/header.webp" />
</p>

5.  **Solana Wallet Generation:** Generate new wallets.

<p align="left">
    <img src="/asset/edge.webp" />
</p>

6.  **Brute-Force Wallet Search (with Telegram):** Find wallets with balances.

<p align="left">
    <img src="/asset/paste.webp" />
</p>

## Telegram Setup

Set up Telegram notifications by entering your [bot token](https://core.telegram.org/bots/tutorial#obtain-your-bot-token) and your [chat_id](https://t.me/getmyid_bot) in the 'telegram-settings.txt' file.

## Getting Started

Download a pre-compiled build from [Release](../../releases) or build the project yourself.

## Building the Project

The project is written in C++ and utilizes several libraries. We recommend using **vcpkg** to manage dependencies:

### Installing Dependencies with vcpkg

1.  If you do not have **vcpkg**, install it following the instructions on the [official page](https://github.com/microsoft/vcpkg).
2.  Add the **vcpkg** installation path to your system's PATH.
3.  Run the following commands to install the dependencies:

    -   Install **OpenSSL**:

    ```bash
    vcpkg install openssl
    ```

    -   Install **nlohmann-json**:

    ```bash
    vcpkg install nlohmann-json
    ```

    -   Install **Crypto++**:

    ```bash
    vcpkg install cryptopp
    ```

    -   Install **libsodium**:

    ```bash
    vcpkg install libsodium
    ```

4.  Build the project after installing the dependencies.

### Building with Visual Studio

1.  Open the project solution in Visual Studio.
2.  Ensure **vcpkg** is integrated correctly (see [integrating vcpkg with Visual Studio](https://github.com/microsoft/vcpkg#visual-studio)).
3.  Click **Build** -> **Build Solution**.
4.  Find the executable in the `bin` folder.

### Building with Another C++ Compiler

1.  Ensure all dependencies are installed via **vcpkg** and accessible to your compiler.
2.  Compile the project using the following command (example using g++):

    ```bash
    g++ -o solanachecker main.cpp -lssl -lcrypto -lsodium -lcryptopp -std=c++17
    ```

## Command Line Usage

1.  **-s / -search**: Start a brute-force search to find wallets with a balance.
2.  **-t / -track (ADDRESS)**: Start tracking a specific address.
3.  **-g / -gen (NUMBER)**: Generate the specified number of Solana wallets.
4.  **-m / -mnemonic (MNEMONIC)**: Display information about a wallet.
5.  **-b / -balance (ADDRESS)**: Display the balance.

## Important Notes

-   For research and informational purposes only.
-   Cryptocurrency investments involve risks.

## License

This project is licensed under the [MIT License](/LICENSE).

Update:  16.06.2025 05:31