# Robot Screenshot Listener

Listener for Automation testing Screenshots with Robot framework-Selenium,Browser and Appium Libraries

## Installation
pip install robotframework-auto-screenshot-listener

## Project Structure

```
Robot Screenshot Listener
├── robotframework_auto_screenshot_listener
│   ├── __init__.py               # Entry point of the application
│   ├── ScreenshotListener.py      # Handles reading and filtering messages
├── requirements.txt           # Lists project dependencies
└── README.md                  # Project documentation
```

**Monitored Selenium Keywords**
   The listener captures screenshots for the following Selenium keywords:
   
   1. Click Element
   2. Input Text
   3. Press Keys
   4. Get Text
   5. Get Element Attribute
   6. Page Should Contain
   7. Page Should Not Contain
   8. Element Should Be Visible
   9. Element Should Not Be Visible
   10. Close Browser
   11. Click Button
   12. Click Link
   13. Click
   14. Fill Text

**How It Works**
   . Test Start: Creates a root directory and test-specific subdirectory
   . Keyword Execution: Before each monitored Selenium keyword, captures a screenshot
   . File Naming: Screenshots are named sequentially (selenium_0.png, selenium_1.png, etc.)
   . Test End: Resets the screenshot counter for the next test

**Technical Details**

Class Structure
   . API Version: Uses Robot Framework Listener API version 2
   . Key Methods:
      . start_test(): Initializes test-specific screenshot directory
      . start_keyword(): Captures screenshots before keyword execution
      . end_keyword(): Handles post-keyword cleanup

Dependencies
   . robot.libraries.BuiltIn: For accessing Robot Framework variables and keywords
   . robot.libraries.String: For string manipulation
   . os: For file system operations
   . shutil: For directory operations



## Usage

   robot --listener robotframework_auto_screenshot_listener.ScreenshotListener:ScreenshotDirectoryName <TestFilePath.robot>

## Contributing

Feel free to submit issues or pull requests if you have suggestions or improvements for the project.

