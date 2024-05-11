# HPI-Socks-Proxy
A script to easily enable a socks proxy to HPI on MacOS and setup instructions
## Setup

### 1. Socks Proxy

1. Go to System Settings -> Network -> your interface (WiFi, Ethernet, etc.) -> Details -> Proxies
2. Enable SOCKS proxy, enter localhost as server and 9999 as port
3. Click okay
4. Disable it
5. Click okay again (the correct proxy is now saved and can be enabled by my script)

### 2. Keychain

1. Open keychain acess
2. Either change hpi-socks to your keychain entry containing your password or add a new keychain entry named hpi-socks and your HPI-password

### 3. (Optional) Change your default interface

1. To list all available interfaces enter `networksetup -listallnetworkservices` in a Terminal
2. Replace my default with the one you'd like to use

### 4. (Optional) Move the script to /usr/local/bin don't need to enter the full path everytime you launch the thing

## Done
### You can now access ressources that would normally require you to be at HPI.
After you're done reading Papers etc. just kill the script and the proxy will be deactivated again

### Disclaimer!!

I'm pretty shitty at cybersec but im pretty sure that your hpi password will be stored somewhere outside of the keychain on runtime. I don't know for how long and I don't know how to make it saver. If you do, feel free to make a PR :))
