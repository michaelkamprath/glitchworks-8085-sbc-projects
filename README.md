Software written for the [Glitch Works 8085 SBC rev 4 Mini](https://www.tindie.com/products/glitchwrks/glitch-works-8085-sbc-rev-4-mini/)

## Software Compiling
Compile with [BespokeASM](https://github.com/michaelkamprath/bespokeasm):

```sh
bespokeasm compile -c bespokeasm/glitchworks-8085-sbc.yaml -I common -n -p -t intel_hex hello-world.gw85
```

Load generated Intel hex in GW-MON with `L` command. Note that your serial client should have character pacing of at least 3 ms so as to not send faster than the SBC can handle.

## References
* [GWMON-80 code](https://github.com/glitchwrks/gwmon-80)
* [Glitch Works 8085 SBC Rev 4 Mini manual](https://filedump.glitchwrks.com/projects/gw-8085sbc-4m/GW-8085SBC-4M_MANUAL.pdf)
* [Glitch Works 8085 SBC Rev 4 Mini schematic](https://filedump.glitchwrks.com/projects/gw-8085sbc-4m/GW-8085SBC-4M_SCHEMATIC.pdf)
