# Polybar Icons font set
Icons fonts for polybar status; battery, Wi-Fi, Volume, etc.

**Note**: This is not limited to Polybar only, And it does not include config.

## Included Fonts
- Material Design Icons (Pictogrammers) [[GitHub](https://github.com/Templarian/MaterialDesign)] [[Website](https://pictogrammers.com/library/mdi/)]
- Ionicons [[GitHub](https://github.com/ionic-team/ionicons)] [[Website](https://ionic.io/ionicons/)]
- Boxicons [[GitHub](https://github.com/atisawd/boxicons)] [[Website](https://boxicons.com/)]
- Bootstrap [[GitHub](https://github.com/twbs/icons)] [[Website](https://icons.getbootstrap.com/)]

## LICENSE

| Fonts                                 | LICENSE                    |
|---------------------------------------|----------------------------|
| Material Design Icons (Pictogrammers) | Pictogrammers Free License |
| Ionicons                              | MIT                        |
| Boxicons                              | MIT                        |
| Bootstrap                             | MIT                        |

## Details

| Fonts                                 | Icons                      |
|---------------------------------------|----------------------------|
| Material Design Icons (Pictogrammers) | Battery Charge/Discharge   |
| Ionicons                              | Volume                     |
| Boxicons                              | Wi-Fi                      |
| Bootstrap                             | Caps/Nums Lock, Signal     |

## Code points

| Icons                                 | Code points | Point step   |
|---------------------------------------|-------------|--------------|
| Battery Discharge/Charge              | E800 - E900 | +10          |
| Volume                                | E700 - E704 | +1           |
| Wi-Fi                                 | E600 - E604 | +1           |
| Signal                                | E800 - E804 | +1*          |
| Caps Lock                             | E800 - E801 | 0/1          | 
| Nums Lock                             | E802 - E803 | 2/3          |

**Volume code point E704 is muted*

*Keylock are sorted by off/on. Caps Off (E800) Caps On (E801) Nums Off (E802) Nums On (E803).*

*Point step represent iteration of code points such as: E600, E601, E602, E603, E604.

### Usage

Install TTF file to system, then add fonts to config.

Charging and discharging use same unicode code point

**Example config for polybar**

```ini
font-1 = battery\-charge
font-2 =battery\-discharge
...

format-charging = %{T2}<ramp-capacity>%{T-} <label-charging>
format-discharging = %{T3}<ramp-capacity>%{T-} <label-discharging>
```


Icon generated by Fontello [[GitHub](https://github.com/fontello/fontello)] [[Website](https://fontello.com/)]

## Plans
 - [ ] More system icon
 - [ ] Polybar config patch
 - [ ] PKGBUILD for Arch Linux
