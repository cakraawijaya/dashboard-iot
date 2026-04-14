[![Open Source Love](https://badges.frapsoft.com/os/v1/open-source.svg?style=flat)](https://github.com/ellerbrock/open-source-badges/)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg?logo=github&color=%23F7DF1E)](https://opensource.org/licenses/MIT)
![GitHub last commit](https://img.shields.io/github/last-commit/cakraawijaya/Dashboard-IoT-Berbasis-Node-JS?logo=Codeforces&logoColor=white&color=%23F7DF1E)
![Project](https://img.shields.io/badge/Project-Website-light.svg?style=flat&logo=googlechrome&logoColor=white&color=%23F7DF1E)
![Type](https://img.shields.io/badge/Type-Workshop%20Assignment-light.svg?style=flat&logo=gitbook&logoColor=white&color=%23F7DF1E)

# Dashboard IoT Berbasis Node.js
This project has high resource efficiency and performance, including real-time data processing, as well as good cybersecurity.

<br>

## Project Requirements
| Part | Description |
| --- | --- |
| Scheme | Virtual |
| Features | • Publish<br>• Subscribe |
| Development Board | DOIT ESP32 DEVKIT V1 |
| Code Editor | Visual Studio Code |
| Application Support | • Wokwi<br>• MQTTX<br>• Node.js |
| MQTT Broker | EMQX Broker |
| Communications Protocol | • Hypertext Transfer Protocol (HTTP)<br>• Message Queuing Telemetry Transport (MQTT) |
| IoT Architecture | 3 Layer |
| Framework | • Bootstrap 5<br>• Express.js<br>• Font-Awesome 6 |
| Libraries | MQTT.js |

<br><br>

## Download & Install
1. Visual Studio Code
   <table><tr><td width="810">

   ```
   https://bit.ly/VScode_Installer
   ```

   </td></tr></table><br>

2. NodeJS
   <table><tr><td width="810">

   ```
   https://nodejs.org/en/download/prebuilt-installer
   ```

   </td></tr></table><br>

3. MQTTX
   <table><tr><td width="810">

   ```
   https://mqttx.app/downloads
   ```

   </td></tr></table>

<br><br>

## Project Designs
<table>
<tr>
<th width="840">Infrastructure</th>
</tr>
<tr>
<td><img src="documentation/diagram/Infrastructure.jpg" alt="infrastructure"></td>
</tr>
</table>

<br><br>

## Get Started
1. Create a new directory named ``` dashboard-iot ```.<br><br>
2. Download and extract this repository.<br><br>
3. Copy the directories: ``` public ``` and ``` views ```.<br><br>
4. Copy the file: ``` server.js ```.<br><br>
5. Paste and Replace into the ``` dashboard-iot ``` directory.<br><br>
6. Open ``` Terminal ``` inside that directory.<br><br>
7. Create a ``` package.json ``` file by typing the command:<br>
   <table><tr><td width="810">
   
   ```bash
   npm init -y
   ```
   
   </td></tr></table>
   <br>
8. Install ``` express ``` to make a backend server:<br>
   <table><tr><td width="810">
      
   ```bash
   npm install express
   ```
   
   </td></tr></table>
   <br>
9. Install ``` mqtt ``` for IoT data communication:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install mqtt
    ```
   
    </td></tr></table>
    <br>
10. Install ``` mqttjs ``` to connect the web and Node.js to the MQTT broker in real time:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install mqttjs
    ```
   
    </td></tr></table>
    <br>
11. Install ``` ejs ``` to create web pages with dynamic content:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install ejs
    ```
   
    </td></tr></table>
    <br>
12. Install ``` bootstrap ``` to manage the appearance (layout):<br>
    <table><tr><td width="810">
      
    ```bash
    npm install bootstrap
    ```
   
    </td></tr></table>
    <br>
13. Install ``` fontawesome ``` for icons:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install @fortawesome/fontawesome-free
    ```
   
    </td></tr></table>
    <br>
14. Open ``` package.json ```, then change the ``` scripts ``` section to look like this:<br>
    <table><tr><td width="810">
      
    ```bash
    "scripts": {
      "start": "node server.js",
      "dev": "nodemon server.js"
    },
    ```
   
    </td></tr></table>
    <br>
15. Install ``` nodemon ``` to restart the server automatically:<br>
    <table><tr><td width="810">
      
    ```bash
    npm install --save-dev nodemon
    ```
   
    </td></tr></table>
    <br>
16. To run the web, type the command:<br>
    <table><tr><td width="810">
      
    ```bash
    npm run dev
    ```
   
    </td></tr></table>
    <br>
17. Open your browser, then type -> ``` http://localhost:3000/ ```.<br><br>
18. Fill in the Topic and Data form first, for example: `kelasiot/pot` | `4095` -> then click `Publish`, then the result will be displayed.<br><br>
19. This port and Topic Subscribe can be changed according to the user's preference. These settings are contained in a file called `server.js`.<br><br>
20. Please access the features and enjoy [Done].

<br><br>

## Simulation With MQTTX
`MQTTX Web` provides 2 communication protocols, namely `WebSocket (WS)` and `WebSocket Secure (WSS)`. There is also `MQTTX Desktop`, which is a more complete option.<br><br>
1. If you are using `MQTTX Web`, make sure to select the `WSS` protocol to be secure.<br><br>
2. If you are using `MQTTX Desktop`, don't forget to download the app. Then, once downloaded, open that application on your laptop or computer.<br><br>
3. Click `+ New Connection` -> then name the connection as you want -> then click `Connect`.<br><br>
4. Create a new topic with the name `kelasiot/pot`.<br><br>
5. Then for topic settings you can customize as seen below:<br><br>
   <table><tr><td width="810">
   • Format Payload to Publish by : &nbsp; <strong>`Plaintext`</strong>.<br><br>
   • Qos : &nbsp; <strong>`0`</strong>.<br><br>
   • Put a check mark on <strong>`Retain`</strong>.
   </td></tr></table><br>
6. Publish data.<br><br>
7. After that, please click `+ New Subscription` -> then list the topics you want to subscribe, for example: `kelasiot/#`.<br><br>
8. Wait for the subscription results to be displayed.<br><br>
9. Have fun and enjoy [Done].

<br><br>

## Deploy on Railway
1. Open the Railway platform:&nbsp;&nbsp;<strong><a href="https://railway.com/">Click Here</a></strong> &nbsp;, then log in with GitHub.<br><br>
2. Allow Railway to access the repository.<br><br>
3. Upload the project to GitHub.<br><br>
4. Log in to the Railway dashboard:&nbsp;&nbsp;<strong><a href="https://railway.com/dashboard">Click Here</a></strong><br><br>
5. Click ``` Add New Project ```.<br><br>
6. Select the desired GitHub repository.<br><br>
7. Select the ``` Settings ``` menu -> Change the ``` Name ``` and ``` Description ``` as needed -> Click the ``` Update ``` button.<br><br>
8. Select the ``` Architecture ``` menu -> Click ``` Project ```.<br><br>
9. Click ``` Variables ``` in the Project section -> Click the ``` New Variable ``` button, then fill it in exactly like this:<br>
   - Placeholder: ``` VARIABLE_NAME ```
       <table><tr><td width="810">
         
       ```bash
       MQTT_BROKER
       ```
      
       </td></tr></table>
       
   - Placeholder: ``` VALUE or ${{REF}} ```
       <table><tr><td width="810">
         
       ```bash
       mqtt://broker.emqx.io
       ```
      
       </td></tr></table>
       <br>
10. Click ``` Settings ``` in the Project section -> Search for ``` Public Networking ``` -> Click the ``` Generate Domain ``` button.<br><br>
11. To get a clean domain:&nbsp;&nbsp;Click ``` Edit ``` -> Click the ``` Update ``` button (*Optional).

<br><br>

## Simulation With Wokwi
Link to simulate : <strong><a href="https://wokwi.com/projects/413253569138415617" target="_blank">Click Here</a></strong>

<br><br>

## Highlights
<table>
<tr>
<th width="420">Dashboard View</th>
<th width="420">Running the Server</th>
</tr>
<tr>
<td><img src="documentation/experiment/Web Dashboard.jpg" alt="dashboard"></td>
<td><img src="documentation/experiment/Running the Server.jpg" alt="server"></td>
</tr>
</table>
<table>
<tr>
<th width="420">MQTTX Simulation</th>
<th width="420">Wokwi Simulation</th>
</tr>
<tr>
<td><img src="documentation/experiment/MQTTX Simulation.jpg" alt="mqttx"></td>
<td><img src="documentation/experiment/Wokwi Simulation.jpg" alt="wokwi"></td>
</tr>
</table>

<br><br>

## Appreciation
If this work is useful to you, then support this work as a form of appreciation to the author by clicking the `⭐Star` button at the top of the repository.

<br><br>

## Disclaimer
This application is the result of the development of the Kelas IoT Workshop. I do not deny that I still use third-party services in this work, including: libraries, frameworks, and so on.

<br><br>

## LICENSE
MIT License - Copyright © 2024 - Devan C. M. Wijaya, S.Kom

Permission is hereby granted without charge to any person obtaining a copy of this software and the software-related documentation files to deal in them without restriction, including without limitation the right to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons receiving the Software to be furnished therewith on the following terms:

The above copyright notice and this permission notice must accompany all copies or substantial portions of the Software.

IN ANY EVENT, THE AUTHOR OR COPYRIGHT HOLDER HEREIN RETAINS FULL OWNERSHIP RIGHTS. THE SOFTWARE IS PROVIDED AS IS, WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESS OR IMPLIED, THEREFORE IF ANY DAMAGE, LOSS, OR OTHERWISE ARISES FROM THE USE OR OTHER DEALINGS IN THE SOFTWARE, THE AUTHOR OR COPYRIGHT HOLDER SHALL NOT BE LIABLE, AS THE USE OF THE SOFTWARE IS NOT COMPELLED AT ALL, SO THE RISK IS YOUR OWN.
