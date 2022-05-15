project('guidemo', 'cpp', 'objcpp')
add_project_arguments('-std=gnu++14', language : 'objcpp')

compiler_settings = environment()
compiler_settings.set('CC', 'clang')
compiler_settings.set('CXX', 'clang++')
meson.add_devenv(compiler_settings)

sources = ['libs/imgui_demo.cpp', 'libs/imgui_draw.cpp', 'libs/imgui_tables.cpp', 'libs/imgui_widgets.cpp', 'libs/imgui.cpp', 'main.mm', 'libs/imgui_impl_metal.mm', 'libs/imgui_impl_osx.mm']
sdl2_dep = dependency('sdl2')
dep_main = dependency('appleframeworks', modules : ['Foundation', 'AppKit', 'MetalKit', 'Metal', 'GameController','QuartzCore'])

executable('demo', sources:sources,dependencies:[dep_main,sdl2_dep])