+---------------+---------------------------------------+-------------------------------------+
| CPU 最高频率  |            电源管理锁获取情况         | APB 频率和 CPU 频率                 |
|               |                                       |                                     |
+---------------+---------------------------------------+-------------------------------------+
|      240      | 获取 ``ESP_PM_CPU_FREQ_MAX``          | | CPU: 240 MHz                      |
|               |                                       | | APB: 80 Mhz                       |
+               +---------------------------------------+-------------------------------------+
|               | | 获取 ``ESP_PM_APB_FREQ_MAX``,       | | CPU: 80 MHz                       |
|               | | 未获得 ``ESP_PM_CPU_FREQ_MAX``      | | APB: 80 Mhz                       |
+               +---------------------------------------+-------------------------------------+
|               |                  无                   | 使用 :cpp:func:`esp_pm_configure`   |
|               |                                       | 为二者设置最小值                    |
+---------------+---------------------------------------+-------------------------------------+
|      160      | 获取 ``ESP_PM_CPU_FREQ_MAX``          | | CPU: 160 MHz                      |
|               |                                       | | APB: 80 Mhz                       |
+               +---------------------------------------+-------------------------------------+
|               | | 获取 ``ESP_PM_APB_FREQ_MAX``,       | | CPU: 80 MHz                       |
|               | | 未获得 ``ESP_PM_CPU_FREQ_MAX``      | | APB: 80 Mhz                       |
+               +---------------------------------------+-------------------------------------+
|               |                  无                   | 使用 :cpp:func:`esp_pm_configure`   |
|               |                                       | 为二者设置最小值                    |
+---------------+---------------------------------------+-------------------------------------+
|       80      | | 获取  ``ESP_PM_CPU_FREQ_MAX``       | | CPU: 80 MHz                       |
|               | | 或 ``ESP_PM_APB_FREQ_MAX``          | | APB: 80 Mhz                       |
+               +---------------------------------------+-------------------------------------+
|               |                  无                   | 使用 :cpp:func:`esp_pm_configure`   |
|               |                                       | 为二者设置最小值                    |
+---------------+---------------------------------------+-------------------------------------+
