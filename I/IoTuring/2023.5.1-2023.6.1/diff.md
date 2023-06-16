# Comparing `tmp/IoTuring-2023.5.1.tar.gz` & `tmp/IoTuring-2023.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "IoTuring-2023.5.1.tar", last modified: Thu May 18 09:46:45 2023, max compression
+gzip compressed data, was "IoTuring-2023.6.1.tar", last modified: Fri Jun 16 13:06:05 2023, max compression
```

## Comparing `IoTuring-2023.5.1.tar` & `IoTuring-2023.6.1.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.278797 IoTuring-2023.5.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/COPYING
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.258797 IoTuring-2023.5.1/IoTuring/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.262797 IoTuring-2023.5.1/IoTuring/ClassManager/
--rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/ClassManager/ClassManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/ClassManager/EntityClassManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/ClassManager/WarehouseClassManager.py
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/ClassManager/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.262797 IoTuring-2023.5.1/IoTuring/Configurator/
--rw-r--r--   0 runner    (1001) docker     (123)    15985 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Configurator/Configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Configurator/ConfiguratorIO.py
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Configurator/ConfiguratorLoader.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Configurator/MenuPreset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.262797 IoTuring-2023.5.1/IoTuring/Entity/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.258797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.262797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/ActiveWindow/
--rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/AppInfo/
--rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/AppInfo/AppInfo.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Battery/
--rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Battery/Battery.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/BootTime/
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/BootTime/BootTime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Cpu/
--rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Cpu/Cpu.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/DesktopEnvironment/
--rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Disk/
--rw-r--r--   0 runner    (1001) docker     (123)      850 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Disk/Disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/DisplayMode/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/FileSwitch/
--rw-r--r--   0 runner    (1001) docker     (123)     1506 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Hostname/
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Hostname/Hostname.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Lock/
--rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Lock/Lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Monitor/
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Monitor/Monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Notify/
--rw-r--r--   0 runner    (1001) docker     (123)     5589 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Notify/Notify.py
--rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Notify/icon.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/OperatingSystem/
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/OperatingSystem/OperatingSystem.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Power/
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Power/Power.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.266797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Ram/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Ram/Ram.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Temperature/
--rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Temperature/Temperature.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Time/
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Time/Time.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Uptime/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Uptime/Uptime.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Username/
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Username/Username.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Volume/
--rw-r--r--   0 runner    (1001) docker     (123)     2903 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Deployments/Volume/Volume.py
--rw-r--r--   0 runner    (1001) docker     (123)     7256 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/Entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     4821 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/EntityData.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/EntityManager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.258797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Brightness/
--rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Brightness/Brightness.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/CpuTemperature/
--rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Network/
--rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Network/Network.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Screenshot/
--rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/State/
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/State/State.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Terminal/
--rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Terminal/Terminal.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Entity/ValueFormat/
--rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ValueFormat/ValueFormatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Entity/ValueFormat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.270797 IoTuring-2023.5.1/IoTuring/Exceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Exceptions/Exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/Logger/
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Logger/Colors.py
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Logger/LogObject.py
--rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Logger/Logger.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Logger/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/MyApp/
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/MyApp/App.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/MyApp/SystemConsts/
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/MyApp/SystemConsts/DesktopEnvironmentDetection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/MyApp/SystemConsts/OperatingSystemDetection.py
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/MyApp/SystemConsts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/MyApp/SystemConsts/consts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.258797 IoTuring-2023.5.1/IoTuring/Protocols/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/Protocols/MQTTClient/
--rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Protocols/MQTTClient/MQTTClient.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Protocols/MQTTClient/TopicCallback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/Warehouse/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.258797 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/ConsoleWarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)      733 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)    15767 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     1927 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.274797 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/MQTTWarehouse/
--rw-r--r--   0 runner    (1001) docker     (123)     4045 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/Warehouse/Warehouse.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/IoTuring/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 09:46:45.262797 IoTuring-2023.5.1/IoTuring.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    53590 2023-05-18 09:46:45.000000 IoTuring-2023.5.1/IoTuring.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2942 2023-05-18 09:46:45.000000 IoTuring-2023.5.1/IoTuring.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 09:46:45.000000 IoTuring-2023.5.1/IoTuring.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-18 09:46:45.000000 IoTuring-2023.5.1/IoTuring.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-18 09:46:45.000000 IoTuring-2023.5.1/IoTuring.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-18 09:46:45.000000 IoTuring-2023.5.1/IoTuring.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)    53590 2023-05-18 09:46:45.278797 IoTuring-2023.5.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12115 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-05-18 09:46:30.000000 IoTuring-2023.5.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-18 09:46:45.278797 IoTuring-2023.5.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/COPYING
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.653518 IoTuring-2023.6.1/IoTuring/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.653518 IoTuring-2023.6.1/IoTuring/ClassManager/
+-rw-r--r--   0 runner    (1001) docker     (123)     3898 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/ClassManager/ClassManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/ClassManager/EntityClassManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/ClassManager/WarehouseClassManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/ClassManager/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Configurator/
+-rw-r--r--   0 runner    (1001) docker     (123)    15591 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Configurator/Configurator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7558 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Configurator/ConfiguratorIO.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Configurator/ConfiguratorLoader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Configurator/ConfiguratorObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7176 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Configurator/MenuPreset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.649518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/ActiveWindow/
+-rw-r--r--   0 runner    (1001) docker     (123)     3060 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/AppInfo/
+-rw-r--r--   0 runner    (1001) docker     (123)     2920 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/AppInfo/AppInfo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Battery/
+-rw-r--r--   0 runner    (1001) docker     (123)     1338 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Battery/Battery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/BootTime/
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/BootTime/BootTime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Cpu/
+-rw-r--r--   0 runner    (1001) docker     (123)     4285 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Cpu/Cpu.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/DesktopEnvironment/
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Disk/
+-rw-r--r--   0 runner    (1001) docker     (123)      850 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Disk/Disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/DisplayMode/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/FileSwitch/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Hostname/
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Hostname/Hostname.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Lock/
+-rw-r--r--   0 runner    (1001) docker     (123)     1606 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Lock/Lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Monitor/
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Monitor/Monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.657518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Notify/
+-rw-r--r--   0 runner    (1001) docker     (123)     5597 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Notify/Notify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7850 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Notify/icon.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/OperatingSystem/
+-rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/OperatingSystem/OperatingSystem.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Power/
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Power/Power.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Ram/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Ram/Ram.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Temperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     9851 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Temperature/Temperature.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)    13900 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Terminal/Terminal.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Time/
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Time/Time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Uptime/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Uptime/Uptime.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Username/
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Username/Username.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Volume/
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Deployments/Volume/Volume.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/Entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5252 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/EntityData.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/EntityManager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.649518 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Brightness/
+-rw-r--r--   0 runner    (1001) docker     (123)     6486 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Brightness/Brightness.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/CpuTemperature/
+-rw-r--r--   0 runner    (1001) docker     (123)     3342 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Network/
+-rw-r--r--   0 runner    (1001) docker     (123)    11348 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Network/Network.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Screenshot/
+-rw-r--r--   0 runner    (1001) docker     (123)     1629 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/State/
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ToImplement/State/State.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Entity/ValueFormat/
+-rw-r--r--   0 runner    (1001) docker     (123)     5865 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ValueFormat/ValueFormatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Entity/ValueFormat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.661518 IoTuring-2023.6.1/IoTuring/Exceptions/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Exceptions/Exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/Logger/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Logger/Colors.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Logger/LogObject.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7727 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Logger/Logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Logger/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/MyApp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/MyApp/App.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/MyApp/SystemConsts/
+-rw-r--r--   0 runner    (1001) docker     (123)      483 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/MyApp/SystemConsts/DesktopEnvironmentDetection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/MyApp/SystemConsts/OperatingSystemDetection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/MyApp/SystemConsts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/MyApp/SystemConsts/consts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.649518 IoTuring-2023.6.1/IoTuring/Protocols/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/Protocols/MQTTClient/
+-rw-r--r--   0 runner    (1001) docker     (123)     4702 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Protocols/MQTTClient/MQTTClient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Protocols/MQTTClient/TopicCallback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/Warehouse/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.653518 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/ConsoleWarehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)      733 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)    15380 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2387 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/MQTTWarehouse/
+-rw-r--r--   0 runner    (1001) docker     (123)     4058 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/Warehouse/Warehouse.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/IoTuring/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-16 13:06:05.653518 IoTuring-2023.6.1/IoTuring.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    54396 2023-06-16 13:06:05.000000 IoTuring-2023.6.1/IoTuring.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-06-16 13:06:05.000000 IoTuring-2023.6.1/IoTuring.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-16 13:06:05.000000 IoTuring-2023.6.1/IoTuring.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-06-16 13:06:05.000000 IoTuring-2023.6.1/IoTuring.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-06-16 13:06:05.000000 IoTuring-2023.6.1/IoTuring.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-06-16 13:06:05.000000 IoTuring-2023.6.1/IoTuring.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    54396 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    12921 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-16 13:05:48.000000 IoTuring-2023.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-16 13:06:05.665518 IoTuring-2023.6.1/setup.cfg
```

### Comparing `IoTuring-2023.5.1/COPYING` & `IoTuring-2023.6.1/COPYING`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/ClassManager/ClassManager.py` & `IoTuring-2023.6.1/IoTuring/ClassManager/ClassManager.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Configurator/Configurator.py` & `IoTuring-2023.6.1/IoTuring/Configurator/Configurator.py`

 * *Files 1% similar despite different names*

