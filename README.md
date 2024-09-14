<div id="header" align="center">
    <h1>Logging</h1>
    <h3>📝 Logging</h3>
</div>

<div id="badges" align="center">

[![license](https://img.shields.io/github/license/justedlev/logging)](https://github.com/justedlev/logging)
[![stars](https://img.shields.io/github/stars/justedlev/logging)](https://github.com/justedlev/logging/star)
[![issues](https://img.shields.io/github/issues/justedlev/logging)](https://github.com/justedlev/logging/issues)

</div>

## 📋 About

Logging configurations for Java

## 🧾 Example

### Logback

Combined usage with `🍃Spring Boot` logback

```xml
<?xml version="1.0" encoding="UTF-8"?>
<configuration>
    <include resource="org/springframework/boot/logging/logback/defaults.xml" />
    <include resource="io/justedlev/logging/logback/properties.xml"/>
    <include resource="io/justedlev/logging/logback/console-appender.xml" />
    <include resource="io/justedlev/logging/logback/file-appender.xml" />
    <include resource="io/justedlev/logging/logback/debug-file-appender.xml"/>

    <!-- Root Logger Configuration -->
    <root level="DEBUG">
        <appender-ref ref="STDOUT"/>
        <appender-ref ref="FILE"/>
        <appender-ref ref="DEBUG_FILE"/>
    </root>
</configuration>
```
