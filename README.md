# 🌱 Grass Bot Auto Farming Guide  
**Join our Telegram community for updates and support:** [@shadowscripters](https://t.me/shadowscripters)  

---

## 📥 Registration & Setup  

### 1. Register on Grass  
Sign up using this referral link: [Grass App Registration](https://app.getgrass.io/register?referralCode=Qj0nK0iL4SRgIT8).  

### 2. Install Python 3.10  
It is recommended to use Python 3.10. [Download it here](https://www.python.org/downloads/release/python-3100/).  

### 3. Dashboard Status  
Grass Dashboard may display errors (as confirmed by the Grass team on Discord), but **points will accumulate correctly.**  

---

## 🛠️ Requirements & Installation  

### Setting Up the Environment  
Run the following commands in your terminal:  

```bash
git clone https://github.com/ShadowScripts1/freeproxygrass.git
cd freeproxygrass
pip install -r requirements.txt
```

### Running the Bot  

#### **Using Free Proxies (Default Option)**  
```bash
python grass_freeproxy.py
```
This script assigns free proxies automatically using the **Proxyscrape API**.  

#### **Using Personal Proxies**  
```bash
python grass_proxy.py
```  

---

## 🔍 How to Retrieve Your Grass User ID  

### For Desktop Browsers  
1. **Log in** to the Grass web app.  
2. Open **Developer Tools**:  
   - Right-click anywhere on the page and select **Inspect**, or press `F12`.  
3. Navigate to the **Console** tab and paste the following code:  
   ```javascript
   localStorage.getItem('userId')
   ```  
   If pasting doesn’t work, type `allow pasting` in the Console, press Enter, and then paste the code above again.  

---

### For Android Users  

#### Retrieve User ID on Android  
1. Install [Kiwi Browser](https://play.google.com/store/apps/details?id=com.kiwibrowser.browser&hl=en).  
2. Log in to the Grass web app and open the Dashboard.  
3. Open **Developer Tools** in Kiwi Browser.  
4. Go to the **Console** tab and paste this code:  
   ```javascript
   localStorage.getItem('userId')
   ```  
   If pasting is blocked, type `allow pasting`, press Enter, then paste the code above.  

---

## Configure Termux  

1. Download and install **Termux** from the [Google Play Store](https://play.google.com/store).  
2. Allow storage permission for Termux by running the following command:  
   ```bash
   termux-setup-storage
   ```  

#### Install Python 3.10 on Termux  
Run the commands below:  
```bash
pkg update && pkg upgrade
pkg install tur-repo
pkg install python-is-python3.10
pkg install -y rust binutils
CARGO_BUILD_TARGET="$(rustc -Vv | grep "host" | awk '{print $2}')" pip install maturin
```  

---

💬 **Need Help?**  
Feel free to reach out to our community on Telegram: [@shadowscripters](https://t.me/shadowscripters)  

--- 

