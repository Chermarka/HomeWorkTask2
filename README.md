<<<Test Case #1>>>

package ua.Epam;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;




public class FirstTest {
    @Test
    public void firstTest() throws InterruptedException {
        System.setProperty("webdriver.gecko.driver", "D:\\geckodriver.exe");
        FirefoxDriver driver = new FirefoxDriver();
        driver.get("https://www.training.by");
        driver.manage().window().maximize();
        Thread.sleep(5000);

        WebElement SignInButton = driver.findElement(By.className("header-auth__signin-icon"));
        SignInButton.click();

        WebElement EmailInput = driver.findElement(By.id("signInEmail"));
        EmailInput.click();
        EmailInput.sendKeys("chermarka@gmail.com");

        WebElement PasswordInput = driver.findElement(By.id("signInPassword"));
        PasswordInput.click();
        PasswordInput.sendKeys("Gameloft1");

        WebElement SignInToSystem = driver.findElement(By.className("popup-reg-sign-in-form__sign-in"));
        SignInToSystem.click();

        driver.quit();

    }
}

<<<Test Case#2>>>

package ua.Epam;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;




public class FirstTest {
    @Test
    public void firstTest() throws InterruptedException {
        System.setProperty("webdriver.gecko.driver", "D:\\geckodriver.exe");
        FirefoxDriver driver = new FirefoxDriver();
        driver.get("https://www.training.by");
        driver.manage().window().maximize();
        Thread.sleep(5000);

        WebElement SignInButton = driver.findElement(By.className("header-auth__signin-icon"));
        SignInButton.click();

        WebElement EmailInput = driver.findElement(By.id("signInEmail"));
        EmailInput.click();
        EmailInput.sendKeys("cherNEmarka@gmail.com");

        WebElement PasswordInput = driver.findElement(By.id("signInPassword"));
        PasswordInput.click();
        PasswordInput.sendKeys("Baldezh");

        WebElement SignInToSystem = driver.findElement(By.className("popup-reg-sign-in-form__sign-in"));
        SignInToSystem.click();

        driver.quit();


    }
}


<<<Test Case #3>>>

package ua.Epam;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.JavascriptExecutor;
import org.openqa.selenium.firefox.FirefoxDriver;




public class FirstTest {
    @Test
    public void firstTest() throws InterruptedException {
        System.setProperty("webdriver.gecko.driver", "D:\\geckodriver.exe");
        FirefoxDriver driver = new FirefoxDriver();
        driver.get("https://www.training.by");
        driver.manage().window().maximize();
        Thread.sleep(5000);
        /*WebElement SignInButton = driver.findElement(By.className("header-auth__signin-icon"));
        SignInButton.click();

        WebElement EmailInput = driver.findElement(By.id("#signInEmail"));
        EmailInput.click();
        EmailInput.sendKeys("chermarka@gmail.com");

        WebElement PasswordInput = driver.findElement(By.id("signInPassword"));
        PasswordInput.click();
        PasswordInput.sendKeys("Gameloft1");

        WebElement SignInToSystem = driver.findElement(By.className("popup-reg-sign-in-form__sign-in"));
        SignInToSystem.click(); */

        WebElement TrainingList = driver.findElement(By.xpath("/html/body/div[1]/header/div/nav/ul/a[1]"));
        TrainingList.click();

        JavascriptExecutor JSE = (JavascriptExecutor) driver;
        JSE.executeScript("window.scrollBy(0, 500);");

        WebElement Search = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/form/input"));
        Search.click();

        WebElement SkillNavigation = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/div[2]/div[1]/div[2]"));
        SkillNavigation.click();

        WebElement TextInput = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/form"));
        TextInput.click();
        TextInput.sendKeys("Java");

        WebElement JavaCheckmark = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/div[2]/div[2]/div[2]/div/div[1]/ul/li[14]/label/span"));
        JavaCheckmark.click();

        WebElement CollapseInputArrow = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/div[1]"));
        CollapseInputArrow.click();

        WebElement ClearSkillJava = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[3]/div/div[2]/div/span/span"));
        ClearSkillJava.click();

        TextInput.click();
        TextInput.sendKeys("DATA");

        List <WebElement> DataCheckmark = driver.findElement(By.cssSelector(".our-skills"));
        for (WebElement DataCherckmarks : DataCheckmark) {
            DataCheckmark.click();
        }

        CollapseInputArrow.click();
        WebElement ClearSkillData = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[3]/div/div[1]/span"));
        ClearSkillData.click();
        TextInput.click();
        TextInput.sendKeys("Pascal");

        driver.quit();

    }
}

