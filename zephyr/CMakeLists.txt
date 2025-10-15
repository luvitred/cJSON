if(CONFIG_CJSON_LIB)
    zephyr_include_directories("${ZEPHYR_CURRENT_MODULE_DIR}")
    zephyr_library()
    zephyr_library_sources(
        "${ZEPHYR_CURRENT_MODULE_DIR}/cJSON.c"
        "${ZEPHYR_CURRENT_MODULE_DIR}/cJSON_Utils.c"
    )
endif()
