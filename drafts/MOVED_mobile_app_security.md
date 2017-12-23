\[FUTURE EDITS IN GITHUB REPO PLEASE\]
======================================

Mobile app security settings
============================

## Overview FIX This is the first short training module in a series of
three trainings dedicated to securing your mobile device. In this
module, participants will learn how to review the security settings on
their mobile devices (for iPhone and Android users). In later trainings,
they will learn how to encrypt their device, set a secure locking
mechanism, and install an encrypted messaging system (Signal). These
three modules are meant to be short, simple, and can be used together to
create a 60- to 75-minute block of training around securing a mobile
device.

**ABOUT THIS LESSON PLAN**

**Review date:** June 5, 2017

**Lesson duration:** 20-30 minutes

**What will participants learn?**

A better understanding of how mobile apps utilize different components
of phones (location services, microphone, camera) and how those
components may be used for more nefarious purposes. Participants will
gain an understanding of the different permission levels that
third-party applications may use, and they will also learn how to change
and edit those settings.

**What materials will participants need?**

Their smartphone (iOS, Android).

**What materials will the instructor need?**

Basic familiarity with both iOS and Android phones and operating
systems.

**Level**

Introductory. This session is for journalists who may not realize how
many permissions they have given to the third-party apps on their phone,
and for those who are not regularly doing good security hygiene on their
devices.

**LESSON PLAN**

**Icebreakers/activities**

Trainer should begin with an overview of why this topic matters. Not all
journalists will realize how their phone components (location services,
microphone, and camera) can be used by third-party apps. Below are
examples of well-known cases of consumer applications using data and
mobile services without average consumers’ knowledge.

**Links in the news**

Uber’s use of riders’ location data and ride history:
[*https://www.buzzfeed.com/bensmith/uber-executive-suggests-digging-up-dirt-on-journalists*](https://www.buzzfeed.com/bensmith/uber-executive-suggests-digging-up-dirt-on-journalists)

Macy’s using shoppers’ location data:
[*http://abcnews.go.com/Technology/retailers-tracking-shoppers-locations-real-world/story?id=47825826*](http://abcnews.go.com/Technology/retailers-tracking-shoppers-locations-real-world/story?id=47825826)

Turn off your Facebook application’s permission to the phone microphone
[*https://qz.com/697923/heres-how-to-stop-facebook-from-listening-to-you-on-your-phone/*](https://qz.com/697923/heres-how-to-stop-facebook-from-listening-to-you-on-your-phone/)

Uber using access to prohibited iOS code to fingerprint devices even
across factory resets:

[*https://arstechnica.com/apple/2017/04/tim-cook-once-slapped-uber-on-the-wrist-for-breaking-the-app-store-rules/*](https://arstechnica.com/apple/2017/04/tim-cook-once-slapped-uber-on-the-wrist-for-breaking-the-app-store-rules/)

**5-minute discussion**

Ask participants to name as many data collection points on their
smartphones as they can (think: gyroscope, compass, microphone, camera,
GPS, barometer, etc). Note which could be used for malicious/nefarious
purposes by a third-party application (Uber using your location to send
a car to you vs. Siri/Alexa listening to you all the time). Use a
whiteboard or giant sticky note if you have one.

Also discuss how apps may utilize hard-coded identifiers that are
required by cellular telecommunications providers, such as a unique
identification for each device (international mobile equipment
identification, IMEI) and unique identifier for each subscriber (SIM
serial number, which is unique to each SIM card). These can be used by
marketing companies or other orgs to track a specific device or
subscriber through multiple apps, regardless of whether the app has been
installed and uninstalled or the entire mobile operating system has been
reinstalled. This concern is primarily associated with Android devices,
which allow apps to request the permission “Device ID and Call
Information.” IOS devices do not allow for IMEI, though it’s still
possible to fingerprint devices using other identifying information.

**Walkthrough or Active Lesson**

Ask participants to break into partner groups for the next exercise. If
they’re comfortable with doing so, each pair will open the settings on
their phones together and review which applications are using location,
microphone, and camera. (If someone wants to review their phone settings
individually, let them know that’s OK.)

While the group is reviewing their privacy settings, it’s a good time to
talk about how and why a seemingly unrelated application may ask for
access to the camera, microphone or location services.

For iPhone users:

-   Open settings, go to Privacy (it’s a small gray icon with a hand)

    -   Location Services: these are applications that have access to
        > your location based on GPS, Bluetooth, wifi hotspots and cell
        > tower locations.

        -   Apps will either have two or three options for this setting:
            > Never, While Using the App, or Always. If “Always” is an
            > option, it means that the application can have access to
            > your location even if you do not have the application open

        -   The app will often have a one-line explanation as to why it
            > is asking for your location. (E.g.: Yelp says, “This app
            > needs your location to search for nearby businesses.”)

        -   A small arrow-shaped icon is used to indicate whether an
            > application has used your location recently or within the
            > past 24 hours

    -   Microphone

        -   Any application that has requested access to the microphone
            > should appear in a list with a set of toggles (the only
            > settings are “on” and “off”)

    -   Camera

        -   Any application that has requested access to the camera will
            > appear in a list with a set of toggles (again, the
            > settings options are “on” and “off”). This includes access
            > to the camera itself, as well as access to the photos
            > stored on your phone.

(*A note for trainers -- this is one section where instructions may
become outdated quickly and often. However, the concepts of checking
location, microphone, and camera access for the reasons outlined above
should hold up).*

For Android users:

**(NOTE TO EVERYONE: this section could use some fleshing out if there
are more Android experts out there--ecg, kg)**

The process of checking application permission settings differs between
Android versions.

\*how to figure out which version you are using

Settings > About Phone (checked on 6.0, 7.0, 5.1.0)

-   Marshmallow (6.0) or later: Open **Settings** / **Apps.** Click the
    > gear icon and open **App Permissions**. A list of permissions will
    > be display including features such as Camera, Location, and
    > Microphone, along with

-   Android versions before 6.0: Open Settings > Apps, select an app,
    > permissions the app uses is displayed

**Screenshot for iPhone users of apps using location services**

![](media/image3.png){width="5.6818186789151355in"
height="10.106060804899387in"}

**Screenshot for Android (6.0 and later) users of an app permissions**

![](media/image4.png){width="4.177083333333333in" height="7.375in"}

**Other similar exisiting/tested curricula: **

-   **https://gitlab.com/ttc/data-privacy-training/blob/4f9a1657770ff0ad8ae27f3c6aaf4196325a692a/content/Workshops/MobilePhoneSettingsHandsOn.md**
