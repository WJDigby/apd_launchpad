# apd_launchpad
Facilitate the creation of hostapd-wpe configuration files and spoofed certificates for WPA2 Enterprise credential harvesting.

Place apd_launchpad.py in your (functioning) hostapd-wpe directory. Running the script creates a new subdirectory named after the "TARGET" parameter and containing the associated configuration and certificate files which can be removed following the assessment.

hostapd-wpe related arguments:

-s SSID, --ssid SSID

SSID of wireless network. Required.

-i INTERFACE, --interface INTERFACE  

Wireless interface on which to broadcast. Required.

-ch CHANNEL, --channel CHANNEL  

Channel on which to broadcast (default "1").

-bc {0,1,2}, --broadcast {0,1,2}  

Broadcast or cloak the SSID. 0=Broadcast SSID; 1=Send empty SSID beacon (length=0); 2=Send SSID beacon with length (length=N) (default 0).

-br BRIDGE, --bridge BRIDGE

Bridge interface to use for MitM (default none).

-w {1,2}, --wpa {1,2}

Version of WPA (default "2")

-cn COMMON_NAME, --common-name COMMON_NAME

Common name for certificate. Required.

-o ORG, --org ORG     

Organization for certificate. Optional.

-st STATE, --state STATE

State or province for certificate. Optional.

-c COUNTRY, --country COUNTRY

Country code for certificate. Optional.

-p PASSWORD, --password PASSWORD

Password for certificate generation (default "password").

-l LOCATION, --location LOCATION

Location for certificate. Optional.

-ou ORG_UNIT, --org-unit ORG_UNIT

Organizatoinal unit for certificate. Optional.

-e EMAIL, --email EMAIL

Email address for cerificate. Optional.

-v, --verbose

Show verbose output.
