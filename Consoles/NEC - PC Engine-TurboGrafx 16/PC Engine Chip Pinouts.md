## PC Engine Chip Pinouts

This data was taken from numerous places. Special thanks to the usual PCE crew: Chris Covell, bt garner, Joann, and also to Backup Technik/GameLab magazine, from which I occasionally learned something new.

### Conventions used

Throughout these pages you'll find abbreviations and shorthand terms for a lot of connections. Here's a guide:

| Short | Long          | Short | Long             |
| ----- | ------------- | ----- | ---------------- |
| Dxx   | Data (number) | Axx   | Address (number) |
| /WR   | Write Enable  | /OE   | Output Enable    |
| /CE   | Chip Enable   | NC    | Not Connected    |
| I/O   | Input/Output  | RAxx  | RAM pin#         |

- Misc ICs are the two RAM chips (numbered 1, 2, and 12 for both)

### The NetList

Netlist for each chip.

- [Hu6260](Hu6260.md)
- [Hu6270](Hu6270.md)
- [Hu6280](Hu6280.md)

### Other Notes

With apologies, I've forgotten what a lot of these notes mean. It's been a long time since I made them.

Oct 2009: This is the textual description of the circuitry supplying the 21MHz clock signal to the Hu6280/Hu6260.

Something to do with the clock circuit?

```
Clock -> R163 -> C138 -> R117 -> +5v
      |               +> R118 -> GND
      |               +> Hu6280 10
      |
      +> R164 -> C137 -> R115 -> +5v
		      +> R116 -> GND
		      +> Hu6260 2
```