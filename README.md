This CSIDataGather is made possible by ESP-IDF API. Refer to the API Guide to flash the CSIDataGather code on to ESP32. (https://docs.espressif.com/projects/esp-idf/en/latest/index.html#esp-idf-programming-guide)

Setup the menuconfig and graph:
1. in menuconfig change CPU Frequency to 240MHz
2. Run make flash monitor to check if data is being gathered
3. make moniotr > raw.log 
4. Open up new terminal in the CSIDataGather folder
5. tail -f raw.log | python SubMag.py

Matlab is used to process time series data and machine learning toolbox is used for training long-short-term-memory network. For more details please check out the matlab file.

By University of Washington, Tacoma students: Francisco Radilla, Jordan Gonzalas, Liezel Reoganis, Wendy Yunqi Yu
