## SSH Tunnel for Windows OS

summary:
    In this tutorial you are going to learn how to use ssh tunel to make your own vpn.    
---

### Requirements:

1. nekoray

### Step 1 - Creating new SSH
Go to website [vpnjantit.com](https://vpanjantit.com)
1. Click on Free VPN SSH
2. Create Free SSH Tunnel
3. Choose a Country (France & Italy suggested)
4. Set username and password (set both the same)
5. Check the checkbox of "I'm not a robot"
6. Click on Create Free SSH Tunnel
7. Click on Show IP from the right side of the page
8. Copy the given IP.
done

### Step 2 - Cmd
Open Cmd and run these command:

```text
    ssh -p 22 -N -D 4002 username-vpnjantit.com@IP
```

After that, if Cmd wants to set fingerprint, type "yes" then you need to put your password:

The Cmd must do nothing else.

---
### Step 3 - Install the Nekoray proxy

1. Create new proxy in Nekoray
   1. Click on Server > New profile
      1. Set these configurations:
         1. Choose SOCKS5 type
         2. Set a name for your proxy
         3. Server: 127.0.0.1
         4. Port: 4002
         5. Save the proxy

2. Start proxy:
   1. Right click on the proxy and click start
   2. Click on VPN Mode at the top of the page

Now you can enjoy the free internet.

---
### Note:
### Each time you want to use this first run the SSH on "Cmd" then Start your "proxy" on Nekoray

