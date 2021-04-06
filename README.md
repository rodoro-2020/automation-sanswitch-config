# SANSWITCH 2498 CONFIGURATION


This tool is created to perform the full configuration of the manual to succesfully clean up a sanswitch model 2498 device.

It has been implemented in:
- SANSWITCH 2498 F48
- SANSWITCH 2498 F24
- SANSWITCH 2498 X24

### Requirements

To be able to execute this scripts, you need to first meet this requierements:

- Linux red hat based system
- Expect tool installed
- Connect the switch configuration port to you machine's ethernet port
- Enable an ssh connection to the switch

### Set up

The follow instructions will guide you to perform a correct set up:

- Connect to the targeted switch through serial connection.
- Reset switch passwords and change the IP of the configuration port if necessary.
- Restart the switch, after it is ready again, connect it to your machine and ping.
- Once your machine reaches the switch execute ./sanswitch_1.exp script and the rest sequentially.

Note: The script ./sanswitch_2.exp is still semi-automatic and you will have to follow the instructions from manual.

The actual configuration on the switch is set as follows:
```sh
set ipswitch "10.0.0.10"
set switchname "IBM_2498_X24"
set switchnametest "IBM_2498_X24"
set prompt ":admin>"
set prompt2 ":root>"
set ports 23
```

You may need to change it to the necessary parameters.

Contact Alan.Flores1@ibm.com for support.
