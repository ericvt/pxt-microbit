# Received Serial number

Reads the serial number contained in the last packet read by ``radio.receiveNumber``, if available.

```sig
radio.receivedSerialNumber();
```

### Returns

* a [number](/reference/types/number) that represents the serial number of the sending device.

### Simulator

This function only works on the micro:bit, not in browsers.

### Example

By default, the serial number is not transmitted. The sender must first use ``radio.setTransmitSerialNumber`` to enable this feature.

The micro:bit sends a random number when button A is pressed. When receiving a number, the serial number is displayed.

```blocks
radio.setTransmitSerialNumber(true);
radio.onDataReceived(() => {
    radio.receiveNumber();
    basic.showNumber(radio.receivedSerialNumber());
})
input.onButtonPressed(Button.A, () => {
    radio.sendNumber(Math.random(10));
})
```

### See also

[receive number](/reference/radio/receive-number), [send number](/reference/radio/send-number), [on data received](/reference/radio/on-data-received),
[radio](/reference/radio/set-transmit-serial-number)

```package
microbit-radio
```