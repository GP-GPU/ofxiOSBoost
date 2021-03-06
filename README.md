#ofxiOSBoost for Boost 1.57.0  ![image](https://travis-ci.org/danoli3/ofxiOSBoost.svg?branch=master)
=====================================


### Boost C++ Libraries 1.57.0 Pre-compiled for iOS
![image](https://github.com/danoli3/ofxiOSBoost/blob/master/ofxaddons_thumbnail.png)

- Addon with Boost 1.57.0 for iOS / Xcode 
- Precompiled library and Command to build yourself
- Master is currently a Fat Lib of All Standard Architectures
- Check Branches for others or to be specific 
- Designed for use as an open frameworks addon, however should definitely work for other iOS projects
- Built with clang++ and using libc++ and std=c++11
- License: See Boost License [LICENSE.MD](https://github.com/danoli3/ofxiOSBoost/blob/master/LICENSE.md)

============


### Where to checkout?

- For openframeworks: Checkout in the addons folder like so: addons/ofxiOSBoost
- For others: anywhere you please



============

### How To Link to an Xcode Project?

In Xcode Build Settings for your project:

- Add to Library Search Paths ( ```LIBRARY_SEARCH_PATHS``` ) ```$(SRCROOT)/../../../addons/ofxiOSBoost/libs/boost/lib/ios ```
- Add to Header Search Paths ( ```HEADER_SEARCH_PATHS``` )  
```$(SRCROOT)/../../../addons/ofxiOSBoost/libs/boost/include ```

In the Target under Build Phases
- Add to 'Link Binary With Libraries' the ```boost.a``` found in the ```ofxiOSBoost/libs/boost/lib/ios``` directory.

If not openFrameworks just add the ``` libs/boost/include ``` to Header Search Paths and the  ``` libs/boost/ios ``` to Library Search Paths



============

### Architectures in Pre-Build Library (Fat Lib)
See the other branches on this repository (All libc++ std=c11)

- ```arm64``` : (iOS 7, 8 64bit only) [iPhone 5S, iPhone 6, iPhone 6 Plus, iPad Air]
- ```armv7``` : (iOS 5, 6, 7, 8) [All devices]
- ```i386``` : (iOS Simulator iPad 2, 3, 4, iPhone 4S, 5, 5C)
- ```x86_64```: (iOS Simulator iPad Air, iPhone 5S, iPhone 6, iPhone 6 Plus)

Check Apple's Hardware sheet if you need to verify: [Apple's Device compatibilty Matrix](https://developer.apple.com/library/ios/documentation/DeviceInformation/Reference/iOSDeviceCompatibility/DeviceCompatibilityMatrix/DeviceCompatibilityMatrix.html)

** Armv7s has been removed due to Apple phasing our the requirement from the STANDARD_ARCHITECTURES.


============

### How to Build?

1. You don't need to. This has the pre-compiled versions of BOOST for you to use
2. If you would prefer to build it yourself checkout the script included in the ``` scripts ``` directory.


=============

### How to use Build Script


- Download files (suggested you download the files to addons/ofxiOSBoost for openFrameworks)
- Double click and run ```scripts/build-libc++.command``` (this will download the 1.57.0 version of boost and begin compiling the library).
- Once completed in the terminal continue with the next steps.
- Add the ofxiOSBoost to your project (src and libs for your chosen architecture)`

#### Alternative Build Script:
- Build using libstdc++ by running the ```scripts/build-libstdc++.command```

#### Clean script
- Run the clean script from ```scripts/cleanAll.command``` to remove pre-compiled code and the final built library


============

#### Documentation on Boost 1.57.0


See: http://www.boost.org/users/history/version_1_57_0.html


### Version 1.57.0 (Date): 24th November 2014

