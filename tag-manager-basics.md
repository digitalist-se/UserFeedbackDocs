
### *Quick navigation*

[Home](./index.md) | [Form templates](./form-templates.md) | [Form creation](./form-creation.md) | [Feature requests and bug reporting](./feature-requests-and-bug-reporting.md)

# Getting started with Matomo TagManager testing
When you work with Matomo tracking you want to testrun your code before going live. Sometimes you also might want to test your tracking or solutions on a site you are not in control of.
This article will describe how you can use your browser to do this.
 Simulating Matomo tracking on any website in Chrome browsers
 
The steps you need to do are quite simple. 
In this guide we recommend the plugin “User Javascript & CSS” for Chrome but there are similar plugins available for other browsers, such as Greasemonkey for Firefox as one example. You can also manually past the code to any browser (read further down how to do that). 

1. Install the Browser plugin “User Javascript & CSS”
Add the plugin to your Chrome browser https://chrome.google.com/webstore/detail/user-javascript-and-css/nbhcbdghjpllgmfilhnhkllmkecfmpld?hl=sv
 
2. Add the TagManager Code via the plugin interface
First go to the URL where you want to testrun Matomo for example 
http://digitalist.se
Click on the plugin icons and then “Add rules to this page button.
 
 
 
## Find your TagManager Code
You will find the code to use in the Matomos Tag Manager.
First select the container to use, then click on the menu item Install code.
The code looks something like this:
```
  <!-- Matomo Tag Manager -->
  <script type="text/javascript">
  var _mtm = window._mtm = window._mtm || [];
  var d=document, g=d.createElement('script'), s=d.getElementsByTagName('script')[0];
  g.type='text/javascript'; g.async=true; g.src='https://your-server/matomo/js/container_3u3tkNVV.js'; s.parentNode.insertBefore(g,s);
  </script>
  <!-- End Matomo Tag Manager -->
 ```

You want to copy everything in purple from your code. Do not  copy the red parts. It will not work (that code works when you add it to an html page, like in your CMS or similar. )
Now paste your TagManager code into the rules for Digitalist.se and save.

After this you can browse the site and you should be able to to see calls to you Matomo Sever.
 
 
# A simple test in the browser console
Go to the page where you want to testrun Matomo, then open up the dev console.
In your console just paste your Matomo Tag Manager code and press enter (to execute the code).
An example from Google Chrome below:

 
How to open the console in different browsers.
## Chrome
To open the developer console in Google Chrome, open the Chrome Menu in the upper-right-hand corner of the browser window and select More Tools > Developer Tools. You can also use the shortcut Option + ⌘ + J (on macOS), or Shift + CTRL + J (on Windows/Linux).
## Firefox
You open the Web Console from a menu or with a keyboard shortcut: Choose Web Console from the Web Developer submenu in the Firefox Menu (or Tools menu if you display the menu bar or are on Mac OS X) Press the Ctrl + Shift + K ( Command + Option + K on OS X) keyboard shortcut
## Internet Explorer
To open the developer console in Internet Explorer, click on the Gear Menu in the upper-right-hand corner of the browser window and select F12 Developer Tools. You can also press F12 to open it. The console will either open up within your existing Internet Explorer window, or in a new window.
## Edge
To open the developer console in Microsoft Edge, open the Edge Menu in the upper-right-hand corner of the browser window and select F12 Developer Tools. You can also press F12 to open it. The console will either open up within your existing Edge window, or in a new window. You may have to select the Console tab.
