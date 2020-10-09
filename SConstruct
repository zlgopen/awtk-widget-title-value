import os
import scripts.app_helper as app

DEPENDS_LIBS = [
  {
    "root" : '../awtk-widget-number-label',
    'static_libs': [],
    'shared_libs': ['number_label']
  }
]

helper = app.Helper(ARGUMENTS)

helper.set_deps(DEPENDS_LIBS)
helper.set_dll_def('src/title_value.def').set_libs(['title_value']).call(DefaultEnvironment)

SConscriptFiles = ['src/SConscript', 'demos/SConscript', 'tests/SConscript']
SConscript(SConscriptFiles)
