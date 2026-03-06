# Amateur Radio Antenna Coverage Simulation (A Beginner Tutorial)
This writing demonstrates how to simulate an antenna coverage from a specific station setup on amateur radio frequency using the "ray-tracing" propagation model.

The tool used in this writing is [**Radio Mobile Online by VE2DBE**](https://www.ve2dbe.com/rmonline_s.asp); therefore, big credits to him.

<p align="center">
  <img src="frontpage.png" alt="frontpage" width="700"/>
</p>

## Study Case
The case that we are going to solve is as follows; 
We are going to install an APRS digipeater (VHF: 144.390 MHz) on a mountain/hill. The equipment that will be used has the following characteristics/constraints:
1. **Icom IC-2200 VHF transceiver**, mid-lo-Tx Power (10 Watts), typical Rx sensitivity (0.13 uV). This value will be de-rated to 0.25 uV to account for the worst case.
2. **Telex HyGain V-2R antenna** (5dBi of Gain)
3. **15m of RG-8 cable**, solid dielectric (1.38 dB of attenuation). This value will be de-rated to -1.5 dB to account for the worst case.
4. **10m high tower**
5. Location is at a mountain/hill.
6. Residential noise level.

The constraints above are a simple-case assumption that more or less describes typical installation conditions.

## Pick the Location
From the main menu, locate the **"New Site"** button and click it.
<p align="center">
  <img src="mainmenu.png" alt="mainmenu" width="700"/>
</p>

You will be presented with the map. Go ahead, navigate the map to find your preferred location. In this case, I will choose the Mt.Karang in Padeglang (Banten, Indonesia) as my preferred location. Click the **"Place cursor at center"** button, drag the pin, zoom in/out as needed, make sure the location is correct, and click **"Submit"**.
<p align="center">
  <img src="map.png" alt="map" width="700"/>
</p>

You will be redirected to the New Site page. Type the location name and click **"Add to My Sites"**.
<p align="center">
  <img src="savelocation.png" alt="savelocation" width="700"/>
</p>

If you are successful, your location will be listed in the **"My Sites"** menu from the Main Menu options.
<p align="center">
  <img src="confirmlisting.png" alt="confirmlisting" width="700"/>
</p>

Congrats! You are successful to define a location. Now, back to the main menu by clicking the **"Return to Main Menu"** button.

## Define the RF Parameters
From the main menu, click the **"New Coverage"** button.

Enter the relevant parameters:
1. **"Center Site"**: Your location name we just made earlier.
2. **"Antenna Height"**: 10m above the ground (case study).
3. **"Antenna Gain"**: 5dB (case study)
4. **"Mobile Antenna Height"**: 3m (car's / mobile antenna)
5. **"Mobile Antenna Gain"**: 3dB (mobile antenna)
6. **"Freq"**: 144.39 MHz
7. **"Tx Power (Watts)"**: 10 Watts (case study)
8. **"Tx Line Loss (dB)"**: 1.5 dB (case study)
9. **"Rx Line Loss (dB)"**: 1.0 dB (assumption)
10. **"Rx threshold (uV)"**: 0.25 uV (case study)
11. **"Required Reliability"**: 80 % (assumption)
12. **"Maximum Range (km)"**: Choose whatever maximum range you want to evaluate. I personally choose 100 - 300 km. The maximum is 300 km.

After finishing, click **"Submit"**.

If everything is okay, the calculation progress page is presented, and you need to wait until it finishes.

## Evaluating The Results
The coverage map will be presented. It is recommended to save the current coverage map by clicking **"Add to my Coverage"** button.

