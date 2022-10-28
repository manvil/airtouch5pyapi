# Airtouch 5 Python TCP API
An api allowing control of AC state (temperature, on/off, mode) of an Airtouch 5 controller locally over TCP.

## Warning
I am using this with my own Airtouch 5 and see no issues. Please don't blame me if you have any issues with your Airtouch 5 or AC system after using this - I don't know much about AC systems and will probably not be able to help!
## Usage
To initialise:
`airTouch = AirTouch("192.168.1.19")`

To load:
`await airTouch.UpdateInfo();`

The following functions are available:

Group Level Functions:
`SetGroupToTemperature` (async)
`TurnGroupOn` (async)
`TurnGroupOff` (async)
`SetCoolingModeByGroup` (async)
`SetFanSpeedByGroup` (async)
`GetSupportedCoolingModesByGroup`
`GetSupportedFanSpeedsByGroup`

AC Level Functions
`TurnAcOn` (async)
`TurnAcOff` (async)
`SetFanSpeedForAc` (async)
`SetCoolingModeForAc` (async)
`GetSupportedCoolingModesForAc`
`GetSupportedFanSpeedsForAc`
`GetAcs`

