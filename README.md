# PWAF (Python Webdriver Automation Framework)

This is web automation framework, implemented using Python & Webdriver. 
Page Object Model (POM) is used to  make the code more readable, maintainable, and reusable.

## _Prerequisite:_

1. Python
2. pip
3. Selenium/WebDriver
4. nosetests & nose-html-reporting
5. Browsers (Firefox, Chrome, IE)
6. Respective Browser drivers
7. Pycharm

### How to run?

**Test scripts can be executed by nosetests:**

>nosetests -s -v --nologcapture <test-script.py>

>e.g: `nosetests -s -v --nologcapture checkbox_page_test.py`

**Execute different group of test:**

>nosetests -s -v --nologcapture  -a group=<group-name> <test-script.py>

>e.g: `nosetests -s -v --nologcapture group=smoke all_tests.py`

**Get Test-reports:**

>nosetests -s -v --nologcapture --with-html --html-report=<test-report-file-path> <test-script.py>

>e.g: `nosetests -s -v --nologcapture --with-html --html-report=test_report.html checkbox_page_test.py`


**_Note:_** Kindly set the respective browser's driver path either to System variable or update it in `drivermanager.py`

e.g: self.driver = webdriver.Firefox(executable_path="geckodriver path") # in case of Firefox browser.
