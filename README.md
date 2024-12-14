<h1 align="center">
  <br>
    <img src="pict/logo.png" alt="logo" width="200">
</h1>

# Dynamic Routing 
Welcome to the Dynamic Routing Repository. This documentation will guide you through understanding and setting up Dynamic Routing on your computer. You will receive all the necessary knowledge and tools from this comprehensive guide.

## Table of Contents
1. [Configuration](#configuration)
2. [Prerequisites](#prerequisites)
3. [Your Steps](#steps)

# Configuration
<h1 align="center">
  <br>
    <img src="pict/configuration.png" alt="configuration" width="1000">
</h1>

# Prerequisites
Before you proceed with the steps, make sure you have the following prerequisites:

1. **Ubuntu**: If you are using Windows, you can download Ubuntu from:
    [Ubuntu](https://ubuntu.com/desktop/wsl)

2. **Mininet**: Download Mininet from:
    [Mininet](https://mininet.org/)

3. Navigate to the Mininet directory:

    ```bash
    cd mininet
    ```

4. Install all Mininet companions by running the following command:

    ```bash
    mininet/util/install.sh
    ```

5. Once the installation is complete, you can proceed to the next steps.

# Steps
Follow the steps below to get the system up and running on your computer:

1. Clone the repository:

    ```bash
    git clone https://github.com/TeamXNetRouter/JKL-DynamicRouting.git
    ```

2. Navigate to the project directory:

    ```bash
    cd dynamic-routing
    ```

3. Run the project with the following command:

    ```bash
    sudo python3 dynamic_routing.py -c frr-config
    ```

4. To test the setup, you can use the following command in the terminal:

    ```bash
    h1 traceroute -I h2
    ```

5. If you are down line r1 to r2 with this command, you can still traceroute it:

    ```bash
    link r1 r2 down
    h1 traceroute -I h2
    ```
---