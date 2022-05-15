#### what is this ?
A bare bones Imgui setup on osx using Meson as the build system

#### Notes
- Works ok on Mac. Not tested on other platforms.

#### Setup
- Mac users make sure to install Xcode and that standard compiler toolchain.
- Follow instructions on setting up Meson on your machine (`*nix/mac/win`)
- Install dependencies (`meson wrap install sdl2`). Additional instructions on meson website on using the WrapDB.
- Build : `meson compile -C build/`
- Run : `./build/demo`

#### References
- Meson : `https://mesonbuild.com/`
- ImGui : `https://github.com/ocornut/imgui`