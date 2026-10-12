# Expense Tracker

Expense Tracker is a simple Android application for tracking personal expenses. It helps users record their daily spending and see where their money goes.

## Functionality

- User can add a new expense.
- User can edit an existing expense.
- User can delete an expense.
- User can view a list of all expenses.
- User can select an expense category.
- User can enter the date and amount of an expense.
- User can view the total amount of expenses.
- App saves expenses locally on the device.

## Project Structure
Структура папок тома Windows   
Серийный номер тома: 00000033 2CA1:73FB
C:.
│   .gitignore
│   build.gradle.kts
│   gradle.properties
│   gradlew
│   gradlew.bat
│   local.properties
│   README.md
│   settings.gradle.kts
│   
├───.gradle
│   ├───9.6.0
│   │   │   gc.properties
│   │   │   
│   │   ├───checksums
│   │   │       checksums.lock
│   │   │       md5-checksums.bin
│   │   │       sha1-checksums.bin
│   │   │       
│   │   ├───executionHistory
│   │   │       executionHistory.lock
│   │   │       
│   │   ├───expanded
│   │   ├───fileChanges
│   │   │       last-build.bin
│   │   │       
│   │   ├───fileHashes
│   │   │       fileHashes.bin
│   │   │       fileHashes.lock
│   │   │       resourceHashesCache.bin
│   │   │       
│   │   ├───kotlin-dsl-plugin-entries
│   │   │       jar-entries.bin
│   │   │       kotlin-dsl-plugin-entries.lock
│   │   │       
│   │   └───vcsMetadata
│   ├───buildOutputCleanup
│   │       buildOutputCleanup.lock
│   │       cache.properties
│   │       
│   └───vcs-1
│           gc.properties
│           
├───.idea
│       .gitignore
│       workspace.xml
│       
├───app
│   │   .gitignore
│   │   build.gradle.kts
│   │   
│   └───src
│       ├───androidTest
│       │   └───java
│       │       └───com
│       │           └───example
│       │               └───expensetracker
│       │                       ExampleInstrumentedTest.kt
│       │                       
│       ├───main
│       │   │   AndroidManifest.xml
│       │   │   
│       │   ├───java
│       │   │   └───com
│       │   │       └───example
│       │   │           └───expensetracker
│       │   │               │   MainActivity.kt
│       │   │               │   
│       │   │               └───ui
│       │   │                   └───theme
│       │   │                           Color.kt
│       │   │                           Theme.kt
│       │   │                           Type.kt
│       │   │                           
│       │   ├───keepRules
│       │   │       rules.keep
│       │   │       
│       │   └───res
│       │       ├───drawable
│       │       │       ic_launcher_background.xml
│       │       │       ic_launcher_foreground.xml
│       │       │       
│       │       ├───mipmap-anydpi-v26
│       │       │       ic_launcher.xml
│       │       │       ic_launcher_round.xml
│       │       │       
│       │       ├───mipmap-hdpi
│       │       │       ic_launcher.webp
│       │       │       ic_launcher_round.webp
│       │       │       
│       │       ├───mipmap-mdpi
│       │       │       ic_launcher.webp
│       │       │       ic_launcher_round.webp
│       │       │       
│       │       ├───mipmap-xhdpi
│       │       │       ic_launcher.webp
│       │       │       ic_launcher_round.webp
│       │       │       
│       │       ├───mipmap-xxhdpi
│       │       │       ic_launcher.webp
│       │       │       ic_launcher_round.webp
│       │       │       
│       │       ├───mipmap-xxxhdpi
│       │       │       ic_launcher.webp
│       │       │       ic_launcher_round.webp
│       │       │       
│       │       ├───values
│       │       │       colors.xml
│       │       │       strings.xml
│       │       │       themes.xml
│       │       │       
│       │       └───xml
│       │               backup_rules.xml
│       │               data_extraction_rules.xml
│       │               
│       └───test
│           └───java
│               └───com
│                   └───example
│                       └───expensetracker
│                               ExampleUnitTest.kt
│                               
└───gradle
│   gradle-daemon-jvm.properties
│   libs.versions.toml
│   
└───wrapper
gradle-wrapper.jar
gradle-wrapper.properties