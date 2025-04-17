---
label: "Custom Domain"
icon: link
---
# How you can connect a domain to SunLicense?
Super easy! Here's the tutorial:

!!!
You'll need Cloudflare in order to follow this tutorial.
!!!

# 📜 How to connect a Domain with SunLicense
## 🚇 Step 1: Create a Tunnel on [Zero Trust](<https://one.dash.cloudflare.com/>)
1. Go on the **Zero Trust** website
2. Go to the **Networks tab** → then click on **Tunnels**

## ⚙️ Step 2: Connect the Tunnel with your machine
3. Click on **`+ Create Tunnel`** → select **Cloudflared**
4. **Name** your Tunnel _(e.g. SunLicense)_
5. You’ll now see **2 commands** – execute __both__, unless **Cloudflared** is already installed _(then only the 2nd one)_

## 🌞 Step 3: Connect the Tunnel with SunLicense
6. Once you see **1 connector active**, click Next
7. In the `Subdomain` field, type e.g. `license` _(or any other subdomain you want)_
8. Next to it you can select the **domain** you want
9. In the `Type` field, choose `HTTP` ___(not `HTTP`**`S`**)___
10. Next to it, in the **URL** field, type `localhost:PORT` ___**(change the port to the port of SunLicense)**___

## ✅ Done!
SunLicense is now accessible via. https://license.yourdomain.com/ _(with automatic SSL from Zero Trust / Cloudflare)
