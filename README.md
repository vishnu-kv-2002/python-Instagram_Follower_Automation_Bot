[![Instagram Logo](instagram-logo.png)](https://img.icons8.com/?size=100&id=Xy10Jcu1L2Su&format=png&color=000000)

# Instagram Follower Automation Bot

A Python Selenium automation project that logs into an Instagram-like practice website, visits a target account's followers list, loads additional followers by scrolling, and automatically follows accounts.

> **Note:** This project uses the App Brewery Share-a-Naan practice website for learning and practicing Selenium automation. It is not the live Instagram website and does not interact with real Instagram accounts.

## 🚀 Features

- Automatically opens the practice website.
- Logs into the demo account.
- Handles optional login popups and notification prompts.
- Visits a specified account's followers page.
- Automatically scrolls through the followers list to load more accounts.
- Finds follow buttons within the followers list.
- Clicks follow buttons automatically.
- Handles existing follow states using a Cancel option.

## 🛠️ Technologies Used

- Python
- Selenium WebDriver
- Chrome WebDriver

## ⚙️ Configuration

You can configure the target account in the Python script:

```python
SIMILAR_ACCOUNT = "chefsteps"
```

Store login credentials securely using environment variables instead of hardcoding them.

## 📦 Installation

1. Clone this repository.
2. Install Selenium:

   ```bash
   pip install selenium python-dotenv
   ```
3. Make sure Google Chrome is installed.

## 🔄 How It Works

1. Opens the practice website's login page.
2. Enters the username and password.
3. Handles optional popups.
4. Opens the target account's followers page.
5. Finds the scrollable followers container.
6. Scrolls to the bottom repeatedly to load more followers.
7. Collects the follow buttons displayed in the followers list.
8. Clicks the buttons to follow accounts.
9. Handles click-intercepted situations by cancelling the confirmation dialog.

## 🧠 Concepts Learned

- Browser automation using Selenium
- CSS Selectors and XPath
- Handling dynamic webpage elements
- Scrolling using JavaScript execution
- Using `execute_script()`
- Working with `arguments[0]`
- Handling Selenium exceptions
- Automating login forms
- Finding and interacting with multiple elements
- Python classes and object-oriented programming

## ▶️ How to Run

```bash
python main.py
```

Chrome will open automatically and execute the follower automation workflow.

## 🔮 Future Improvements

- Use explicit waits instead of fixed `time.sleep()`.
- Scroll until no new followers are loaded.
- Track the number of accounts followed.
- Add better exception handling.
- Generate a summary report after execution.

## 👨‍💻 Author

**Vishnu K V**
