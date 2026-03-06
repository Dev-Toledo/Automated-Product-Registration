# 🚀 Automated Product Registration (Python)

Practical project developed during the **Python Intensive Course** by **Hashtag Programação** (an 8-hour focused training divided into 4 days).

## 📋 About the Project

The goal of this project is to automate the repetitive process of registering products into a web-based system. The automation simulates human behavior by opening the browser, logging in, and filling out hundreds of records using an external database.

### Automation Workflow:
1. **System Access:** Opens the web browser and navigates to the system's URL.
2. **Authentication:** Automatically fills in credentials and logs in.
3. **Data Processing:** Reads a `.csv` file containing the product list.
4. **Registration Loop:** Fills in all required fields (Code, Brand, Type, Category, Price, Cost, and Notes) and submits the data.
5. **Exception Handling:** Checks for empty "Notes" (NaN values) before attempting to type them.

---

## 🛠️ Technologies Used

* **Python 3**
* **PyAutoGUI:** For graphical user interface (GUI) automation (mouse and keyboard control).
* **Pandas:** For database manipulation and analysis.
* **Time:** To manage synchronization and system loading pauses.

---

## ⚙️ How to Install and Run

To run this project on your machine (Windows/Mac), follow the steps below:

### 1. Prerequisites
Make sure you have [Python](https://www.python.org/downloads/) installed on your computer. During installation on Windows, ensure the **"Add Python to PATH"** option is checked.

### 2. Set Up the Environment
Open your terminal or command prompt (cmd/PowerShell) in the project folder and run the following commands:

```bash
# (Optional but recommended) Create and activate a virtual environment
python -m venv venv
venv\Scripts\activate

# Install required Python packages
pip install pyautogui pandas
```
### 3. Execution
Ensure that the produtos.csv file is in the same folder as your script, then run:
```bash
python your_script_name.py
```
---

## ⚠️ Important Notes & Adjustments

* **Screen Coordinates:** The script uses fixed coordinates like pyautogui.click(x=685, y=451). Since these coordinates vary depending on your monitor's resolution and scaling settings, you will need to recalibrate the click points for your specific screen before running the script.

* **Fail-Safe:** To abort the execution in case of an emergency or if the bot loses control, quickly drag your mouse pointer to the top-left corner of your screen.

* **Execution Speed:** The pyautogui.PAUSE = 0.3 command adds a small delay between each action to ensure the system has time to process the inputs. Adjust this value depending on your computer's speed and internet connection.

---

## 🎓 Credits
Project developed as part of the educational material provided by Hashtag Programação.
