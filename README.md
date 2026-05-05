> [See in spanish/Ver en español](https://github.com/LuisMiSanVe/AndroidLLMServerScript/blob/main/README.es.md)
# 📲 Android LLM Server Script
[![image](https://img.shields.io/badge/json-5E5C5C?style=for-the-badge&logo=json&logoColor=white)](https://www.newtonsoft.com/json)
[![image](https://img.shields.io/badge/Visual_Studio_Code-0078D4?style=for-the-badge&logo=visual%20studio%20code&logoColor=white)](https://code.visualstudio.com/)
[![image](https://img.shields.io/badge/Android-3DDC84?style=for-the-badge&logo=android&logoColor=white)](https://developer.android.com/studio)
[![Python](https://img.shields.io/badge/python-3670A0?style=for-the-badge&logo=python&logoColor=ffdd54)](https://www.python.org/)
[![JS](https://img.shields.io/badge/javascript-%23ff8040.svg?style=for-the-badge&logo=JavaScript&logoColor=ffffff)](https://developer.mozilla.org/docs/Web/JavaScript)

Python Script that rises a Localhost LLM server using [llama.cpp](https://github.com/ggml-org/llama.cpp) on Android.

## 📝 Technology Explanation
This script allows you to create a LLM Service using an Android device as Server.

Android `Termux` can't compile `llama-server` due to it lacks of some necessary libraries, this python script makes a workaround by using `llama-simple` instead.

## 🛠️ Setup
In your Android 13+ device (tested), install Termux and run the following commands:

```
pkg update && pkg upgrade
pkg install git cmake clang wget python
```

Then clone and install `llama.cpp` following it's guide.

Get a LLM model suitable for your device.

Then, adapt the Python Script with your folder structure and copy it to your Android device, then run:

```
python server.py
```

Then, your service would be published on your local network and will be listening at the `8000` port by default.

## ⚙️ Project Usage Explanation
In order to test the service, you can use the HTML website client `test.html`, it includes various options and settings to test your local LLM.

## 💻 Technologies Used
- Programming Language: [Python](https://www.python.org/), [JavaScript](https://developer.mozilla.org/docs/Web/JavaScript)
- Tested OS: [Android 13 (MAUI)](https://www.android.com/)
- Libraries: [urllib](https://docs.python.org/es/3/library/urllib.html)
- Other:
    - [llama.cpp](https://github.com/ggml-org/llama.cpp)
    - [Termux](https://f-droid.org/es/packages/com.termux/)
- Recommended IDE: [VS Code](https://code.visualstudio.com/)