```diff
@@ -260,25 +260,23 @@
 
     def AddActiveEntity(self, entityName, ecm: EntityClassManager):
         """ From entity name, get its class and retrieve the configuration preset, then add to configuration dict """
         entityClass = ecm.GetClassFromName(entityName)
         try:
             preset = entityClass.ConfigurationPreset()
 
-            if preset is not None:  # Then let's configure the Entity
-                # Ask also for Tag if the entity allows multi-instance - multi-instance has sense only if a preset is available 
+            if preset.HasQuestions():
+                # Ask for Tag if the entity allows multi-instance - multi-instance has sense only if a preset is available
                 if entityClass.AllowMultiInstance():
                     preset.AddTagQuestion()
 
                 preset.PrintRules()
-                for index, question in enumerate(preset.ListEntries()):
-                    preset.Question(index)
+                preset.AskQuestions()
 
             else:
-                preset = MenuPreset()  # Use blank
                 print("No configuration needed for this Entity :)")
 
             self.EntityMenuPresetToConfiguration(entityName, preset)
         except Exception as e:
             print("Error during entity preset loading: " + str(e))
 
     def IsEntityActive(self, entityName) -> bool:
@@ -301,24 +299,21 @@
         return False
 
     def AddActiveWarehouse(self, warehouseName, wcm: WarehouseClassManager) -> None:
         """ Add warehouse to the preferences using a menu with the warehouse preset if available """
 
         whClass = wcm.GetClassFromName(warehouseName + "Warehouse")
         try:
-            # With the use of "type" I get the staticmethod of the subclass and not of the parentclass
             preset = whClass.ConfigurationPreset()
 
-            if preset is not None:
+            if preset.HasQuestions():
                 preset.PrintRules()
+                preset.AskQuestions()
 
-                for index, question in enumerate(preset.ListEntries()):
-                    preset.Question(index)
             else:
-                preset = MenuPreset()  # Use blank
                 print("No configuration needed for this Warehouse :)")
 
             # Save added settings
             self.WarehouseMenuPresetToConfiguration(warehouseName, preset)
         except Exception as e:
             print("Error during warehouse preset loading: " + str(e))
```

### Comparing `IoTuring-2023.5.1/IoTuring/Configurator/ConfiguratorIO.py` & `IoTuring-2023.6.1/IoTuring/Configurator/ConfiguratorIO.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Configurator/ConfiguratorLoader.py` & `IoTuring-2023.6.1/IoTuring/Configurator/ConfiguratorLoader.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/AppInfo/AppInfo.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/AppInfo/AppInfo.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Battery/Battery.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Battery/Battery.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Cpu/Cpu.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Cpu/Cpu.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/DesktopEnvironment/DesktopEnvironment.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Disk/Disk.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Disk/Disk.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/DisplayMode/DisplayMode.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/FileSwitch/FileSwitch.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,11 +40,11 @@
     def Update(self):
         self.SetEntitySensorValue(KEY_STATE,
                                   str(Path(self.config_path).exists()))
     
         self.SetEntitySensorExtraAttribute(KEY_STATE, "Path", str(self.config_path))
 
     @classmethod
-    def ConfigurationPreset(self):
+    def ConfigurationPreset(cls) -> MenuPreset:
         preset = MenuPreset()
         preset.AddEntry("Path to file?", CONFIG_KEY_PATH, mandatory=True)
         return preset
