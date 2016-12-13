# How to download from Mixcloud

This document explains how you can download a mix
from Mixcloud by yourself without any third party software. However I want to recommend not doing that on your on, instead use this [Mixcloud Downloader](http://www.mixcloud-downloader.com/).
Having said that, here's the step by step manual how to download from Mixcloud:

## Prerequisite
You need Chrome or Chromium as browser. Actually
Firefox works as well, but this document refers to specifics of Chrome.
Furthermore you'll need a tool to download from a URL e.g. wget.

## Instructions
1. Go to [Mixcloud](https://www.mixcloud.com/).
2. Open Chrome's DevTools by pressing `ctrl+shift+i`.
3. Select the "Network" tab in the DevTools.
4. Find the mix which you want to download on Mixcloud and start the playback.
5. You now see a list of resources in the DevTools. Sort the resources by size.
6. The largest resource is the mix which you can directly dowload. The URL matches the following URL template: `https://stream{number}.mixcloud.com/c/m4a/64/{path}.m4a` e.g. "https://stream13.mixcloud.com/c/m4a/64/b/e/c/6/1f6b-fd50-4ad4-aa44-0376c01a73ee.m4a"
7. Right click on that resource and select "Copy Link address". Now you have the URL of the downloadable mix
in your clipboard.
8. Use a download tool like wget to download the URL which you copied into your clipboard. Example: `wget https://stream13.mixcloud.com/c/m4a/64/b/e/c/6/1f6b-fd50-4ad4-aa44-0376c01a73ee.m4a`
