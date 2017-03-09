---
layout: essay
type: essay
title: "Meteor Gotchas"
date: 2017-03-09
labels:
  - Software Engineering
  - Meteor
---

# Introduction

In my time with Meteor, I personally have not had much issues with the framework. However, over Slack for the ICS 314 class, several students have posted various questions and answers to different issues when working with Meteor. While Meteor is a great tool to have when developing modern day web applications (as it can easily organize both server side and client side code), it does have quite a bit of a learning curve. In this essay, we will cover two issues encountered by people using the Slack channel for the ICS 314 class

# Long Run Times

One particular student using a MacBook had a particularly hard time getting the application to run under the DNF time of the WOD (more than 30 minutes). She was trying to configure the correct files/settings to get the application running right when it took too much time to complete the assignment. Furthermore, she claimed that GitHub showed over 8,000 more files to be committed than on the case with demo video.

Another student had a similar problem and was able to elaborate on the issue: she was instructed by the software to run the command 'meteor npm install -save bcrypt' to make the original command run faster. The OP (Original Poster) tried that command but still not luck. It was after some more conversation between the students and a third person jumped in that the solution began to be made clear: the command would get fast after running it for the first time. So, repitition, or getting rid of some initial processes, saved the time and allowed the Meteor app to be built more quickly.

The professor chimed and and pointed out the true cause of this issue is that the first time that command is run, it downloads a bunch of packages, but doesn't do that after the initial run. Also, he noted the bcrypt warning can be safely ignored.

# Pushing People's Buttons

One more comical scenerio was when one of the students wasn't able to get a button working quite right. While working with Semantic UI to help improve the look of a Meteor application, one user couldn't get a submit button to work. In many scenarios, you use a <div> element with a special class to get a certain component of a website. However, this student's mistake was using <div> instead of the already dedicated <button> tag. This error was pointed out and corrected by another student.

# Conclusion

In the end, we can see that problems large and small can be solved by a community that stands together. Meteor makes modern applicaiton design more efficient, and allows other to create things they wouldn't have been able to before without having time for other projects.