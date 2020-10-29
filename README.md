# Even Better Jira
Removes everything off the screen that is not the kanban board itself, and then fullscreens the page. (must refresh the page to bring menus back)

![fullscreen jira kanban board](https://user-images.githubusercontent.com/39921371/97606917-525a0f00-19de-11eb-9bff-33af2e57645f.png)

## Instructions
1. Bookmark this page
2. Right click the newly created bookmark
3. Click "Edit" (if on Firefox, click "Properties")
4. Rename the bookmark to "Even Better Jira"
5. Copy and Paste the following code into the "URL" section of the bookmark (or "location" or "Address" depending on the browser)
```
javascript:(function(){var container=document.querySelector('[data-testid="Content"]'),sideNav=document.querySelector('[data-testid="Navigation"]'),topNav=document.querySelector('[data-testid="atlassian-navigation--header"]').parentNode,boardMenu=document.querySelector("#ghx-operations"),titleHeader=document.querySelector("#ghx-header"),breadCrumbs=document.querySelector('[data-testid="rapidboard-breadcrumbs"]'),board=document.querySelector("#ghx-work");[sideNav,topNav,boardMenu,titleHeader,breadCrumbs].forEach(function(e){e.remove()});var haxor1337styles=document.createElement("style");haxor1337styles.type="text/css",haxor1337styles.id="haxor1337styles",haxor1337styles.appendChild(document.createTextNode('[data-testid="Content"] {padding: 0px !important; margin: 0px !important; }')),container.parentNode.insertBefore(haxor1337styles,container),board.style.height="100vh";document.documentElement.requestFullscreen();})();

```
6. Open a jira kanban board and click your new bookmark
7. Profit!

---
### Like this tool? [Let me know!](mailto:sisk@hey.com?subject=Hey%20I%20really%20like%20Even%20Better%20Jira!)
---
made with ♥️ by Adam Sisk

