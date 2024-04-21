Attempt to create a generic template to add custom chips to Wokwi from Github.

Example chips:
- [Inverter](https://github.com/wokwi/inverter-chip/blob/3f3c2398313c91552dd2ed51099a085b8453c09f/docs/README.md)
- [PWM](https://github.com/Dlloydev/Wokwi-Chip-PWM)
- [Oscilloscope](https://github.com/Dlloydev/Wokwi-Chip-Scope)
- [st7735](https://github.com/martysweet/st7735-wokwi-chip)

----------


## Usage

To use this chip in your project, include it as a dependency in your `diagram.json` file:

```json
  "dependencies": {
    "chip-scope": "github:Dlloydev/Wokwi-Chip-scope@1.0.7"
  }
```

Then, add the chip to your circuit by adding a `chip-scope` item to the `parts` section of `diagram.json`:

```json
  "parts": {
    ...,
    {
      "type": "chip-scope",
      "id": "scope1",
      "top": -100.0,
      "left": 100.0,
      "attrs": {
      }
    },
```

The actual source code for the chip lives in [src/main.c](https://github.com/Dlloydev/Wokwi-Chip-Scope/blob/main/src/main.c), and the pins are described in [chip.json](https://github.com/Dlloydev/Wokwi-Chip-Scope/blob/main/chip.json).

## Example

[![Wokwi_badge](https://user-images.githubusercontent.com/63488701/212449119-a8510897-c860-4545-8c1a-794169547ba1.svg)](https://wokwi.com/projects/359330496025635841) Graph four analog or digital signals as they vary over time.

## License

This project is licensed under the MIT license. See the [LICENSE](https://github.com/Dlloydev/Wokwi-Chip-Scope/blob/main/LICENSE) file for more details.

