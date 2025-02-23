# Simulate iPhone Location using Xcode

Easily change your iPhone's location using Xcode's **Simulate Location** feature with a custom GPX file.

## 🚀 Features
- Fake GPS location on iPhone using Xcode.
- No jailbreak or third-party apps required.
- Use custom GPS coordinates from Google Maps.

## 📌 Requirements
- macOS with Xcode installed.
- Apple Developer account (free or paid).
- iPhone with **Developer Mode** enabled.

## 📥 Installation
1. Enable **Developer Mode** on your iPhone:
   - Go to **Settings > Privacy & Security > Developer Mode** and enable it.
2. Connect your iPhone to your Mac and open Xcode.
3. Open **Xcode > Settings > Accounts** and log in with your Apple Developer account.
4. Select your device in **Xcode > Window > Devices and Simulators**.

## 📍 How to Simulate Location in Xcode
### 1️⃣ Create a Custom GPX File
1. Open any text editor and create a new `.gpx` file.
2. Use the following format (replace with your coordinates):

```xml
<?xml version="1.0"?>
<gpx version="1.1" creator="Xcode">
    <wpt lat="37.7749" lon="-122.4194">
        <name>San Francisco</name>
    </wpt>
</gpx>
```

3. Save the file as `custom_location.gpx`.

### 2️⃣ Load the GPX File in Xcode
1. Open your project in Xcode (or create an empty one).
2. Click on **Product > Scheme > Edit Scheme**.
3. Go to the **Run** section and select **Options**.
4. Under **Core Location**, select **GPX File** and choose `custom_location.gpx`.
5. Run your app on your iPhone, and the location will change!

## 📌 Example GPX File
You can download an example GPX file from [here](./custom_location.gpx) or copy the code above.

## ❓ FAQ
**Q: My iPhone is not showing in Xcode. What should I do?**  
A: Make sure Developer Mode is enabled and you have trusted your Mac from the iPhone settings.

**Q: My location is not changing on apps like Google Maps. Why?**  
A: Some apps cache location data. Restart the app or device to see changes.

## 📜 License
This project is licensed under the MIT License.
