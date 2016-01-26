= How do I get started developing?

    gem install bundler && bundle
    ruboto setup
    android update sdk
    guard

= How do I build the app?

    rake

= How do I find the Android x86 ip address?

    # in the console (ALT-F1)
    netcfg

= How do I deploy the app?

    adb connect Robo-Android-Development
    adb install -r bin/HelloWorld-debug.apk

= How do I install ruboto core on the device?

    adb connect Robo-Android-Development
    wget http://ruboto.org/downloads/RubotoCore-release-1.0.5.apk
    adb install -r RubotoCore-release-1.0.5.apk

= When I try to run the emualtor I get the error "Error: Failed to create the SD card.". I'm running a x64 System. What can I do?

Your system is missing 32-bit libs:

    sudo apt-get install libstdc++6:i386 libgcc1:i386 zlib1g:i386 libncurses5:i386