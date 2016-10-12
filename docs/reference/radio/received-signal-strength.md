# Received Signal Strength

Find how strong the ``radio`` signal is, from `255` to `0`.
(`255` means a weak signal and `0` means a strong one.)

The micro:bit finds the signal strength by checking how strong it was
the last time it ran the
[receive number](/reference/radio/receive-number) function. That means
it needs to run **receive number** first.

```sig
radio.receivedSignalStrength();
```

### Returns

* a [number](/reference/types/number) between `255` and `0` that means
how strong the signal is.

### Simulator

This function only works on the micro:bit, not in browsers.

### Example

The micro:bit sends the serial number when button A is pressed. When receiving a number, the RSSI is displayed.

```blocks
basic.onDataReceived(() => {
    radio.receiveNumber();
    basic.showNumber(radio.receivedSignalStrength());
});
input.onButtonPressed(Button.A, () => {
    radio.sendNumber(control.deviceSerialNumber());
})
```

### See also

[receive number](/reference/radio/receive-number), [send number](/reference/radio/send-number), [on data received](/reference/radio/on-data-received)

```package
microbit-radio
```