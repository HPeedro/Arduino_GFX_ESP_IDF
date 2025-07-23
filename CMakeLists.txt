set(COMPONENT_SRCDIRS "src")
set(COMPONENT_ADD_INCLUDEDIRS "src")

file(GLOB_RECURSE GFX_SRC
    "src/*.cpp"
)

idf_component_register(
    SRCS ${GFX_SRC}
    INCLUDE_DIRS "src"
    REQUIRES arduino-esp32 esp_lcd esp_mm
)