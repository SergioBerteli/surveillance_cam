set(srcs "connect_wifi.c"
            "main.c")
idf_component_register(SRCS ${srcs}
                        PRIV_INCLUDE_DIRS "."
                        PRIV_REQUIRES nvs_flash
                        REQUIRES esp_http_server esp_timer esp_wifi mqtt)

