---
layout: lab
title: Getting Started Using the Web Console
subtitle: Understanding how to navigate the web console
html_title: Getting started using the web console
categories: [lab, intro, welcome, developers, ops]
---

## Getting started using the web console

Lets begin this lab by going to the home page.  You can do this by selecting the "Red Hat Mobile Application Platform" button located in the top left of the web console.

<img src="{{ site.baseurl }}/www/4.2/default/screenshots/rhmap-homescreen-admin.png" width="600"/><br/>
   *RHMAP Homepage with admin access*

## Create your own project

1. Navigate to the projects area.

2. Click New Project. <img src="{{ site.baseurl }}/www/4.2/default/screenshots/rhmap-newproject.png" width="600"/><br/>

3. Select the Xamarin Hello World Project by clicking choose on the right side next to it.

4. Enter a name for the project.

5. Click Create.
<br/><img src="{{ site.baseurl }}/www/4.2/default/screenshots/rhmap-xamarin-newproject.png" width="600"/><br/>

6. When the progress bar turns green the project is successfully created. Click Finish.

## Exploring the project
After creating a project, you can see the project page. This shows the client apps, cloud apps, and MBaaS services associated with a project.

* Client Apps: applications deployed on mobile devices used by the end users.
* Cloud Apps: applications deployed in the MBaaS that handle requests from client apps and communicate with other internal or external systems.
* MBaaS Services: reusable services used by cloud apps and shared across multiple projects.

The newly created Hello World Project contains one Xamarin client app and one cloud app with a single HTTP endpoint. You can add more client apps, cloud apps, and MBaaS services to the project by clicking the + symbol in each box.

## Deploying the Cloud App

Depending on settings within the cluster the cloud app may need to be manually deployed.  We will step through the process of how to do that now.

1. On the projects page open the *Cloud App*.  

2. Click **Deploy** on the sidebar on the left.
<img src="{{ site.baseurl }}/www/4.2/default/screenshots/rhmap-deploy.png" width="600"/><br/>

3. Click the **Deploy Cloud App**.

4. Once the progress bar turns green your cloud app will be deployed.

5. Click the **Details** button on the left sidebar.

6. Confirm that your **Cloud App Status** is *running*.  If the app is not started confirm your app successfully deployed on the previous page and then click **Start App**

## Creating a Client App
For this part of the lab we will create a Cordova application to easily walk through the process within the browser.

1. Navigate to **Apps, Cloud Apps & Services**.

2. Select **+** at the top of the **Client App** Column.

3. Select **Create New App**.

4. Click **Choose** on the **Cordova App**.

5. Name your new Cordova app *Cordova Hello World* and select **Create Client App**.

## Exploring the Client App

1. The app details page shows information about your client app.  It has information such as the name, a Description, and the ID's which will be used later.  Since this is a Cordova application, which is HTML5, CSS, & JavaScript, we can preview the application in the browser.
<img src="{{ site.baseurl }}/www/4.2/default/screenshots/rhmap-clientappdetails.png" width="600"/><br/>

2. Test the app by inputing some text in the app on the right and selecting **Say Hello From The Cloud**

##Building the Client App

1. Navigate to **Build** on the left sidebar.

2. In the **Client Binary** section, select **Android** as the target platform.

3. Click **Build**.

4. Once the build is complete, a popup will display showing a download link & a QR code.  Android users can download the application natively to their devices now.

``` Note: On your Android mobile device, you must enable the option to install apps from unknown sources. See the section User Opt-In for Apps from Unknown Sources in the Alternative Distribution Options guide in Android documentation for more information. The client app built in this example is considered by Android as coming from an unknown source since the client app binary is not signed with a developer’s certificate. ```