set(SOURCES GUIControlSettings.cpp
            GUIWindowSettings.cpp
            GUIWindowSettingsCategory.cpp
            GUIWindowSettingsScreenCalibration.cpp
            GUIWindowTestPattern.cpp)

core_add_library(settings_windows)
add_dependencies(settings_windows libcpluff)