```

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Lock/Lock.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Lock/Lock.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Monitor/Monitor.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Monitor/Monitor.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Notify/Notify.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Notify/Notify.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,17 +67,18 @@
         # ! Changing the name we recognize the difference in warehouses only using the name 
         # e.g HomeAssistant warehouse can use the regex syntax with NotifyPaylaod to identify that the component needs the text message
         self.NAME = self.NAME + ("Payload" if self.data_mode == MODE_DATA_VIA_PAYLOAD else "")
 
         self.RegisterEntityCommand(EntityCommand(self, KEY, self.Callback))
 
         # Prepare the notification system
-        if OsD.IsWindows() and not supports_win:
-            raise Exception(
-                'Notify not available, have you installed \'tinyWinToast\' on pip ?')
+        if OsD.IsWindows():
+            if not supports_win:
+                raise Exception(
+                    'Notify not available, have you installed \'tinyWinToast\' on pip ?')
 
         elif OsD.IsLinux() or OsD.IsMacos():
             if not OsD.CommandExists(commands[OsD.GetOs()].split(" ")[0]):            
                 raise Exception(
                     f'Command not found {commands[OsD.GetOs()].split(" ")[0]}!'
                 )  
         else:
@@ -122,13 +123,14 @@
                 .format(self.notification_message,self.notification_title))
 
         else:
             self.Log(self.LOG_WARNING, "No notify command available for this operating system (" +
                      str(OsD.GetOs()) + ")... Aborting")
 
     @classmethod
-    def ConfigurationPreset(self):
+    def ConfigurationPreset(cls) -> MenuPreset:
         preset = MenuPreset()
         preset.AddEntry("Notification title - leave empty to send this data via remote message", CONFIG_KEY_TITLE, mandatory=False)
-        # ask for the message only if the title is provided, otherwise don't ask (use display_if_value_for_following_key_provided)
-        preset.AddEntry("Notification message", CONFIG_KEY_MESSAGE, display_if_value_for_following_key_provided=CONFIG_KEY_TITLE, mandatory=True)
+        # ask for the message only if the title is provided, otherwise don't ask (use display_if_key_value)
+        preset.AddEntry("Notification message", CONFIG_KEY_MESSAGE, 
+            display_if_key_value={CONFIG_KEY_TITLE: True}, mandatory=True)
         return preset
```

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Notify/icon.png` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Notify/icon.png`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/OperatingSystem/OperatingSystem.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/OperatingSystem/OperatingSystem.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Power/Power.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Power/Power.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Ram/Ram.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Ram/Ram.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Temperature/Temperature.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Temperature/Temperature.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Uptime/Uptime.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Uptime/Uptime.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Username/Username.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Username/Username.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Deployments/Volume/Volume.py` & `IoTuring-2023.6.1/IoTuring/Entity/Deployments/Volume/Volume.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,61 +1,93 @@
 import subprocess
+import re
 
 from IoTuring.Entity.Entity import Entity
 from IoTuring.Entity.EntityData import EntityCommand, EntitySensor
 from IoTuring.Entity.ValueFormat import ValueFormatter, ValueFormatterOptions
 from IoTuring.MyApp.SystemConsts import OperatingSystemDetection as OsD
 
 KEY_STATE = 'volume_state'
 KEY_CMD = 'volume'
 
 EXTRA_KEY_MUTED_OUTPUT = 'Muted output'
 EXTRA_KEY_OUTPUT_VOLUME = 'Output volume'
 EXTRA_KEY_INPUT_VOLUME = 'Input volume'
 EXTRA_KEY_ALERT_VOLUME = 'Alert volume'
-VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0 = ValueFormatterOptions(value_type=ValueFormatterOptions.TYPE_PERCENTAGE, decimals=0)
+VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0 = ValueFormatterOptions(
+    value_type=ValueFormatterOptions.TYPE_PERCENTAGE, decimals=0)
+
+commands = {
+    OsD.OS_FIXED_VALUE_LINUX: 'pactl set-sink-volume @DEFAULT_SINK@ {}%',
+    OsD.OS_FIXED_VALUE_MACOS: 'osascript -e "set volume output volume {}"'
+}
+
 
 class Volume(Entity):
     NAME = "Volume"
 
-    def Initialize(self):        
-        if OsD.IsMacos():        
-            self.RegisterEntitySensor(EntitySensor(self, KEY_STATE, supportsExtraAttributes=True, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0))
-            self.RegisterEntityCommand(EntityCommand(
-                self, KEY_CMD, self.CallbackMac, KEY_STATE))
+    def Initialize(self):
+        extra_attributes = False
+
+        if OsD.IsLinux():
+            if not OsD.CommandExists("pactl"):
+                raise Exception(
+                    "Only PulseAudio is supported on Linux! Please open an issue on Github!")
+        elif OsD.IsMacos():
+            extra_attributes = True
         else:
-            raise Exception("Currently working only on macOS")
+            raise Exception("System not supported!")
 
+        # Register:
+        self.RegisterEntitySensor(EntitySensor(
+            self, KEY_STATE,
+            supportsExtraAttributes=extra_attributes,  # Extra attributes only on macos
+            valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0))
+        self.RegisterEntityCommand(EntityCommand(
+            self, KEY_CMD, self.Callback, KEY_STATE))
 
     def Update(self):
-        if OsD.IsMacos():        
+        if OsD.IsMacos():
             self.UpdateMac()
-    
-    def CallbackMac(self, message):
+        elif OsD.IsLinux():
+            # Example: 'Volume: front-left: 39745 /  61% / -13,03 dB,   ... 
+            # Only care about the first percent.
+            p = subprocess.run("pactl get-sink-volume @DEFAULT_SINK@",
+                               capture_output=True, shell=True, text=True)
+            self.Log(self.LOG_DEBUG, f"pactl stdout: {p.stdout}")
+            m = re.search(r"/ +(\d{1,3})% /", p.stdout)
+            if m:
+                volume = m.group(1)
+                self.SetEntitySensorValue(KEY_STATE, volume)
+
+    def Callback(self, message):
         payloadString = message.payload.decode('utf-8')
-        try:
-            # parse the payload and get the volume number which is between 0 and 100
-            volume = int(payloadString)
-            if volume < 0 or volume > 100:
-                raise Exception('Incorrect payload!')
-            self.SetVolumeMac(volume)
-        except Exception as e:
+
+        # parse the payload and get the volume number which is between 0 and 100
+        volume = int(payloadString)
+        if not 0 <= volume <= 100:
             raise Exception('Incorrect payload!')
-        
-    def SetVolumeMac(self, volume_level):
-        subprocess.run(['osascript', '-e', f'set volume output volume {volume_level}'], check=True)
+        else:
+            subprocess.run(
+                commands[OsD.GetOs()].format(volume),
+                shell=True, check=True)
 
     def UpdateMac(self):
         # result like: output volume:44, input volume:89, alert volume:100, output muted:false
-        result = subprocess.run(['osascript', '-e', 'get volume settings'], capture_output=True, text=True)
+        result = subprocess.run(
+            ['osascript', '-e', 'get volume settings'], capture_output=True, text=True)
         result = result.stdout.strip().split(',')
-        
+
         output_volume = result[0].split(':')[1]
         input_volume = result[1].split(':')[1]
         alert_volume = result[2].split(':')[1]
         output_muted = False if result[3].split(':')[1] == 'false' else True
