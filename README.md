# Corne 5-Column ZMK Config

Personal ZMK firmware configuration for a 36-key Corne split keyboard.

## Hardware

| Component | Detail |
|-----------|--------|
| PCB | Corne 5-column from [Typeractive](https://typeractive.xyz) |
| Controller | nice!nano v2 |
| Switches | Kailh Choc Pro Red |

## Keymap

Miryoku-inspired layout with 6 layers. Layers are accessed via hold on the thumb keys.

### Base

```
┌─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┐
│  Q  │  W  │  E  │  R  │  T  │   │  Y  │  U  │  I  │  O  │  P  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│GUI/A│ALT/S│CTL/D│SFT/F│  G  │   │  H  │SFT/J│CTL/K│ALT/L│GUI/'│
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│  Z  │  X  │  C  │  V  │  B  │   │  N  │  M  │  ,  │  .  │ /`  │
└─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┘
            │NAV/ │NUM/ │SYM/ │   │     │FUN/ │MED/ │
            │ DEL │ BSP │ ENT │   │ TAB │ SPC │ ESC │
            └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

- Home row mods: GUI, Alt, Ctrl, Shift (mirrored on both halves)
- Bottom-right key (`/``) is a mod-morph: `/` normally, `` ` `` with GUI held (for macOS Cmd+` window cycling)

### Num (hold left middle thumb)

```
┌─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┐
│     │     │     │     │     │   │  [  │  7  │  8  │  9  │  ]  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ GUI │ ALT │ CTL │ SFT │     │   │  =  │  4  │  5  │  6  │  ;  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │   │  \  │  1  │  2  │  3  │  `  │
└─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┘
            │     │ --- │     │   │  -  │  0  │  .  │
            └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Symbol (hold left inner thumb)

```
┌─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┐
│     │     │     │     │     │   │  {  │  &  │  *  │  (  │  }  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ GUI │ ALT │ CTL │ SFT │     │   │  +  │  $  │  %  │  ^  │  :  │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │   │  |  │  !  │  @  │  #  │  ~  │
└─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┘
            │     │     │ --- │   │  _  │  (  │  )  │
            └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Function (hold right middle thumb)

```
┌─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┐
│ Mic │     │     │     │Claude│   │PrtSc│ F7  │ F8  │ F9  │ F12 │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ GUI │ ALT │ CTL │ SFT │     │   │ScrLk│ F4  │ F5  │ F6  │ F11 │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │   │Pause│ F1  │ F2  │ F3  │ F10 │
└─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┘
            │     │     │     │   │     │ --- │     │
            └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Media (hold right inner thumb)

```
┌─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┐
│     │     │ V+  │     │     │   │     │     │     │     │     │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│     │ Prv │ V-  │ Nxt │BTCLR│   │     │ SFT │ CTL │ ALT │ GUI │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│BT 0 │BT 1 │BT 2 │BT 3 │BTCLR│   │     │     │     │     │     │
└─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┘
            │Mute │Play │Stop │   │     │     │ --- │
            └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

### Navigation (hold left outer thumb)

```
┌─────┬─────┬─────┬─────┬─────┐   ┌─────┬─────┬─────┬─────┬─────┐
│     │     │     │     │     │   │S+Tab│PgDn │PgUp │ Tab │     │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│ GUI │ ALT │ CTL │ SFT │     │   │  <  │  v  │  ^  │  >  │     │
├─────┼─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┼─────┤
│     │     │     │     │     │   │Caps │ End │Home │     │     │
└─────┴─────┼─────┼─────┼─────┤   ├─────┼─────┼─────┼─────┴─────┘
            │ --- │     │     │   │     │     │     │
            └─────┴─────┴─────┘   └─────┴─────┴─────┘
```

## Home Row Mods

Two custom hold-tap behaviors to reduce misfires:

| Behavior | Used for | Flavor | Tapping term | Prior idle |
|----------|----------|--------|-------------|------------|
| `LHRM` / `RHRM` | GUI, Alt, Ctrl | tap-preferred | 280ms | 150ms |
| `LShiftMT` / `RShiftMT` | Shift | balanced | 175ms | 100ms |

Both use positional hold triggers (opposite-hand activation only) and `hold-trigger-on-release`.

## Configuration

| Setting | Value |
|---------|-------|
| Debounce (press / release) | 5ms / 5ms |
| Bluetooth TX power | +8 dBm |
| Deep sleep | Enabled (15 min timeout) |

## Building

Firmware builds automatically via GitHub Actions on push. Download the artifacts from the Actions tab and flash to each half.
