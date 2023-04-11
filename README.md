# Polybar Icons font set
Icons fonts for polybar status; battery, wifi and volume

**Notes**: This is not limited to Polybar only, And it does not include config.

## Included Fonts
- Material Design Icons (Pictogrammers) [Github](https://github.com/Templarian/MaterialDesign) [Website](https://pictogrammers.com/library/mdi/)
- Ionicons [Github](https://github.com/ionic-team/ionicons) [Website](https://ionic.io/ionicons/)
- Boxicons [Github](https://github.com/atisawd/boxicons) [Website](https://boxicons.com/)

## LICENSE
| Fonts                                 | LICENSE                    |
|---------------------------------------|----------------------------|
| Material Design Icons (Pictogrammers) | Pictogrammers Free License |
| Ionicons                              | MIT                        |
| Boxicons                              | MIT                        |

### Usage

Charging and discharging use same codepoints

**Example config for polybar**

 - font-1 is Battery-Charge
 - font-2 is Battery-Discharge

```ini
format-charging = %{T2}<ramp-capacity>%{T-} <label-charging>
format-discharging = %{T3}<ramp-capacity>%{T3} <label-discharging>
```