-        
+
         self.SetEntitySensorValue(KEY_STATE, output_volume)
-        self.SetEntitySensorExtraAttribute(KEY_STATE, EXTRA_KEY_OUTPUT_VOLUME, output_volume, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0)
-        self.SetEntitySensorExtraAttribute(KEY_STATE, EXTRA_KEY_INPUT_VOLUME, input_volume, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0)
-        self.SetEntitySensorExtraAttribute(KEY_STATE, EXTRA_KEY_ALERT_VOLUME, alert_volume, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0)
-        self.SetEntitySensorExtraAttribute(KEY_STATE, EXTRA_KEY_MUTED_OUTPUT, output_muted)
+        self.SetEntitySensorExtraAttribute(
+            KEY_STATE, EXTRA_KEY_OUTPUT_VOLUME, output_volume, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0)
+        self.SetEntitySensorExtraAttribute(
+            KEY_STATE, EXTRA_KEY_INPUT_VOLUME, input_volume, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0)
+        self.SetEntitySensorExtraAttribute(
+            KEY_STATE, EXTRA_KEY_ALERT_VOLUME, alert_volume, valueFormatterOptions=VALUEFORMATTEROPTIONS_PERCENTAGE_ROUND0)
+        self.SetEntitySensorExtraAttribute(
+            KEY_STATE, EXTRA_KEY_MUTED_OUTPUT, output_muted)
```

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/Entity.py` & `IoTuring-2023.6.1/IoTuring/Entity/Entity.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
+from IoTuring.Configurator.ConfiguratorObject import ConfiguratorObject
 from IoTuring.Entity.EntityManager import EntityManager
 from IoTuring.Entity.ValueFormat import ValueFormatter
 from IoTuring.Exceptions.Exceptions import UnknownEntityKeyException
 from IoTuring.Logger.LogObject import LogObject
 from IoTuring.Entity.EntityData import EntitySensor, EntityCommand
 import time
 
 KEY_ENTITY_TAG = 'tag'  # from Configurator.Configurator
 
 DEFAULT_UPDATE_TIMEOUT = 10
 
 
-class Entity(LogObject):
+class Entity(LogObject, ConfiguratorObject):
     NAME = "Unnamed"
     ALLOW_MULTI_INSTANCE = False
 
     def __init__(self, configurations) -> None:
         # Prepare the entity
         self.entitySensors = []
         self.entityCommands = []
@@ -164,14 +165,7 @@
             self.tag = ""
 
     @classmethod
     def AllowMultiInstance(self):
         """ Return True if this Entity can have multiple instances, useful for customizable entities 
             These entities are the ones that must have a tag to be recognized """
         return self.ALLOW_MULTI_INSTANCE
-
-    # Configuration methods
-
-    @classmethod
-    def ConfigurationPreset(self):
-        """ Prepare a preset to manage settings insert/edit for the warehouse """
-        return None
```

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/EntityData.py` & `IoTuring-2023.6.1/IoTuring/Entity/EntityData.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,40 +1,49 @@
 from IoTuring.Logger.LogObject import LogObject
 
-# EntitySensor extra attribute aren't read from all the warehouses 
+# EntitySensor extra attribute aren't read from all the warehouses
+
 
 class EntityData(LogObject):
 
-    def __init__(self, entity, key):
+    def __init__(self, entity, key, customPayload = {}):
         self.entityId = entity.GetEntityId()
         self.id = self.entityId + "." + key
         self.key = key
         self.entity = entity
+        self.customPayload = customPayload
 
     def GetEntity(self):
         return self.entity
 
     def GetId(self):
         return self.id
 
     def GetKey(self):
         return self.key
 
     def LogSource(self):
         return self.GetId()
 
+    def GetCustomPayload(self):
+        return self.customPayload
+
 
 class EntitySensor(EntityData):
 
-    def __init__(self, entity, key, valueFormatterOptions=None, supportsExtraAttributes = False):
+    def __init__(self, entity, key,
+                 valueFormatterOptions=None,
+                 supportsExtraAttributes=False,
+                 customPayload={}):
         """
         If supportsExtraAttributes is True, the entity sensor can have extra attributes.
         valueFormatterOptions is a IoTuring.Entity.ValueFormat.ValueFormatterOptions object.
+        CustomPayload overrides HomeAssistant discovery configuration
         """
-        EntityData.__init__(self, entity, key)
+        EntityData.__init__(self, entity, key, customPayload)
         self.supportsExtraAttributes = supportsExtraAttributes
         self.value = None
         self.extraAttributes = None
         self.valueFormatterOptions = valueFormatterOptions
 
     def DoesSupportExtraAttributes(self):
         return self.supportsExtraAttributes
@@ -52,47 +61,54 @@
 
     def HasValue(self):
         """ True if self.value isn't empty """
         return self.value is not None
 
     def GetExtraAttributes(self):
         if self.supportsExtraAttributes == False:
-            raise Exception("This entity sensor does not support extra attributes. Please specify it when initializing the sensor.")
+            raise Exception(
+                "This entity sensor does not support extra attributes. Please specify it when initializing the sensor.")
         return self.extraAttributes
-    
+
     def HasExtraAttributes(self):
         """ True if self.extraAttributes isn't empty """
         return self.extraAttributes is not None
-    
+
     def SetExtraAttribute(self, name, value, valueFormatterOptions=None):
         if self.supportsExtraAttributes == False:
-            raise Exception("This entity sensor does not support extra attributes. Please specify it when initializing the sensor.")
+            raise Exception(
+                "This entity sensor does not support extra attributes. Please specify it when initializing the sensor.")
         if self.extraAttributes is None:
             self.extraAttributes = []
         # If the Attribute does not already exists, create it, otherwise update it
-        extraAttributeObj = next((attr for attr in self.extraAttributes if attr.GetName() == name), None)
+        extraAttributeObj = next(
+            (attr for attr in self.extraAttributes if attr.GetName() == name), None)
         if (extraAttributeObj is None):
-            self.extraAttributes.append(ExtraAttribute(name, value, valueFormatterOptions))
+            self.extraAttributes.append(ExtraAttribute(
+                name, value, valueFormatterOptions))
         else:
             extraAttributeObj.SetValue(value)
 
+
 class EntityCommand(EntityData):
 
-    def __init__(self, entity, key, callbackFunction, connectedEntitySensorKey = None):
+    def __init__(self, entity, key, callbackFunction,
+                 connectedEntitySensorKey=None, customPayload={}):
         """
         If a key for the entity sensor is passed, warehouses that support it use this command as a switch with state.
         Better to register the sensor before this command to avoud unexpected behaviours.
+        CustomPayload overrides HomeAssistant discovery configuration
         """
