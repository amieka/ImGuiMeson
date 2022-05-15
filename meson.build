project('guidemo', 'cpp', 'objcpp')
add_project_arguments('-std=gnu++14', language : 'objcpp')

compiler_settings = environment()
compiler_settings.set('CC', 'clang')
compiler_settings.set('CXX', 'clang++')
meson.add_devenv(compiler_settings)

sources = ['imgui_demo.cpp', 'imgui_draw.cpp', 'imgui_tables.cpp', 'imgui_widgets.cpp', 'imgui.cpp', 'main.mm', 'imgui_impl_metal.mm', 'imgui_impl_osx.mm']
sdl2_dep = dependency('sdl2')
dep_main = dependency('appleframeworks', modules : ['Foundation', 'AppKit', 'MetalKit', 'Metal', 'GameController','QuartzCore'])

executable('demo', sources:sources,dependencies:[dep_main,sdl2_dep])