# Yahoomail

package testing;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.openqa.selenium.firefox.FirefoxDriver;

public class Sample {

	public static void main(String[] args) {
		// TODO Auto-generated method stub
		WebDriver driver=new FirefoxDriver();
		driver.get("https://edit.europe.yahoo.com/registration");
		driver.manage().window().maximize();
		driver.findElement(By.id("first-name")).sendKeys("Praveen");
		driver.findElement(By.id("last-name")).sendKeys("Nair");
		driver.findElement(By.id("user-name")).sendKeys("praveenmnair2103");
		driver.findElement(By.id("password")).sendKeys("march21@world");
		driver.findElement(By.id("mobile")).sendKeys("7373711753");
		driver.findElement(By.id("male")).click();
    driver.close();
    
	}

}
