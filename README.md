EasyMonero-PHP
===============

A simple class for making calls to Monero's daemon JSON-RPC API using PHP.

Getting Started
---------------
1. Include easymonero.php into your PHP script:

    ```php
    require_once('easymonero.php');
    ```
2. Initialize Monerod connection/object:

    ```php
    $monero = new Monero();
    ```

    Optionally, you can specify a host and port. Defaults are 127.0.0.1 and port 18081.

    ```php
    $monero = new Monero('12.34.56.78','9999');
    ```

3. Make calls to monerod as methods for your object. Examples:

    ```php
    $monero->is_ready();
    
    $monero->getblockcount();
    
    $monero->get_block_header_by_height(1);
    ```
