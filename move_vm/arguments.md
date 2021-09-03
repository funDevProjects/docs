# Arguments

The main function of the script can have arguments and will be executed when you send a transaction with your script.

With `dove tx` command you can pass arguments to script function and build it, see help:

```text
dove tx --help
```

Calling the main function, developers can pass arguments, example: 

```text
dove tx 'my_script<0x1::PONT::PONT>(1, [1, 2, 3], 1exaAg2VJRQbyUBAeXcktChCAqjVP9TUxF3zo23R2T6EGdE, false)'
```

The command compiles both script file and adds arguments into one file with `*.mvt` extension. The file could be used to send `execute` (script one) transaction to the network.

From example you can see that dove **"tx"** command supports different kind of arguments, as:

* Numbers (u8, u64, u128)
* Boolean
* Addresses
* Vectors
* Type parameters (generics).