<<<Test Case #4>>>

package ua.Epam;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.firefox.FirefoxDriver;

public class FirstTest {
    @Test
    public void firstTest() throws InterruptedException {
        System.setProperty("webdriver.gecko.driver", "D:\\geckodriver.exe");
        FirefoxDriver driver = new FirefoxDriver();
        driver.get("https://www.training.by");
        driver.manage().window().maximize();
        Thread.sleep(5000);

        WebElement SignInButton = driver.findElement(By.className("header-auth__signin-icon"));
        SignInButton.click();

        WebElement EmailInput = driver.findElement(By.id("signInEmail"));
        EmailInput.click();
        EmailInput.sendKeys("chermarka@gmail.com");

        WebElement PasswordInput = driver.findElement(By.id("signInPassword"));
        PasswordInput.click();
        PasswordInput.sendKeys("Gameloft1"); 

        WebElement NewsLink = driver.findElement(By.xpath("/html/body/div[1]/header/div/nav/ul/a[3]"));
        NewsLink.click();


        WebElement News = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/div[3]/section/div[1]/div/div[2]/news-categories/div/div/div[1]/span"));
        if(News == null){
            System.out.println("The News link is absent");
        }
        
        WebElement SuccessStories = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/div[3]/section/div[1]/div/div[2]/news-categories/div/div/div[2]/span"));
        if(SuccessStories == null){
            System.out.println("The Success Stories link is absent");
        }
       
        WebElement Materials = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/div[3]/section/div[1]/div/div[2]/news-categories/div/div/div[3]/span"));
        String MaterialsString = Materials.getText();
        if(Materials == null){
            System.out.println("The Materias link is absent");
        }
        
        WebElement Video = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/div[3]/section/div[1]/div/div[2]/news-categories/div/div/div[4]/span"));
        if(Video == null){
            System.out.println("The Video link is absent");
        }
        
        Materials.click();
        driver.quit();

    }
}

<<<Test Case #5>>>
package ua.Epam;
import org.junit.Test;
import org.openqa.selenium.By;
import org.openqa.selenium.WebElement;
import org.openqa.selenium.JavascriptExecutor;
import org.openqa.selenium.firefox.FirefoxDriver;




public class FirstTest {
    @Test
    public void firstTest() throws InterruptedException {
        System.setProperty("webdriver.gecko.driver", "D:\\geckodriver.exe");
        FirefoxDriver driver = new FirefoxDriver();
        driver.get("https://www.training.by");
        driver.manage().window().maximize();
        Thread.sleep(5000);

        WebElement SignInButton = driver.findElement(By.className("header-auth__signin-icon"));
        SignInButton.click();

        WebElement EmailInput = driver.findElement(By.id("signInEmail"));
        EmailInput.click();
        EmailInput.sendKeys("chermarka@gmail.com");

        WebElement PasswordInput = driver.findElement(By.id("signInPassword"));
        PasswordInput.click();
        PasswordInput.sendKeys("Gameloft1");

        WebElement SignInToSystem = driver.findElement(By.className("popup-reg-sign-in-form__sign-in"));
        SignInToSystem.click();

        WebElement TrainingList = driver.findElement(By.xpath("/html/body/div[1]/header/div/nav/ul/a[1]"));
        TrainingList.click();

        JavascriptExecutor JSE = (JavascriptExecutor) driver;
        JSE.executeScript("window.scrollBy(0, 500);");

        WebElement Search = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/form/input"));
        Search.click();

        WebElement LocationNavigation = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/div[2]/div[1]/div[1]"));
        LocationNavigation.click();

        WebElement ChooseCountry = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/div[2]/div[2]/div[1]/div/div[1]/ul/li[6]/div"));
        ChooseCountry.click();

        WebElement CheckmarkCity = driver.findElement(By.xpath("/html/body/div[1]/div[2]/div/ui-view/div/section[3]/div/div[2]/div[1]/div[2]/div[2]/div[1]/div/div[2]/ul/li[4]/label/span"));
        CheckmarkCity.click();
        
        driver.quit();

    }
}
