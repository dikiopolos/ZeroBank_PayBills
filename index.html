package tests;

import java.util.concurrent.TimeUnit;

import org.openqa.selenium.By;
import org.openqa.selenium.WebDriver;
import org.testng.annotations.AfterMethod;
import org.testng.annotations.BeforeMethod;
import org.testng.annotations.Test;

public class ZeroBank_PayBills {
	
	WebDriver driver;
	String login = "username";
	String password = "password";
	String numAmt = "65";
	String alphaAmt = "gazillion";
	String expDate = "2019-07-12";
	String expPaymentConf = "The payment was successfully submitted.";
	String description1 = "Test date";
	String payeeName = "PG&E";
	String payeeAddress = "8765 Sunset Blvd.\r\nLos Angeles, CA 90201\r\n\r\nOrange County\r\nUSA";
	String acctType = "Electric";
	String acctID = "E876123-H65";
	String pcAmt = "1000";
	
	@Test
	public void ZeroBank_PayBills() {
		
		// SIGN-IN 
		driver.findElement(By.xpath("(//div[contains(.,'Online Banking')])[7]")).click();
		driver.findElement(By.id("signin_button")).click();
		driver.findElement(By.id("user_login")).sendKeys(login);
		driver.findElement(By.id("user_password")).sendKeys(password);
		driver.findElement(By.id("user_remember_me")).click();
		driver.findElement(By.name("submit")).click();
		
		// PAY BILLS
		driver.findElement(By.id("pay_bills_tab")).click();
		driver.findElement(By.id("sp_payee")).click();
		driver.findElement(By.xpath("//option[@value='bofa']")).click();
		driver.findElement(By.id("sp_account")).click();
		driver.findElement(By.xpath("//option[@value='5']")).click();
		
		// MAKE PAYMENT TO EXISTING PAYEE
		driver.findElement(By.id("sp_amount")).sendKeys(numAmt);
		driver.findElement(By.id("sp_date")).click();
		driver.findElement(By.xpath("//span[contains(.,'Next')]")).click();
		driver.findElement(By.xpath("//a[contains(.,'12')]")).click();
		driver.findElement(By.id("sp_description")).sendKeys(description1);
		driver.findElement(By.id("pay_saved_payees")).click();
		
		// Get Payment Confirmation
		String actPaymentConf = driver.findElement(By.xpath("(//div[contains(.,'The payment was successfully submitted.')])[8]")).getText();
		if (actPaymentConf.equals(expPaymentConf)) {
			System.out.println("CONFIRMATION: " + actPaymentConf);
		} else {
			System.out.println("TEST FAILED");
		}
		
		// Test Required Fields
		
		
		// ADD NEW PAYEE
		driver.findElement(By.xpath("//a[contains(.,'Add New Payee')]")).click();
		driver.findElement(By.id("np_new_payee_name")).sendKeys(payeeName);
		driver.findElement(By.id("np_new_payee_address")).sendKeys(payeeAddress);
		driver.findElement(By.id("np_new_payee_account")).sendKeys(acctType);
		driver.findElement(By.id("np_new_payee_details")).sendKeys(acctID);
		driver.findElement(By.id("add_new_payee")).click();
		
		String addPayeeConf = driver.findElement(By.xpath("//div[@id='alert_content']")).getText();
		System.out.println("CONFIRMATION: " + addPayeeConf);
		driver.findElement(By.xpath("//button[contains(.,'×')]")).click();
		
		// PURCHASE FOREIGN CURRENCY
		driver.findElement(By.xpath("//a[contains(.,'Purchase Foreign Currency')]")).click();
		driver.findElement(By.id("pc_currency")).click();
		driver.findElement(By.xpath("//option[@value='NZD']")).click();
		driver.findElement(By.id("pc_amount")).sendKeys(pcAmt);
		
		driver.findElement(By.id("pc_inDollars_true")).click();
		driver.findElement(By.id("pc_calculate_costs")).click();
		String convertFromUSD = driver.findElement(By.xpath("//label[@id='pc_conversion_amount']")).getText();
		System.out.println("Conversion Amt in USD " + convertFromUSD);
		
		driver.manage().timeouts().implicitlyWait(4, TimeUnit.SECONDS);
		
		driver.findElement(By.id("pc_inDollars_false")).click();
		driver.findElement(By.id("pc_calculate_costs")).click();
		String convertToUSD = driver.findElement(By.xpath("//label[@id='pc_conversion_amount']")).getText();
		System.out.println("Conversion Amt in FXCur " + convertToUSD);
		
		driver.findElement(By.id("purchase_cash")).click();
		String buyFX = driver.findElement(By.xpath("//div[@id='alert_content']")).getText();
		System.out.println("CONFIRMATION: " + buyFX);
		
		
	}
	
	
	@BeforeMethod
	public void setUp() {
		driver = utilities.DriverFactory.open("firefox");
		driver.manage().timeouts().implicitlyWait(7, TimeUnit.SECONDS);
		driver.get("http://zero.webappsecurity.com/index.html");
	}
	
	
	@AfterMethod
	public void tearDown() {
//		driver.quit();
	}

}
