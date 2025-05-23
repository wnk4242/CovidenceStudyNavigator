# Covidence Study Navigator (Tampermonkey Userscript)

This Tampermonkey userscript is designed to streamline the screening process in [Covidence](https://www.covidence.org/), a tool commonly used for literature and systematic reviews. In large reviews, researchers are often assigned to screen a range or a randomized set of studies. Covidence allows users to search for one study at a time, but doesn't support easy navigation through a custom list of study IDs, especially when the study IDs are non-consecutive, or they are not located at the top of the study list.


## Features
The script helps users:
- Embedded draggable panel in the Covidence UI.
- Automatically navigate to each study in the list.
- Make Yes/No/Maybe decisions using built-in buttons on the panel.
- Record and log decisions in real time.
- Export screening decisions as a CSV file for tracking or auditing.
- Click on logged study IDs in a summary section to jump directly to a specific study.

#### Front panel:
![UIx](ui/CSN_UIx.png)

#### Main panel:
![UIxx](ui/CSN_UIxx.png)


## How to Install Tampermonkey and Add This Script

### ✅ Step 1: Add Tampermonkey to Chrome  
1. Go to the [Chrome Web Store](https://chrome.google.com/webstore/) and search for **Tampermonkey**.

![Step 1.1](installation/install_step1.1.png)

2. Click **Add to Chrome** on the extension page.

3. Alternatively, visit [tampermonkey.net](https://www.tampermonkey.net/) and click **Get from Store**.

![Step 1](installation/install_step1.png)  
---

### ✅ Step 2: Pin Tampermonkey to Your Toolbar  
![Step 1.2](installation/install_step1.2.png)  

1. Click the puzzle piece icon (Extensions) in the top-right of Chrome.  
2. Find **Tampermonkey** and click the pin icon to keep it visible in your toolbar.

---

### ✅ Step 3: Open the Tampermonkey Dashboard  
![Step 2](installation/install_step2.png)  

1. Click the **Tampermonkey** icon in your toolbar.  
2. Choose **Dashboard** from the dropdown menu.

---

### ✅ Step 4: Create a New Userscript  
![Step 2.1](installation/install_step2.1.png)  

1. In the dashboard, click the **➕ (plus)** icon at the top right to create a new script.  
2. Delete the default code entirely in the code editor and paste the code in **Covidence Study Navigator-2.0.1.user.js** into the code editor and click **File > Save**.
3. Once saved, the script will automatically run whenever you visit Covidence. You should see a red badge on the Tampermonkey icon showing that your userscript is active and running on the page.

![Step 3](installation/install_step3.png)  






## How to Use the Covidence Study Navigator Userscript



### ✅ Step 1: Export your assigned study list from Covidence  


1. In Covidence, go to your review’s **Export** tab.
2. Under **References**, select:
   - **Options**: `Title and abstract screening`
   - **Format**: `CSV`
3. Click **Prepare file**, then **Download** the CSV.

![Export CSV](use/use_step1.png)
---

### ✅ Step 2: Open the CSV in Excel  


1. Open the downloaded file (e.g., `review_XXXX_screen_csv_XXXX.csv`) in Excel.
2. Find the **Covidence #** column.
3. Select and copy the list of study numbers that are assigned to you (e.g., rows 10 to 19).

![Open CSV](use/use_step2.png)
---

### ✅ Step 3: Paste the study numbers into the Tampermonkey panel  


1. Go to your Covidence review project in Chrome.
2. You should see the Covidence Study Panel on the left (if the script is installed and active).
3. Paste your copied list of study numbers into the input box.
4. Click **Start** to begin screening.

![Paste into panel](use/use_step3.png)
---

### ✅ Step 4: Screen studies using the panel  


1. This userscript will automatically navigate to each study in your list.
2. Click **Maybe**, **Yes**, or **No** in the panel to make your decisions.
3. All decisions are logged in real time and visible in the panel.
4. Click **Export decisions to .csv** at any time to download your screening log.

![Screen from panel](use/use_step4.png)
---

