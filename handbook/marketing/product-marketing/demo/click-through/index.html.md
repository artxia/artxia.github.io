---
layout: markdown_page
title: "Click-through demos"
---

## Summary

This page focuses on how to create click-through demos.


## What is click-through demo

There are certain times when slides, video or other such media just will not do. When you are with a customer or on a trade show stage, a live product demonstration is far superior to slides or videos. Live demos, however, can be fraught with challenges, from technical issues to poor content or delivery. Click-through demos ensure every demo presentation, with groups small or large, is done perfectly every time, eliminating technical and content challenges. Click-through demos are reliable, easy to present and give the audience an absolutely life-like demonstration EVERY TIME.

## Who can create click-through demos

Everyone can download [DemoEasel](https://www.demoeasel.com/download) and record and edit demos, you don't need license to create and edit demos, however, in order to generate demo packages, license is required. The Technical marketing team purchased licenses, the team will be happy to generate packages for you. The priority will be for customer facing demos, which can be reused by other team members.

## Click-through demo consumers in GitLab

Different teams and individuals in GitLab can use it

* New employees - Use it to learn the product.
* SDRs , Solution Architects, SAL, - Deliver GitLab demos to customers.
* Executives - Deliver keynote demos, or deliver demos to executives.
* Field marketing - use click-through demos in trade shows and events.
* Whenever you need to deliver GitLab demo, but you don't have internet access.
* Non-technical users that would like to see how the product works and even present it.


## How to create GitLab click-through demo


### Define the use case

Demos should highlight the value of the product, it should demonstrate how it solves a market challenge. Focusing on features, no matter how they robust, will not be relevant to the customers if they don't understand how it solves their challenges.

To plan a winning demo
* Identify a customer challenge and how GitLab solves this challenge.
* Define a demo flow that shows how we solve this challenges, and how we do it better than our competitors.
* It is recommended to create short demos, up to 20 steps (clicks/screens), demo that you can present in 2 to 5 minutes.


### Prepare your environment

Close all opened windows, keep only Chrome window with GitLab instance opened.
You should have a stable demo flow configured with the right demo data, ready for screen capturing.
Prepare your browser, hide bookmarks and notifications.
Hide OS notifications.
Use the following script to resize Chrome to the required resolution.
Open Script Editor in your MacBook and paste this script to it
```
set theApp to "Google Chrome"
set appHeight to 1080
set appWidth to 1920

tell application "Finder"
set screenResolution to bounds of window of desktop
end tell

set screenWidth to item 3 of screenResolution
set screenHeight to item 4 of screenResolution

tell application theApp
activate
reopen
set yAxis to (screenHeight - appHeight) / 2 as integer
set xAxis to (screenWidth - appWidth) / 2 as integer
set the bounds of the first window to {xAxis, yAxis, appWidth + xAxis, appHeight + yAxis}
end tell
```
Run the script. This will resize your browser to 1080*1920. If necessary, you can modify those parameters in the script for different screen resolution.


### Capture the demo

Download and install [DemoEasel](https://www.demoeasel.com/download).
Open DemoEasel, click **New Demo**, read and follow the tips that presented , then click **Start Capture**. Navigate through your flow. DemoEasel will capture all screens and clicks. To finish recording, click the DemoEasel icon on the bottom dock to bring its UI, then Click **Abstract Demo**.
DemoEasel will automatically recognize the recorded window (Chrome) and will suggest Auto Cropping, accept this option.
Define a name for your demo, click **OK**.


### Edit and Optimize

Once a demo has been captured we can use DemoEasel's editor to optimize and document it so that others can easily present the demo. Select from the demo list the demo you want to edit, click  **Edit the Demo** button.
The editor provides some basic and advanced capabilities. As for the beginning, it is essential for you to get familiar with the following items:
* Red boxes - Make sure all red boxes that automatically added look good, with correct location and size. You can adjust them manually as necessary by dragging them to the right position.
* Edit Note - Add a note for each step, the note describes the step, and specifies where is the next click.
* Review ALL recorded frames, hide unnecessary recorded frames.
* Control the speed of the frames.
* Export / import frames.

For more info, read the **Getting Started.html**  in your DemoEasel folder.

### Package and Share

There are two types of packages we use at GitLab: **browser**(HTML5) and **simulation** (Windows/MacOS executables).
The Technical Marketing produces and upload **browser** demo packages to the [demo page in handbook](https://about.gitlab.com/handbook/marketing/product-marketing/demo/#click-throughs) so employees and customers can learn the product and use cases. Since it supports iPAD, we use the **browser** to demo GitLab in demo booths in events.

For customer facing demos or keynotes, it is recommended to use the **simulation** version as it has better performance and actually gives the audience live demonstration experience.

For transparency, when we present a click-through demo, we announce at the beginning that this is a product simulation, not a live demo.

While everyone can contribute and create click-through demos, we would like to keep on consistency of the messages, ensure demos released in high quality and with the same look and feel, and due to license restrictions, the Technical Marketing team will review the demos, provide feedbacks and will generate the final demo packages for you.

To request the team to review and generate demo packages
* Once you created and completed the demo editing, notes and optimization, Go to ‘_Demos_’ folder under your DemoEasel installation folder, locate a folder with the name of your demo (this folder contains
three files).
* Upload the entire folder to [source files](https://drive.google.com/drive/folders/1tbmY1zg9taLSqH-clJSrcuEcwP2rqMfA?usp=sharing). Set access permissions to anyone in GitLab.
* Open an Issue in [product-marketing](https://gitlab.com/gitlab-com/marketing/product-marketing/issues/new?issue%5Bassignee_id%5D=&issue%5Bmilestone_id%5D=), select **TMM_Support_request** template. Add the following title: "Click-through demo support". In the description, describe the customer challenge and the solution you demonstrate in the demo. Include the path of your demo files you uploaded.

The team will review the demo and might have some improvement suggestions. Once the demo will be ready for release, the team will produce demo packages, will provide you a link to it, and will close the Issue.
