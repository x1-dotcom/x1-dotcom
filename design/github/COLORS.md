# X1 GitHub Color System

## Canonical palette

| Token | Hex | Role |
|---|---|---|
| X1 Black | `#02060A` | primary background |
| X1 Deep | `#071018` | secondary background |
| X1 Surface | `#0A151F` | cards / panels |
| X1 Border | `#173342` | passive borders |
| X1 Cyan | `#19E8FF` | primary signal |
| X1 Cyan Bright | `#19F6FF` | focal highlights |
| X1 Blue | `#326BFF` | secondary signal |
| X1 Violet | `#7B5CFF` | private/internal accent only |
| X1 Text | `#F4FCFF` | primary text |
| X1 Muted | `#8FB3BF` | secondary text |
| X1 Success | `#27E39B` | verified/healthy state |
| X1 Warning | `#FFC857` | warning state |
| X1 Danger | `#FF5D73` | failure/danger state |

## Usage rules

### Background

Default hero gradient:

`#02060A → #071018 → #02070C`

Avoid light backgrounds in X1-owned hero and system-diagram assets.

### Cyan

Cyan is the X1 identity signal. Use it for:

- primary border highlights
- active signal lines
- key micro-labels
- the `X` / X1 brand mark
- important public/community states

Do not fill every surface with cyan.

### Blue

Electric blue is the secondary system signal. Use it for:

- commercial/private classification
- data paths
- secondary focus states
- gradient transitions from cyan

### Violet

Violet is deliberately scarce. Use it only for:

- internal engineering
- privileged/protected systems
- security authority boundaries

Public community repositories should not become violet-dominant.

## Contrast

Primary text should be near-white, not pure cyan.

Muted text must remain readable against the X1 Deep background. Decorative lines can use lower opacity; explanatory text should not.

## Status semantics

- healthy / verified: green
- attention / pending: amber
- failure / blocked: red
- neutral / inactive: muted blue-grey

Status colors are semantic. Never use red or green as decorative brand accents.
