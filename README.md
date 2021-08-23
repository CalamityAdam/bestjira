# Even Better Jira
Removes everything off the screen that is not the kanban board itself, and then fullscreens the page. (must refresh the page to bring menus back)

### **UPDATE** Feb 01, 2021 script has been updated
If you already have the "Even Better Jira" bookmark, simply copy the new script below and edit the existing bookmark to replace the old script.

---

![kanban board](https://user-images.githubusercontent.com/39921371/130500882-863427ca-68f4-422e-8a15-f5c94a022b73.png)


## Instructions
1. Bookmark this page
2. Right click the newly created bookmark
3. Click "Edit" (if on Firefox, click "Properties")
4. Rename the bookmark to "Even Better Jira"
5. Copy and Paste the following code into the "URL" section of the bookmark (or "location" or "Address" depending on the browser)
```
javascript:(function(){var frontend=document.querySelector('#jira-frontend'),container=document.querySelector('.ghx-work-wrapper'),sideNav=document.querySelector('[data-testid="ContextualNavigation"]'),topNav=document.querySelector('[aria-label="Primary Navigation"]'),boardMenu=document.querySelector('#ghx-operations'),titleHeader=document.querySelector('#ghx-header'),breadCrumbs=document.querySelector('[data-testid="rapidboard-breadcrumbs"]'),headerBanner=document.querySelector('header[role="banner"]').parentNode.parentNode,board=document.querySelector('#ghx-work');[sideNav, topNav, boardMenu, titleHeader, breadCrumbs, headerBanner].forEach(elem => elem && elem.remove());document.querySelectorAll('.ghx-issue-subtask').forEach(elem => elem.style = 'margin-left: 20px;');frontend.style = 'padding: 10px;';frontend.firstElementChild.firstElementChild.style = 'display: block;';board.style = 'height: 100vh;';document.documentElement.requestFullscreen();})();

```
6. Open a jira kanban board and click your new bookmark
7. Profit!

---
### Like this tool? [Let me know!](mailto:sisk@hey.com?subject=Hey%20I%20really%20like%20Even%20Better%20Jira!)
---
made with ♥️ by Adam Sisk