-        EntityData.__init__(self, entity, key)
+        EntityData.__init__(self, entity, key, customPayload)
         self.callbackFunction = callbackFunction
         self.connectedEntitySensorKey = connectedEntitySensorKey
 
     def SupportsState(self):
         return self.connectedEntitySensorKey is not None
-    
+
     def GetConnectedEntitySensor(self):
         """ Returns the entity sensor connected to this command, if this command supports state.
             Otherwise returns None. """
         return self.GetEntity().GetEntitySensorByKey(self.connectedEntitySensorKey)
 
     def CallCallback(self, message):
         """ Safely run callback for this command, passing the message (a paho.mqtt.client.MQTTMessage).
@@ -106,27 +122,28 @@
             return False
 
     def RunCallback(self, message):
         """ Called only by CallCallback. 
             Run callback for this command, passing the message (a paho.mqtt.client.MQTTMessage) """
         self.callbackFunction(message)
 
+
 class ExtraAttribute():
     def __init__(self, name, value, valueFormatterOptions=None):
         self.name = name
         self.value = value
         self.valueFormatterOptions = valueFormatterOptions
-        
+
     def GetName(self):
         return self.name
-    
+
     def GetValue(self):
         return self.value
-    
+
     def GetValueFormatterOptions(self):
         return self.valueFormatterOptions
-    
+
     def HasValueFormatterOptions(self):
         return self.valueFormatterOptions is not None
-    
+
     def SetValue(self, value):
-        self.value = value
+        self.value = value
```

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/EntityManager.py` & `IoTuring-2023.6.1/IoTuring/Entity/EntityManager.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Brightness/Brightness.py` & `IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Brightness/Brightness.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py` & `IoTuring-2023.6.1/IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Network/Network.py` & `IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Network/Network.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py` & `IoTuring-2023.6.1/IoTuring/Entity/ToImplement/Screenshot/Screenshot.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ToImplement/State/State.py` & `IoTuring-2023.6.1/IoTuring/Entity/ToImplement/State/State.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ValueFormat/ValueFormatter.py` & `IoTuring-2023.6.1/IoTuring/Entity/ValueFormat/ValueFormatter.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py` & `IoTuring-2023.6.1/IoTuring/Entity/ValueFormat/ValueFormatterOptions.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Logger/Logger.py` & `IoTuring-2023.6.1/IoTuring/Logger/Logger.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Logger/consts.py` & `IoTuring-2023.6.1/IoTuring/Logger/consts.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/MyApp/App.py` & `IoTuring-2023.6.1/IoTuring/MyApp/App.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/MyApp/SystemConsts/OperatingSystemDetection.py` & `IoTuring-2023.6.1/IoTuring/MyApp/SystemConsts/OperatingSystemDetection.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Protocols/MQTTClient/MQTTClient.py` & `IoTuring-2023.6.1/IoTuring/Protocols/MQTTClient/MQTTClient.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Protocols/MQTTClient/TopicCallback.py` & `IoTuring-2023.6.1/IoTuring/Protocols/MQTTClient/TopicCallback.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py` & `IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/ConsoleWarehouse/ConsoleWarehouse.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py` & `IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/HomeAssistantWarehouse.py`

 * *Files 6% similar despite different names*

```diff
@@ -85,18 +85,21 @@
             in case the command has a sensor connected to it (= is a switch).
             This is needed to avoid status blinking on HA."""
         def CommandCallback(message):
             status = entityCommand.CallCallback(
                 message)  # True: success, False: error
             if status and self.client.IsConnected():
                 if entityCommand.SupportsState():
-                    self.Log(self.LOG_DEBUG, "Switch callback: sending state to " +
-                             self.MakeEntityDataTopicForSensorByCommandIfSwitch(entityCommand))
-                    self.client.SendTopicData(self.MakeEntityDataTopicForSensorByCommandIfSwitch(
-                        entityCommand), message.payload.decode('utf-8'))
+
+                    connected_sensor = entityCommand.GetConnectedEntitySensor()
+                    # Only set value if it was already set, to exclude optimistic switches
+                    if connected_sensor.HasValue():
+                        sensor_topic = self.MakeEntityDataTopic(connected_sensor)
+                        self.Log(self.LOG_DEBUG, "Switch callback: sending state to " + sensor_topic)
+                        self.client.SendTopicData(sensor_topic, message.payload.decode('utf-8'))
         return CommandCallback
 
     def Loop(self):
         # Send online state
         self.client.SendTopicData(self.MakeValuesTopic(
             LWT_TOPIC_SUFFIX), LWT_PAYLOAD_ONLINE)
 
@@ -149,26 +152,28 @@
             for entityData in entity.GetAllEntityData():
 
                 # if I found a sensor data that will be configured only after, together with
                 # its command (as a switch)
                 if entityData.GetKey() in keys_of_sensors_connected_to_commands:
                     continue  # it's a sensor linked to a command, so skip
 
-                entitycommand_supports_state = False
+                connected_sensor = None
+                is_entity_sensor = False
                 data_type = ""
                 autoDiscoverySendTopic = ""
                 payload = {}
                 payload['name'] = entity.GetEntityNameWithTag() + " - " + \
                     entityData.GetKey()
 
                 if entityData in entity.GetEntitySensors():  # it's an EntitySensorData
                     data_type = "sensor"
+                    is_entity_sensor = True
                 elif entityData.SupportsState():  # it's a EntityCommandData: has it a state ?
                     data_type = "switch"
-                    entitycommand_supports_state = True
+                    connected_sensor = entityData.GetConnectedEntitySensor()
                 else:
                     data_type = "button"
 
                 # add custom info to the entity data, reading it from external file and accessing the information using the entity data name
                 payload = self.AddEntityDataCustomConfigurations(
                     payload['name'], payload)
                 # check if custom configs have a new data type
@@ -181,37 +186,35 @@
                     payload['name'] = self.clientName + " " + payload['name']
 
                 payload['device'] = self.MakeApplicationConfiguration()
                 payload['unique_id'] = self.clientName + \
                     "." + entityData.GetId()
 
                 # add configurations about sensors or switches (both have a state)
-                if entityData in entity.GetEntitySensors() or entitycommand_supports_state:  # it's an EntitySensorData
+                if is_entity_sensor or connected_sensor:
                     # If the sensor supports extra attributes, send them as JSON.
                     # So here I have to specify also the topic for those attributes
-                    # - for sensors that became switches: entityData is the command 
-                    # so I need to retrieve the sensor and check there if supports extra attributes 
+                    # - for sensors that became switches: entityData is the command
+                    # so I need to retrieve the sensor and check there if supports extra attributes
                     # and get from there the topic
