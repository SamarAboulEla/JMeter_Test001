# JMeter_Test001


## TODO list:-

1. In test 3, change how to reference the csv data file (send as a parameter, instead of hard-coding in the jmx file)
2. Add the rest of JMeter tests (requests using varaibles, timestamps, JSON extractor, etc.)

## **Notes:-**
* The following are required for ant build: 'build.xml' and 'ant-jmeter-1.1.1.jar'

## Repo JMeter_Tests files overview:-

* **Test 1:** [1 thread, 1 request] Simple HTTP request to open Google.com 
* **Test 2:** [1 thread, 3 requests] Using regular expression extractor, open APOD, then open html link in the page, then open image in the page
    - Connect to NASA'S API (Astronomy Picture of the Day: APOD) and extract HTML links
    - Open the page for the picture of the day (today) and extract the jpg image
    - Open the page for the jpg image  
* **Test 3:** [n threads, 1 request] Connect to Open Weather Map REST API
    - The request uses an input CSV data file containing cityName & appId    
    - **Required:** add your appId to data file the run the test
    - The maximum number of threads is set to 10.
    - Actual thread count n = min(10, number of rows in the dataset file)


## References:-

1. **[General]** Guide for formatting the repo's readme file:
https://cloudaffaire.com/how-to-write-readme-md-using-markdown/

2. **Performance testing Basics:**
https://www.udemy.com/course/performance-testing-basics/

2. **JMeter for Beginners:**
https://www.udemy.com/course/jmeter-step-by-step-for-beginners/

3. Performance testig using JMeter:
https://www.udemy.com/course/performance-testing-using-apache-jmeter-arabic/

4. Run JMeter from Command-line:
https://www.numpyninja.com/post/run-jmeter-and-generate-html-dashboard-report-from-command-line-non-gui-mode


