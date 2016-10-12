# Received Name

Reads the name of the value in the last packet read by ``radio.receiveNumber``. The time stamp represents the running time of the sending device when the packet was sent.

```sig
radio.receivedTime();
```

### Returns

* a [number](/reference/types/number) that represents the running time (ms) of the sending device when the packet was sent.

### Simulator

This function only works on the micro:bit, not in browsers.

### Example

The micro:bit sends a random number when button A is pressed. When receiving a number, the time is displayed.

```blocks
radio.onDataReceived(() => {
    radio.receiveNumber();
    basic.showString(radio.receivedName());
})
input.onButtonPressed(Button.A, () => {
    radio.sendValue("dice", Math.random(10));
})
```

### See also

[receive number](/reference/radio/receive-number), [send number](/reference/radio/send-number), [on data received](/reference/radio/on-data-received)

```package
microbit-radio
```