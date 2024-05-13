![[dashboard_screenshot.png|align:center|450]]

The [[Dashboard.canvas|Dashboard]] is an Obsidian Canvas constructed to help keep track of the progress you have made during your studying experience. 

To utilize the Dashboard, you will be required to download the [AstroWiki 2.0 repository](https://github.com/AYelland/AstroWiki_2.0) to your local machine and work within the Obsidian application. In the following steps, I outline the necessary changes you will need to make to your local version.

## Changing the Homepage:

Currently, the *homepage* for the AstroWiki is the [[AstroWiki Homepage|splash page]] you saw when first navigated to the URL. In the local version of this Obsidian Vault, this means that you can quickly navigate to this splash page by clicking on the house-icon on the top-left of your Obsidian window. Additionally, this splash page will be opened when no other pages or files are opened.

This can be a useful thing, but there is a more useful, recommended homepage if you are using a local version of the AstroWiki to study: the [[Dashboard.canvas|Dashboard]]. To change the default homepage...

1) Navigate to the Obsidian Settings by clicking on the cog/gear in the bottom left of the application window.
2) Click on the **Homepage** plugin under the heading of **Community Plugins**.
3) Change the filename in the top of the **Homepage** settings to the reference *"Dashboard.canvas"* file, instead of the *"AstroWiki Homepage"*.

![[HowToDashboard.png|align:center]]

## Structure and Configuring the Dashboard

As mentioned before, the [[Dashboard.canvas|Dashboard]] is an Obsidian Canvas. That is, it is a specific type of Obsidian file that allows us to create sticky notes, reference already-created notes and images, and connect them all together with lines and explanatory text. This proves to be very useful with brainstorming ideas, developing program/code structures, and creating bubble plots for different concepts.

We exploited this feature with the assistance of some Javascript and the Dataview plugin to create a widget-like homepage to track our studying progress. As the user, all you have to do is change some date values for your specific study plan! 

Here's how...

1) Navigate to the [[Deadlines]] file (`x. Other/DashboardResources/Deadlines`)
2) In the **Properties** at the top of the file, you will see 3 dates correlating to the deadlines you want to set to complete your first pass through the content (`first_pass`), your second pass through the content (`second_pass`), and the date of your oral exam (`test_day`). Change these dates to your desirable values.
3) Refresh (close and reopen) the [[Deadlines]] file, and confirm the numbers and dates are changing in the content of the file.
4) Navigate to the [[Dashboard.canvas|Dashboard]], and you will see three of the widgets will update with the proper dates and numerical values. (You may need to refresh the page if it was already open.)
5) Success! Your Dashboard is now configured. :)

On the right-side of the Dashboard, you will find a [[Question Checklist]]. This is the key to the whole Dashboard experience. As you complete questions and check them off the list, this will automatically update all of the numbers and progress bars on the rest of the Dashboard. It gives a visual representation of the effort that you put in and how many more questions you have yet to complete.

On the top-left of the Dashboard, there is also a [[Tasks To-Do]] widget that can be helpful for tracking where you left off, what you completed, and what you want to work on next. 

Finally, on the bottom of the Dashboard, you will find a handful of useful links and hyperlinks referencing the list of the [[168 Questions.pdf|168 Questions]], the [[168 Flashcards]], the AstroWiki 1.0 and 2.0 GitHub repositories, and more.

> [!note] If you ever want to open any of the widgets as a full page, you can right-click, and "Open in new tab".