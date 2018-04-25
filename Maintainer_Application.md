# Prerequisites for device maintaining #

## Application procedure ##

* Applicants with history of "conflicts" won't be accepted in any way. You should be aware of this before applying.
* Applicants should drop a message to <strong>one</strong> team member only. The member will forward the message to the reviewers and give you the appropriate contact information for your reviewer. "Spamming" more than one team member will result in an immediate rejection.
* Applicants contacting the reviewers on any other communication platform but <strong>Google Hangouts</strong> will be rejected as they clearly didn't read this!
* Applicants <strong>must</strong> be aware of the fact that the team's language for communicating is ENGLISH.
* <strong>Continued support</strong> will be needed, so ask yourself: <em>"Can/Do I want to provide continuous support?"</em>. AICP is not a "submit & forget" home for buildbots. We don't want people who build numerous custom ROMs. This is not the purpose of maintaining from our point of view. You need to be willing to continue maintaining the device by fixing bugs, applying AOSP security updates and eventually improving performance.
* An application should include links to the device, vendor and kernel trees on GitHub, plus the email address of the applicant. Please be patient once you have sent your application. It takes some time to review your source code. If changes are deemed necessary, you will receive notice for improvement and be able to re-apply after improving.
* Applicants should show some respect towards the reviewer regardless of the decision. Privacy is respected by us, so the applicant is supposed to do this too.
* Applicants <strong>must</strong> use some common sense, mature behavior and politeness, as the team considers that too. Reviewers are not "Bro's" as they are not your family and thus the application will be rejected immediately.
* Applicants should keep in mind <strong>not to bother</strong> any reviewer nor the team for the final results of the application. Reviewers try to judge objective on every application.
* Accepted applicants <strong>must</strong> be active and reachable on our team chat, unless they have given a reason as of why they can't.
* Accepted applicants should also keep in mind that spreading/sharing parts of team internal conversations to anyone for whatever purpose, will result in a ban from the team.


<em>Note: Successfully passing the application for the team also gives you the possibility of opening an "official" DevDB thread on XDA for your device using our <a href="https://raw.githubusercontent.com/AICP/vendor_aicp/o8.1/xda_template/xda_thread-template.txt">XDA template</a>.</em>

---

## Maintainer ##

* Maintainers <strong>must</strong> have an account on Github and Gerrit.
* Maintainers <strong>must</strong> know how to use Gerrit correctly, including the abilities to push / rebase / review / cherrypick commits, the usage of proper topics for related commits or assigning reviewers.
* Maintainers <strong>must</strong> know how to handle Git correctly, including rebasing / merging / pulling or amending to commits as well as cloning and working with repositories.
* Maintainers <strong>must</strong> retain proper authorship on commits or changes including the commit history, when using "picked" commits from other sources. Authorship hereby means the <b>original</b> author should be named (commit history!). As authorship is important for us in the open source community, it is mandatory for pushing to Github or Gerrit.
* Maintainers <strong>must</strong> have some basic knowledge about fixing bugs and pulling logs (on device and/or via ADB).


---

## Device ##

* The device <strong>must</strong> be buildable by using open sourced dependencies that have a valid commit history. Preferably using LineageOS dependencies (incl. vendor) when possible.
* The device <strong>must</strong> have an official or at least trustable recovery (TWRP preferably) working and publicly available.
* The device <strong>must</strong> enforce SELinux before going official. If not possible at the moment of adding, it will stay in beta stage until SELinux can be enforced.
* The kernel <strong>must</strong> use LineageOS kernel sources or needs to be upstreamed including the latest patches from kernel.org. Kernel feature additions <strong>must</strong> be allowed and approved by the team before adding. <em>For example: Overclocking/undervolting apart from the manufacturer's default is not tolerated.</em>
* The device's storage capabilities (internal and/or external) <strong>must</strong> be fully working.
* The device <strong>must</strong> have working audio for phone calls(!) on at least handset, speaker, headset (phone jack) and Bluetooth.
* The device <strong>must</strong> be able to make a data connections via SIM and/or Wifi. If the device has more than one SIM slot, both slots must be working.
* The device <strong>must</strong> have other features for data transfers/communication working, like Bluetooth / NFC / Wifi Hotspot or USB tethering. This is of course dependent on the device's hardware.
* The device <strong>must</strong> have a working camera. This includes front and rear cameras, if applicable. This means that <strong>all</strong> Camera supported features for Photo and Video should be supported and working.
* The device's sensors, including fingerprint / proximity / acceleration / etc., <strong>must</strong> be working.
* The device tree <strong>must</strong> not include any unused overlays, but <strong>must</strong> include the basic overlays to work with AICP/LineageOS features like Live Display, key configs, DUI, pocketmode, doze etc.
* The device tree <strong>can</strong> include device specific overlays and packages, but not any obsolete packages or unnecessary properties (system.prop, vendor.prop, etc.).


<em>Note: Once you and your device have been successfully accepted, you will be given access to our team chat and limited access to our servers for your needed device repositories. Of course you will receive help on maintaining your device and have to coordinate your device with the development of AICP.</em>



## Do you think you still have the guts to tame the beast? ##