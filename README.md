# Esp32-Stick-Cam-Boards-ESPHome

Go to Add-ons in Home assistant and open ESP Home add-on, you can also click this link to open it
https://my.home-assistant.io/redirect/config_flow_start?domain=esphome

* Install ESP Home if you don't have it yet
* Open ESP Home add-on
* Click NEW DEVICE at bottom right
  ![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/c7e43185-e3d6-4bba-bd44-5adeea2c1403)
  ![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/768d3dc3-c80f-4107-9079-0b1536e8b4d1)
* Enter name of the device and WIFI detail if it asks you
  ![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/3d3865b0-3ccd-4140-8f95-477f23462080)
  ![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/a8cfe7fe-a4cf-4b9d-b006-e9dbe5a17df3)
* Don't install the firmware on the device yet, just click skip or continue
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/dd1d7fcc-e388-415d-b237-cf9a222dbe74)
* Click edit on the device you just created, delete the generated configuration and replace it by contents of eth-cam.yaml
* If you want uncomment OTA password and API encryption and enter ota and api passwords, boath can be randomly generated
  ![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/d3351019-1d8d-41a1-bd61-0acb9fbe6724)
  ![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/9a369965-0753-4713-b4cc-6f4e6a151f68)
* Flash the device, click install and
  * If you are using https click plug into this computer, connect the device, select serial port and wait for the code to upload, and you are done. Now you can add the esp32-stic-cam board to your home assistant
  * If you are not using https folow instruction below
   * click manual download
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/26380470-bfe0-48b0-a069-de01b1e2320b)
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/a90f0998-8b38-4de1-b30b-047cd9eb4e9c)
   * then go to https://web.esphome.io/ and click connect
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/4a83891f-7e3a-4083-864a-f909e016c55e)
   * connect the device to USB, select serial port, thet newly appeard
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/c9a2e1e7-16c0-4ab9-bac0-2abfea181513)
  * then click install
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/98251adb-80cb-4abe-a9a4-5c65870eddd8)
  * Select the file you just downloaded
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/9692572a-dcae-4154-b3d4-260fe3df7059)
  * Click install to install the firmware on the device
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/58978e65-b4de-4bf7-8dab-bf81dda495f6)
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/a6ab4079-3d33-40a2-a195-c7efa78d11dd)
* Now is time to add the camera to home assistant. Go to Settings and than to Devices & services
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/0cc6b549-004e-484b-a79f-40fa7fb92916)
* The device sould be descoverd automaticky, just clic configure and select area. If you enabled api encryption it will ask for the key.
![image](https://github.com/petrak-vitek/Esp32-Stick-Cam-Boards-ESPHome/assets/76689233/640acbcb-0246-4dd0-a6c1-3ded76939cf7)
  * If the device was not desocered automaticky clic ADD INTEGRATION select ESPHome and enter ip address of Esp32-Stick-Cam (you can find it in your router)
