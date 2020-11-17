This is a submission for the Hawaii Annual Code Challenge (HACC 2020).
Check it out at https://hacc-fire-frontend.vercel.app/
(if it becomes unavailable, it is because I killed the AWS EC2 instance.
Also the HTTPS certificates are self-signed because I do not hae a domain, so the browser will give you a warning that the site is untrusted).

The challenge done was: Hawaii State Archives – Gamification of Crowdsource Indexing
See: https://hacc.hawaii.gov/challenges/ for more info on the challenge. This image creates an interactive interface for

A nice little app that I learned a lot from! The front page is pretty spare... click the buttons in the tool bar to checkout the whole thing.

Frontend Technologies: React, NextJS
Backend Technologies: NodeJS, Postgresql
Other Technologies: OAuth2 for Google Login, AWS ElasticBeanstalk (backend hosting), Server Certificates/Keys for HTTPS, Cookies

Current features:
-Allow users to login with Google OAuth2 to keep track of their contributions
-Show leaderboard with score of each user -Display pdf served from an Amazon S3 bucket (can be migrated to SharePoint or other storage solution)
-Read a schema file from S3 bucket and dynamically create DB columns
-Server tasks when the file name is specificed before hand (working on dynamically reading all tasks from file)

Possible future features:
-Point to a storage folder to create a schema based on an xml file and create tasks automatically
-Allow csv file download of the postgres data of compelted tasks
-Allow form validation of tasks before user submits
-Allow tracking of tasks so that each task is served to two individuals
-Allow users to skip a task and go onto next ask