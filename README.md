using OpenQA.Selenium;
using OpenQA.Selenium.Chrome;

class Program
{
    static void Main()
    {
        // Create a new instance of ChromeDriver
        IWebDriver driver = new ChromeDriver();

        // Launch the website
        driver.Url = "https://www.example.com";

        // Find an element on the page by its ID
        IWebElement element = driver.FindElement(By.Id("example-element-id"));

        // Perform an action on the element (e.g., click, type text)
        element.Click();

        // Close the browser
        driver.Quit();
    }
}
