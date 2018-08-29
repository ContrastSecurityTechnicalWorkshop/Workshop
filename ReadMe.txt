I fixed 2 vulnerabilities in WebGoat that Contrast detected.
One is Cross-Site Scripting and another is Overly Long Session Timeout.
Below are the source codes that I fixed.

1. Source code of Cross-Site Scripting:
webapps\WebGoat\plugin_extracted\plugin\CrossSiteScripting\jsp
ViewProfile.jsp

I fixed to escape HTML special characters when the values that the users have inputted are displayed.
# I wanted to fix "EditProfile.jsp" as well but unfortunately I didn't have much time.

2. Source code of Overly Long Session Timeout
sources\conf
web.xml

I set the session timeout to 30min(Default setting was 48 hours).
