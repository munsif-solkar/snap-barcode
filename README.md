

# Snap Barcode Scanner | Phone to PC

Snap Barcode is a simple, fast system to scan barcodes using your phone and instantly send the data to your computer/server.

It is designed for real-world use like:
- Mobile shops (like inventory entry)
- Small businesses
- Warehouses
- Personal productivity setups

The system connects your phone (client) to your computer (server) over the same network and lets you scan barcodes directly into your system.

---

## How It Works

 -  You run the **server** on your computer
 -  You open the **client app** on your phone
 - Both devices are connected to the **same WiFi network**
 - You scan a barcode using your phone
 - The data is instantly sent to your computer

---

## Project Structure

This project is split into two repositories:

### 1. Server
👉 https://github.com/munsif-solkar/snap-barcode-server

- Handles incoming barcode data
- Runs locally on your computer
- Can trigger automation (like typing, saving, etc.)

---

### 2. Client
👉 https://github.com/munsif-solkar/snap-barcode-client

- Mobile app
- Uses camera to scan barcodes
- Sends scanned data to server

---





## Installation


### 💻 Windows (Recommended)

1. Go to the **Releases** section of this repository  
2. Download the latest `.exe` release 
3. Launch **Snap Barcode Server**


No additional setup required ✅

---

### 🐧 Linux (Manual Setup)

Since prebuilt binaries are not provided for Linux, follow these steps:

#### 1. Clone the repository
```bash
git clone https://github.com/munsif-solkar/snap-barcode-server
cd snap-barcode-server
```

#### 2. Install dependencies
```bash
npm install
```

#### 3. Run Server
```bash
npm start
```
## Fix for Ubuntu (Typing feature)

If you're using Wayland, switch to X11:

**How to check?**
```bash
echo $XDG_CURRENT_DESKTOP
```
If you see `WAYLAND` in output you need to switch your desktop environment. 

At login screen:

*Click ⚙️ (settings icon)*

Select:
```bash
Ubuntu on Xorg
```
*Then login again.*
