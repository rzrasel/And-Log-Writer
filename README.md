# And-Log-Writer
And Log Writer

### GIT Command
```git_command
git init
git remote add origin https://github.com/rzrasel/And-Log-Writer.git
git remote -v
git fetch && git checkout master
git add .
git commit -m "Add Readme & Git Commit File"
git pull
git push --all
```

[ ![Download](https://api.bintray.com/packages/rzrasel/CommonLibraries/fine-log-writer/images/download.svg?version=100.00.01) ](https://bintray.com/rzrasel/CommonLibraries/fine-log-writer/100.00.01/link)

Download
--------

Download the latest JAR or grab via Maven:
```xml
<dependency>
	<groupId>com.adept.coffeelab</groupId>
	<artifactId>log-writer</artifactId>
	<version>100.00.01</version>
	<type>pom</type>
</dependency>
```
or Gradle:
```groovy
implementation 'com.adept.coffeelab:log-writer:100.00.01'
```

Usage
-----

In your Activity

```java
import android.app.Activity;
import android.content.Context;
import android.support.v7.app.AppCompatActivity;
import android.os.Bundle;

import rz.logwriter.LogWriter;

public class ActSplash extends AppCompatActivity {
    private Activity activity;
    private Context context;

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.act_splash);
        activity = this;
        context = this;
        LogWriter.Log("Test Log");
    }
}
```