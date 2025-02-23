# HTML Details Element Script Execution Issue

This repository demonstrates an uncommon bug related to the execution of a &lt;script&gt; tag placed inside an HTML &lt;details&gt; element.  The script within the &lt;details&gt; element, by default, will not execute. This is because the browser does not process the script when the content is initially rendered in a collapsed state.

**Problem:** The script within the &lt;details&gt; tag is not executed until the &lt;details&gt; section is expanded.

**Solution:** Move the script outside the &lt;details&gt; element or use an event listener to execute the script after the &lt;details&gt; is opened.