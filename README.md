## EPICS-FMR
EPICS support module for the Ferro-Magnetic Resonance equipment. The submodule exists within ISIS, not support as this is an older device.

This is currently an LVDCOM IOC wrapping the users' VI.

### Useful Recources
* [Using LVDCOM](https://github.com/ISISComputingGroup/ibex_developers_manual/wiki/Using-LVDCOM)
* [Ferro Magnetic Resonance Equipment](https://github.com/ISISComputingGroup/ibex_developers_manual/wiki/Ferro-Magnetic_Resonance_equipment)

### Emulator and Tests
Currently the FMR does not have an emulator so the command `make ioctests` will not work. The directory to contain an emulator going forward has been created (`FMR\master\system_tests\lewis_emulators`)

Tests have been migrated from [EPICS-IOC_Test_Framework](https://github.com/ISISComputingGroup/EPICS-IOC_Test_Framework) to `FMR\master\system_tests\tests`.


To run system tests, open an EPICS enviorment and execute the following command:
* `%PYTHON3% %EPICS_ROOT%\support\IocTestFramework\master\run_tests.py --test_and_emulator .\system_tests`