-                    if entitycommand_supports_state and entityData.GetConnectedEntitySensor().DoesSupportExtraAttributes():
+
+                    # select the sensor for data:
+                    if connected_sensor:
+                        data_sensor = connected_sensor
+                    else:
+                        data_sensor = entityData
+
+                    # extra attributes
+                    if data_sensor.DoesSupportExtraAttributes():
                         payload["json_attributes_topic"] = self.MakeEntityDataExtraAttributesTopic(
-                            entityData.GetConnectedEntitySensor())
+                            data_sensor)
                     
-                    # - for real sensors -
-                    elif not entitycommand_supports_state and entityData.DoesSupportExtraAttributes():
-                        payload["json_attributes_topic"] = self.MakeEntityDataExtraAttributesTopic(
-                            entityData)
-
                     payload['expire_after'] = 600  # TODO Improve
 
-                    if entitycommand_supports_state: # it has a state, so the key of the sensor to generate the topic is found in the sensor
-                        payload['state_topic'] = self.MakeEntityDataTopicForSensorByCommandIfSwitch(
-                            entityData)
-                    else: # it's a real sensor:
-                        payload['state_topic'] = self.MakeEntityDataTopic(
-                            entityData)
+                    payload['state_topic'] = self.MakeEntityDataTopic(data_sensor)
 
                 # Add default payloads (only for ON/OFF entities)
                 if data_type in ["binary_sensor", "switch"]:
                     if not 'payload_on' in payload:
                         payload['payload_on'] = PAYLOAD_ON
                     if not 'payload_off' in payload:
                         payload['payload_off'] = PAYLOAD_OFF
@@ -226,14 +229,20 @@
 
                 # Add availability configuration
                 payload["availability_topic"] = self.MakeValuesTopic(
                     LWT_TOPIC_SUFFIX)
                 payload["payload_available"] = LWT_PAYLOAD_ONLINE
                 payload["payload_not_available"] = LWT_PAYLOAD_OFFLINE
 
+                # Override from custom entity payload config:
+                custom_payload = entityData.GetCustomPayload()
+                if connected_sensor:
+                    custom_payload = {**custom_payload, **connected_sensor.GetCustomPayload()}
+                payload.update(custom_payload)
+                
                 # Send
                 self.client.SendTopicData(
                     autoDiscoverySendTopic, json.dumps(payload))
 
     def SendLwtSensorConfiguration(self):
         """ Sends the same configuration as any other entity, but for the lwt message value (so we have
             a message with a value that isn't from an entity and we want to send discovery data for it) """
@@ -272,22 +281,14 @@
                 for entityData, entityDataConfiguration in data.items():
                     # entityData may be the correct name, or a regex expression that should return something applied to the real name
                     if re.search(entityData, entityDataName):
                         # merge payload and additional configurations
                         return {**payload, **entityDataConfiguration}
         return payload  # if nothing found
 
-    def MakeEntityDataTopicForSensorByCommandIfSwitch(self, entityData):
-        """ If the entityData is a command, returns the topic of the sensor connected to it """
-        if entityData.SupportsState():
-            return self.MakeEntityDataTopic(entityData.GetConnectedEntitySensor())
-        else:
-            raise Exception(entityData.GetID() +
-                            " is not a switch, can't get its sensor topic")
-
     def MakeEntityDataTopic(self, entityData):
         """ Uses MakeValuesTopic but receives an EntityData to manage itself its id"""
         return self.MakeValuesTopic(entityData.GetId())
 
     def MakeEntityDataExtraAttributesTopic(self, entityData):
         """ Uses MakeValuesTopic but receives an EntityData to manage itself its id, appending a suffix to distinguish
             the extra attrbiutes from the original value """
@@ -303,15 +304,15 @@
         device['model'] = self.clientName
         device['identifiers'] = self.clientName
         device['manufacturer'] = App.getName() + " by " + App.getVendor()
         device['sw_version'] = App.getVersion()
         return device
 
     @classmethod
-    def ConfigurationPreset(self):
+    def ConfigurationPreset(cls) -> MenuPreset:
         preset = MenuPreset()
         preset.AddEntry("Home assistant MQTT broker address",
                         CONFIG_KEY_ADDRESS, mandatory=True)
         preset.AddEntry("Port", CONFIG_KEY_PORT, default=1883)
         preset.AddEntry("Client name", CONFIG_KEY_NAME, mandatory=True)
         preset.AddEntry("Username", CONFIG_KEY_USERNAME, default="")
         preset.AddEntry("Password", CONFIG_KEY_PASSWORD, default="")
```

### Comparing `IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml` & `IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/HomeAssistantWarehouse/entities.yaml`

 * *Files 13% similar despite different names*

```diff
@@ -51,14 +51,15 @@
   icon: "mdi:calculator-variant"
 Cpu: # if no matches with above CPU patterns, set this
   icon: "mdi:calculator-variant"
 Time:
   icon: "mdi:clock"
 Monitor:
   icon: "mdi:monitor-shimmer"
+  custom_type: switch
 AppInfo - update:
   custom_type: binary_sensor
   icon: "mdi:package-up"
   device_class: "update"
   payload_on: "True"
   payload_off: "False"
 AppInfo:
@@ -77,8 +78,29 @@
 FileSwitch:
   icon: mdi:file-star
   payload_on: "True"
   payload_off: "False"
 Volume:
   icon: mdi:volume-high
   unit_of_measurement: "%"
-  custom_type: number
+  custom_type: number
+TerminalPayloadCommand:
+  icon: mdi:console-line
+  custom_type: text
+TerminalSwitch:
+  icon: mdi:console
+  custom_type: switch
+TerminalSensor:
+  icon: mdi:console
+  custom_type: sensor
+TerminalBinarySensor:
+  icon: mdi:console
+  custom_type: binary_sensor
+TerminalCover:
+  icon: mdi:console
+  custom_type: cover
+  state_closing: CLOSE
+  state_opening: OPEN
+  state_stopped: STOP
+TerminalButton:
+  icon: mdi:console
+  custom_type: button
```

### Comparing `IoTuring-2023.5.1/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py` & `IoTuring-2023.6.1/IoTuring/Warehouse/Deployments/MQTTWarehouse/MQTTWarehouse.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,15 +74,15 @@
             for entity in self.GetEntities():
                 for entityCommand in entity.GetEntityCommands():
                     f.write(entityCommand.GetId() + " registered on " +
                             self.MakeTopic(entityCommand)+"\n")
 
     # CONFIGURATION
     @classmethod
-    def ConfigurationPreset(self):
+    def ConfigurationPreset(cls) -> MenuPreset:
         preset = MenuPreset()
         preset.AddEntry("Address", CONFIG_KEY_ADDRESS, mandatory=True)
         preset.AddEntry("Port", CONFIG_KEY_PORT, default=1883)
         preset.AddEntry("Client name", CONFIG_KEY_NAME, default=App.getName())
         preset.AddEntry("Username", CONFIG_KEY_USERNAME, default="")
         preset.AddEntry("Password", CONFIG_KEY_PASSWORD, default="")
         preset.AddEntry("Add units to values (Y/N)", CONFIG_KEY_ADD_UNITS, default="Y", modify_value_callback=MenuPreset.Callback_NormalizeBoolean)
