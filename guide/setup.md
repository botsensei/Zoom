## Start Zoomin

### Step 1. Insert mini SD card into SD Adapter then into computer

After inserting check to see if the card shows up as **boot**. 

### Step 2. Get your wifi network name and password

### Step 3. Set Up Your WiFi

There are many ways to set up your WiFi but byfar the easiest way is to:

1. Download and open this file with your favorite text editor (like MS Word): [wpa_supplicant.conf](/assets/wpa_supplicant.conf)

   It should look something like this:

   ```bash
   ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
   network={
       ssid="YOUR_SSID"
       psk="YOUR_WIFI_PASSWORD"
       key_mgmt=WPA-PSK
   }
   ```

2. Change the WiFi settings to match yours. Follow our example:

   **Example ssid:** whizkit

   **Example psk:** zoomzoomzoom

   ```bash
   ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
   network={
       ssid="whizkit" #this where your WiFi name goes like 'whizkit'
       psk="zoomzoomzoom" #this is where your password goes
       key_mgmt=WPA-PSK
   }
   ```

   If you don't have a password, follow this example:

   Example **ssid**: whizkit

   Example **key_mgmt**:NONE

   ```bash
   ctrl_interface=DIR=/var/run/wpa_supplicant GROUP=netdev
   network={
       ssid="whizkit" #this where your WiFi name goes like 'whizkit'
       key_mgmt=NONE #since you have no password change this to NONE
   }
   ```

Now, save the file then drag and drop to the SD card you inserted earlier named **boot**.

### Step 4. Safely eject the SD card, reinsert into the PiBrain, and turn on Zoom. 

### Step 5. Log into whizkit launchpad 

After you turn on the Zoom head to [launchpad](launchpad.whiz.fun). Here you can see if the device is connected (make sure you are on the same wifi network) and if so you are now able to access test-drive. 

### Step 6. Access Zoom controller

### Step 7. Insert or connect to USB controller

### Step 8. Select Gamepad Option

### Step 9. Practice driving around the track!

### Step 10. Press START to collect training data

### Step 11. Download training data 

### Step 12. Head to Colab
