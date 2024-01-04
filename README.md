# ALSupportToolFramework
A framework for support tools for ISV, Partners and others.

This extension is for support tasks and makes detecting and fixing common errors/known potential issues faster. This tool does not contain any detection mechanisms but will instead expose a table where people can add Codeunits containing detection and/or fix for a given task. The main page shows which issues are detected as the background tasks report back, and you can then mark an issue and press fix. This will then run the supplied fix CU or redirect you to a URL with information on how to fix this manually.

If detection CUs are supplied, then those are run as background tasks when opening the tool's Main page. Each detection can contain rules for whether they should be run unless a specific BC version or Extension is installed (Or a combination). See example CUs in this repo *Insert link here*.

Passing parameters/results from the detection CU over to the fix CU utilizing a dictionary is possible. So the fix CU does not always have to run the entire detection process all over again.
