# La Madriguera · Private

Pack del servidor **bunnydev.zaroz.fun** (Minecraft 1.21.1, NeoForge). Lo instala `LaMadriguera-Instalador` (Windows .exe / Mac .dmg): **baja exactamente lo que hay en este repositorio** (mods, configuración, paquetes de texturas, opciones y servidor), instala la misma versión de NeoForge que el dueño y aplica el perfil elegido. Subir o borrar un archivo aquí lo pone o lo quita en la próxima instalación.

| Archivo | Qué es |
|---|---|
| `mods/` `config/` `resourcepacks/` | el pack tal cual (se copia a `.minecraft`) |
| `options.txt` `servers.dat` | opciones, idioma y el servidor (solo la primera vez: luego son del jugador) |
| `manifest.json` | versión de Minecraft y de NeoForge |
| `1/` `2/` `3/` | los perfiles Potato, Normal y High (`perfil.json` + `config/`) |

El instalador pregunta la RAM, los núcleos y los hilos de tu PC (los rellena solo) y recomienda un perfil: menos de 8 GB o de 4 hilos → **1 Potato**; menos de 16 GB o de 8 hilos → **2 Normal**; si no → **3 High**. Se puede elegir otro. Cambiar de perfil y volver a instalar quita o pone los mods del pack y vuelve a aplicar su configuración (las teclas, el volumen y el idioma no se tocan).

## Comparativa

| | 1 Potato | 2 Normal | 3 High |
|---|---|---|---|
| Mods | 70 de 102 | 102 | 102 |
| RAM para el juego | 3–4 GB | 5–6 GB | 6–8 GB |
| Hilos de Sodium | hilos ÷ 4 (1–2) | hilos ÷ 3 (2–5) | hilos ÷ 2 (2–8) |
| Chunks visibles | 6 | 9 | 12 |
| Chunks simulados | 5 | 6 | 8 |
| Gráficos | rápidos | detallados | detallados |
| Partículas | mínimas | reducidas | todas |
| Nubes | no | rápidas | sí |
| Iluminación suave | no | sí | sí |
| Mezcla de biomas | 0 | 1 | 2 |
| Mipmaps | 0 | 2 | 4 |
| Sombras de entidades | no | sí | sí |
| Distancia de entidades | 0.5 | 0.75 | 1.0 |
| VSync | no | sí | sí |
| FPS máx. (260 = sin límite) | 60 | 120 | 260 |
| Prioridad de chunks | 0 | 0 | 1 |
| Desenfoque de menús | 0 | 3 | 5 |
| Balanceo de cámara | no | sí | sí |

## Carpeta `1` · Potato

Solo los mods necesarios para entrar y los de rendimiento; sin animaciones, partículas ni capas.

- `perfil.json`: claves de `options.txt` de la tabla, RAM 3–4 GB (unos 3/8 de la RAM del PC, dejando 2 GB al sistema; se escribe en el perfil de NeoForge del launcher oficial) e hilos de construcción de chunks de Sodium.
- `config/`: `sodium-options.json`.
- Mods que **no** instala (estéticos u opcionales, solo de cliente):

  - `Chest-Preview-NeoForge-1.21.1-1.0.0.jar`
  - `F1CinematicModes-NeoForge-1.21.1-1.1.6.jar`
  - `InventoryParticles-3.2.0+1.21.1+neoforge.jar`
  - `LegendaryTooltips-1.21.1-neoforge-1.5.5.jar`
  - `MossyLib-1.6.0+1.21.1+neoforge.jar`
  - `Prism-1.21.1-neoforge-1.0.11.jar`
  - `Resourcify (1.21.1-neoforge)-1.8.7.jar`
  - `SubtleEffects-neoforge-1.21.1-1.15.1.jar`
  - `block-dithering-1.0.6+1.21.1+neoforge.jar`
  - `diorama-0.5.0+neoforge-1.21.1.jar`
  - `emf_compat_better_combat_neoforge_1.21.1_2.1.1.jar`
  - `emf_compat_carry_on_neoforge_1.21.1_2.1.1.jar`
  - `emf_compat_core_neoforge_1.21.1_2.3.2.jar`
  - `emf_compat_gliders_1.21.1_2.0.0.jar`
  - `entity_model_features-3.3.12-1.21-neoforge.jar`
  - `entity_texture_features-7.2.6-1.21-neoforge.jar`
  - `fzzy_config-0.7.7+fix1+1.21+neoforge.jar`
  - `kotlinforforge-5.12.0-all.jar`
  - `loot_journal-neoforge-1.21.1-6.2.2.jar`
  - `mru-1.0.41+1.21.1-neoforge.jar`
  - `optifinecapes-1.0.1.jar`
  - `punchy-2.8g-neoforge-1.21.1.jar`
  - `rrls-5.0.11+mc1.21.1-forge.jar`
  - `skinlayers3d-neoforge-1.11.4-mc1.21.1.jar`
  - `sodiumdynamiclights-neoforge-1.0.10-1.21.1.jar`
  - `sounds-2.4.22+lts+1.21.1-neoforge.jar`
  - `studious-keybinds-neoforge-1.21.1-1.0.8-beta.1.jar`
  - `touch_n_motion_neoforge_1.21.1_1.0.4.jar`
  - `visuality-forge-3.0.0.jar`
  - `waveycapes-neoforge-1.11.3-mc1.21.1.jar`
  - `yet_another_config_lib_v3-3.8.2+1.21.1-neoforge.jar`
  - `zoomify-neoforge-1.5.0.jar`

## Carpeta `2` · Normal

Todos los mods, con los efectos más pesados rebajados.

- `perfil.json`: claves de `options.txt` de la tabla, RAM 5–6 GB (unos 3/8 de la RAM del PC, dejando 2 GB al sistema; se escribe en el perfil de NeoForge del launcher oficial) e hilos de construcción de chunks de Sodium.
- `config/`: `sodium-options.json`, `sodiumdynamiclights-client.toml`, `subtle_effects/general.toml`, `subtle_effects/environment.toml`, `subtle_effects/blocks.toml`, `visuality/config.toml`, `skinlayers.json`.

## Carpeta `3` · High

Todos los mods al máximo y 12 chunks; la RAM se ajusta a la de tu PC.

- `perfil.json`: claves de `options.txt` de la tabla, RAM 6–8 GB (unos 3/8 de la RAM del PC, dejando 2 GB al sistema; se escribe en el perfil de NeoForge del launcher oficial) e hilos de construcción de chunks de Sodium.
- `config/`: `sodium-options.json`, `sodiumdynamiclights-client.toml`, `subtle_effects/general.toml`, `subtle_effects/environment.toml`, `subtle_effects/blocks.toml`, `visuality/config.toml`, `skinlayers.json`.

Los mods de rendimiento (Sodium, Sodium Extra, Reese's Sodium Options, FerriteCore, ModernFix, ImmediatelyFast, Entity Culling, Dynamic FPS) van en los tres perfiles.
