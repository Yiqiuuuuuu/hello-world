# Test - Set Selenium in Node

1. To start with, set up a npm project.
2. Install framework **selenium-webdriver**. <br>Notice: run this command inside my npm project folder!! :no_mouth:
```
npm install selenium-webdriver
```

3. Download browser drivers from [selenium-webdriver](https://www.npmjs.com/package/selenium-webdriver) pages (see the table in the first section) for different browsers. I put all downloaded drivers in D:\workspace\BrowserDrivers.<br>

4. Set the path of the drivers. See my another tech-blog: [Test - How to set PATH variable on Windows10?](https://github.com/Yiqiuuuuuu/tech-blog/blob/master/Test%20-%20Set%20PATH%20variable.md)<br>

5. Try to test to make sure everything is working.
  * Create a new file inside your project directory called google_test.js:
  * Give it the following contents, then save it:<br>
  ```
  var webdriver = require('selenium-webdriver'),
    By = webdriver.By,
    until = webdriver.until;

var driver = new webdriver.Builder()
    .forBrowser('firefox')
    .build();

driver.get('http://www.google.com');
driver.findElement(By.name('q')).sendKeys('webdriver');
driver.findElement(By.name('btnG')).click();

driver.sleep(2000).then(function() {
  driver.getTitle().then(function(title) {
    if(title === 'webdriver - Google Search') {
      console.log('Test passed');
    } else {
      console.log('Test failed');
    }
  });
});

driver.quit();
```






















  
