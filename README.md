Android project sample structure
================================

Android Sample structure for hierarchical projects with library with very DRY gradle.

The purpose is to simplify the onboarding of new developers.



    git clone git@github.com:retospect/sampleStructure.git
    cp local.properties.sample local.properties
(fix local.properties to point to your sdk)

Then either

    ./gradlew installDebug

or 

open it in AndroidStudio.

Known errors and solutions
==========================

Error:

    > Ambiguous method overloading for method java.io.File#<init>.
      Cannot resolve which method to invoke for [null, class java.lang.String] due to overlapping prototypes between:
          [class java.lang.String, class java.lang.String]
          [class java.io.File, class java.lang.String]

Fix:

Create/update local.properties file, or open Android Studio to do it for you. It should contain one line that refers to the sdk, like

    sdk.dir=/Applications/AndroidStudio.app/sdk

