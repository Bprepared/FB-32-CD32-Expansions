#FB-32R CD32 Riser Board

Fundamentally, this is a passive board, with 2off 2x40 2mm Female Pin Headers giving 160 of the 182 signals from the CD32's edge connector. I choose to pull as many signals as I could, but drop those that were probably never going to be used i.e. the _EXT Video signals associated with the FMV module, and a few VCC/GNDS.
The female headers were selected as they allowed me to piggy back a second board on the back which will contain the magic, while not exposing pins to potential shorting. They can take 1A of current nicely, and the height of 2mm header male and female together are the same as standard PCB stand offs, so I don't have to rely on the connectors taking all the mechanical strain and abuse loads from plugging/unplugging cables, and I can develop different riser configurations with only needing to solder 160 through-hole pins (worst case) instead of 364!

#Bill of Materials
|Part | Value    | Device  | Package | Description        |
|-----|----------|---------|---------|--------------------|
| J1  | CD32     |5650092-1| MCA-182 | Skt Edge Connector |
| J2  | EXP CARD |5650092-1| MCA-182 | Skt Edge Connector |
| J3  | BUSSES   |Header|2mm Female 2x40|                 |
| J4  | SIGNALS  |Header|2mm Female 2x40|                 |