```

### Comparing `IoTuring-2023.5.1/IoTuring/Warehouse/Warehouse.py` & `IoTuring-2023.6.1/IoTuring/Warehouse/Warehouse.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from IoTuring.Configurator.MenuPreset import BooleanAnswers
 from IoTuring.Logger.LogObject import LogObject
+from IoTuring.Configurator.ConfiguratorObject import ConfiguratorObject
 from IoTuring.Entity.EntityManager import EntityManager
 
 from threading import Thread
 import time
 
 DEFAULT_LOOP_TIMEOUT = 10
 
 
-class Warehouse(LogObject):
+class Warehouse(LogObject, ConfiguratorObject):
     NAME = "Unnamed"
 
     def __init__(self, configurations) -> None:
         self.loopTimeout = DEFAULT_LOOP_TIMEOUT
         self.configurations = configurations
 
     def Start(self) -> None:
@@ -69,13 +70,7 @@
     def GetTrueOrFalseFromConfigurations(self, key):
         """ Get boolean value from confiugurations with key (if not present raise Exception) """
         value = self.GetFromConfigurations(key).lower()
         if value in BooleanAnswers.TRUE_ANSWERS:
             return True
         else:
             return False
-
-    # Configuration methods
-    @classmethod
-    def ConfigurationPreset(self):
-        """ Prepare a preset to manage settings insert/edit for the warehouse """
-        return None
```

### Comparing `IoTuring-2023.5.1/IoTuring/__init__.py` & `IoTuring-2023.6.1/IoTuring/__init__.py`

 * *Files identical despite different names*

### Comparing `IoTuring-2023.5.1/IoTuring.egg-info/PKG-INFO` & `IoTuring-2023.6.1/IoTuring.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoTuring
-Version: 2023.5.1
+Version: 2023.6.1
 Summary: Simple and powerful cross-platform script to control your pc and share statistics using communication protocols like MQTT and home control hubs like HomeAssistant.
 Author-email: richibrics <riccardo.briccola.dev@gmail.com>, infeeeee <gyetpet@mailbox.org>
 Maintainer-email: richibrics <riccardo.briccola.dev@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -797,15 +797,15 @@
 
 Your computer will show up in HomeAssistant as a single Device, so all your entities will be grouped together. 
 The device will also have some properties like connectivity and battery status.
 
 You can see how your device will appear under the Devices section in Home Assistant in the following GIF (wait until it's loaded):
 
 
-![device](docs/images/homeassistant-demo.gif)
+![device](https://github.com/richibrics/IoTuring/blob/main/docs/images/homeassistant-demo.gif?raw=true)
 
 All sensors and switches will be available to be added to your dashboard in your favourite cards !
 
 ## Features
 
 ### Available entities
 
@@ -814,26 +814,28 @@
 | ActiveWindow       | shares the name of the window you're working on                             | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | AppInfo            | shares app informations like the running version                            | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Battery            | shares the battery level and charging status                                | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | BootTime           | shares the machine boot time                                                | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Cpu                | shares useful information about cpu usage (times, frequencies, percentages) | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | DesktopEnvironment | shares the running desktop environment (useful only for Linux)              | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Disk               | shares disk usage data                                                      | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
+| DisplayMode        | command for changing multimonitor display mode                              | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) |
 | Hostname           | shares the machine hostname                                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Lock               | command for locking the machine                                             | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Monitor            | command for switching monitors on/off                                       | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                             |
 | Notify             | displays a notification                                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
-| Os                 | shares the operating system of your machine                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
+| OperatingSystem    | shares the operating system of your machine                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Power*             | commands for poweroff, reboot and sleep                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Ram                | shares useful information about ram usage                                   | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Time               | shares the machine local time                                               | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Temperature        | shares temperature sensor data                                              | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                             |
+| Terminal           | runs custom commands in the shell                                           | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Uptime             | shares the time since the machine is on                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Username           | shares the name of the user who is working on the machine                   | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
-| Volume           | control audio volume                | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png)  |
+| Volume             | control audio volume                                                        | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                                                             |
 
 \* To use the features from Power entity on Linux and macOS you need to give permissions to your user to shutdown and reboot without sudo password.
 You can easily do that by adding the following line at the end of the "/etc/sudoers" file (you can use the following command: sudo nano /etc/sudoers):
 
 ```
 YOURUSERNAMEHERE ALL=(ALL) NOPASSWD: /sbin/poweroff, /sbin/reboot, /sbin/shutdown
 ```
```

### Comparing `IoTuring-2023.5.1/IoTuring.egg-info/SOURCES.txt` & `IoTuring-2023.6.1/IoTuring.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 IoTuring/ClassManager/ClassManager.py
 IoTuring/ClassManager/EntityClassManager.py
 IoTuring/ClassManager/WarehouseClassManager.py
 IoTuring/ClassManager/consts.py
 IoTuring/Configurator/Configurator.py
 IoTuring/Configurator/ConfiguratorIO.py
 IoTuring/Configurator/ConfiguratorLoader.py
+IoTuring/Configurator/ConfiguratorObject.py
 IoTuring/Configurator/MenuPreset.py
 IoTuring/Entity/Entity.py
 IoTuring/Entity/EntityData.py
 IoTuring/Entity/EntityManager.py
 IoTuring/Entity/Deployments/ActiveWindow/ActiveWindow.py
 IoTuring/Entity/Deployments/AppInfo/AppInfo.py
 IoTuring/Entity/Deployments/Battery/Battery.py
@@ -34,24 +35,24 @@
 IoTuring/Entity/Deployments/Monitor/Monitor.py
 IoTuring/Entity/Deployments/Notify/Notify.py
 IoTuring/Entity/Deployments/Notify/icon.png
 IoTuring/Entity/Deployments/OperatingSystem/OperatingSystem.py
 IoTuring/Entity/Deployments/Power/Power.py
 IoTuring/Entity/Deployments/Ram/Ram.py
 IoTuring/Entity/Deployments/Temperature/Temperature.py
+IoTuring/Entity/Deployments/Terminal/Terminal.py
 IoTuring/Entity/Deployments/Time/Time.py
 IoTuring/Entity/Deployments/Uptime/Uptime.py
 IoTuring/Entity/Deployments/Username/Username.py
 IoTuring/Entity/Deployments/Volume/Volume.py
 IoTuring/Entity/ToImplement/Brightness/Brightness.py
 IoTuring/Entity/ToImplement/CpuTemperature/CpuTemperatures.py
 IoTuring/Entity/ToImplement/Network/Network.py
 IoTuring/Entity/ToImplement/Screenshot/Screenshot.py
 IoTuring/Entity/ToImplement/State/State.py
