# REGEX JAVA [![Build Status](https://travis-ci.org/nomensa/jquery.hide-show.svg)](https://travis-ci.org/nomensa/jquery.hide-show.svg?branch=master)

```java
import java.util.regex.Matcher;
import java.util.regex.Pattern;


public class Main {
	public static void main(String[] args) {
		String mydata = "22/06 Brazil 19:00 Costa Ric";
		Pattern pattern = Pattern.compile("\\s+\\d{2}\\:\\d{2}\\s+");
		Matcher matcher = pattern.matcher(mydata);
		if (matcher.find())
		{
		    System.out.println(matcher.group());
		}
	}
}
```

- Advance

```java
String mydata = "22/06 Brazil 19:00 Costa Ric 14:22 Allo";
Pattern pattern = Pattern.compile("\\s+\\d{2}\\:\\d{2}\\s+");
Matcher matcher = pattern.matcher(mydata);
while(matcher.find())
{
    System.out.println("Result: "+ matcher.group());
}
```

- Test regex by website https://www.regextester.com/
```java
\s+\d{2}\:\d{2}\s+
```

```
22/06 Brazil 19:00 Costa Ric
```
