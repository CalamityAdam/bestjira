# Even Better Jira
### instructions
1. Bookmark this page
2. Right click the newly created bookmark
3. Click "Edit" (if on Firefox, click "Properties")
4. Rename the bookmark to "Even Better Jira"
5. Copy and Paste the following code into the "URL" section of the bookmark (or "location" or "Address" depending on the browser)
```js
javascript:(function(){var container=document.querySelector('[data-testid="Content"]'),sideNav=document.querySelector('[data-testid="Navigation"]'),topNav=document.querySelector('[data-testid="atlassian-navigation--header"]').parentNode,boardMenu=document.querySelector("#ghx-operations"),titleHeader=document.querySelector("#ghx-header"),breadCrumbs=document.querySelector('[data-testid="rapidboard-breadcrumbs"]'),board=document.querySelector("#ghx-work");[sideNav,topNav,boardMenu,titleHeader,breadCrumbs].forEach(function(e){e.remove()});var haxor1337styles=document.createElement("style");haxor1337styles.type="text/css",haxor1337styles.id="haxor1337styles",haxor1337styles.appendChild(document.createTextNode('[data-testid="Content"] {padding: 0px !important; margin: 0px !important; }')),container.parentNode.insertBefore(haxor1337styles,container),board.style.height="100vh";document.documentElement.requestFullscreen();})();

```
6. open a jira kanban board and click your new bookmark
7. profit!

---
made with ❤️ by Adam Sisk
