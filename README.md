# Context-Click
How to achive context click  in selenium?

	public static void main(String[] args) throws AWTException, InterruptedException 
	{
		WebDriver driver = new ChromeDriver();
		driver.manage().window().maximize();
		driver.get("...<URL>...");
		WebElement link = driver.findElement(By.linkText("<Text Name>"));
		Actions action = new Actions(driver);
		action.contextClick(link).perform();
	}