-IoTuring/Entity/ToImplement/Terminal/Terminal.py
 IoTuring/Entity/ValueFormat/ValueFormatter.py
 IoTuring/Entity/ValueFormat/ValueFormatterOptions.py
 IoTuring/Entity/ValueFormat/__init__.py
 IoTuring/Exceptions/Exceptions.py
 IoTuring/Logger/Colors.py
 IoTuring/Logger/LogObject.py
 IoTuring/Logger/Logger.py
```

### Comparing `IoTuring-2023.5.1/PKG-INFO` & `IoTuring-2023.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: IoTuring
-Version: 2023.5.1
+Version: 2023.6.1
 Summary: Simple and powerful cross-platform script to control your pc and share statistics using communication protocols like MQTT and home control hubs like HomeAssistant.
 Author-email: richibrics <riccardo.briccola.dev@gmail.com>, infeeeee <gyetpet@mailbox.org>
 Maintainer-email: richibrics <riccardo.briccola.dev@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
@@ -797,15 +797,15 @@
 
 Your computer will show up in HomeAssistant as a single Device, so all your entities will be grouped together. 
 The device will also have some properties like connectivity and battery status.
 
 You can see how your device will appear under the Devices section in Home Assistant in the following GIF (wait until it's loaded):
 
 
-![device](docs/images/homeassistant-demo.gif)
+![device](https://github.com/richibrics/IoTuring/blob/main/docs/images/homeassistant-demo.gif?raw=true)
 
 All sensors and switches will be available to be added to your dashboard in your favourite cards !
 
 ## Features
 
 ### Available entities
 
@@ -814,26 +814,28 @@
 | ActiveWindow       | shares the name of the window you're working on                             | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | AppInfo            | shares app informations like the running version                            | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Battery            | shares the battery level and charging status                                | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | BootTime           | shares the machine boot time                                                | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Cpu                | shares useful information about cpu usage (times, frequencies, percentages) | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | DesktopEnvironment | shares the running desktop environment (useful only for Linux)              | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Disk               | shares disk usage data                                                      | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
+| DisplayMode        | command for changing multimonitor display mode                              | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) |
 | Hostname           | shares the machine hostname                                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Lock               | command for locking the machine                                             | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Monitor            | command for switching monitors on/off                                       | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                             |
 | Notify             | displays a notification                                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
-| Os                 | shares the operating system of your machine                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
+| OperatingSystem    | shares the operating system of your machine                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Power*             | commands for poweroff, reboot and sleep                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Ram                | shares useful information about ram usage                                   | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Time               | shares the machine local time                                               | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Temperature        | shares temperature sensor data                                              | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                             |
+| Terminal           | runs custom commands in the shell                                           | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Uptime             | shares the time since the machine is on                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Username           | shares the name of the user who is working on the machine                   | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
-| Volume           | control audio volume                | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png)  |
+| Volume             | control audio volume                                                        | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                                                             |
 
 \* To use the features from Power entity on Linux and macOS you need to give permissions to your user to shutdown and reboot without sudo password.
 You can easily do that by adding the following line at the end of the "/etc/sudoers" file (you can use the following command: sudo nano /etc/sudoers):
 
 ```
 YOURUSERNAMEHERE ALL=(ALL) NOPASSWD: /sbin/poweroff, /sbin/reboot, /sbin/shutdown
 ```
```

### Comparing `IoTuring-2023.5.1/README.md` & `IoTuring-2023.6.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -103,15 +103,15 @@
 
 Your computer will show up in HomeAssistant as a single Device, so all your entities will be grouped together. 
 The device will also have some properties like connectivity and battery status.
 
 You can see how your device will appear under the Devices section in Home Assistant in the following GIF (wait until it's loaded):
 
 
-![device](docs/images/homeassistant-demo.gif)
+![device](https://github.com/richibrics/IoTuring/blob/main/docs/images/homeassistant-demo.gif?raw=true)
 
 All sensors and switches will be available to be added to your dashboard in your favourite cards !
 
 ## Features
 
 ### Available entities
 
@@ -120,26 +120,28 @@
 | ActiveWindow       | shares the name of the window you're working on                             | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | AppInfo            | shares app informations like the running version                            | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Battery            | shares the battery level and charging status                                | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | BootTime           | shares the machine boot time                                                | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Cpu                | shares useful information about cpu usage (times, frequencies, percentages) | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | DesktopEnvironment | shares the running desktop environment (useful only for Linux)              | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Disk               | shares disk usage data                                                      | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
+| DisplayMode        | command for changing multimonitor display mode                              | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) |
 | Hostname           | shares the machine hostname                                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Lock               | command for locking the machine                                             | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Monitor            | command for switching monitors on/off                                       | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                             |
 | Notify             | displays a notification                                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
-| Os                 | shares the operating system of your machine                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
+| OperatingSystem    | shares the operating system of your machine                                 | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Power*             | commands for poweroff, reboot and sleep                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Ram                | shares useful information about ram usage                                   | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Time               | shares the machine local time                                               | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Temperature        | shares temperature sensor data                                              | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                             |
+| Terminal           | runs custom commands in the shell                                           | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Uptime             | shares the time since the machine is on                                     | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
 | Username           | shares the name of the user who is working on the machine                   | ![win](https://github.com/richibrics/IoTuring/blob/main/docs/images/win.png?raw=true) ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png) |
-| Volume           | control audio volume                | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png)  |
+| Volume             | control audio volume                                                        | ![mac](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/mac.png) ![linux](https://raw.githubusercontent.com/richibrics/IoTuring/main/docs/images/linux.png)                                                             |
 
 \* To use the features from Power entity on Linux and macOS you need to give permissions to your user to shutdown and reboot without sudo password.
 You can easily do that by adding the following line at the end of the "/etc/sudoers" file (you can use the following command: sudo nano /etc/sudoers):
 
 ```
 YOURUSERNAMEHERE ALL=(ALL) NOPASSWD: /sbin/poweroff, /sbin/reboot, /sbin/shutdown
 ```
```

### Comparing `IoTuring-2023.5.1/pyproject.toml` & `IoTuring-2023.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "IoTuring"
-version = "2023.5.1"
+version = "2023.6.1"
 description = "Simple and powerful cross-platform script to control your pc and share statistics using communication protocols like MQTT and home control hubs like HomeAssistant."
 readme = "README.md"
 requires-python = ">=3.7"
 license = {file = "COPYING"}
 keywords = ["iot","mqtt","monitor"]
 authors = [
   {name = "richibrics", email = "riccardo.briccola.dev@gmail.com"},
```

