How to setup a Jenkins production and testing pipeline using docker??

Assumptions: Jenkins And Docker are installed in RHEL OS

Jenkins is added in sudoers file.

User has a Github Profile and Git Bash is Installed

What i did in this project ?

I integrate my local git repo with github repo, if i do any commit in any of my local repo of git , than git push command will auto trigger and than our code will update in github, AS i link my github repo with Jenkins jobs , when any changes found by jenkins in master branch ,than jenkins will trigger job2 hw, which than launch a docker httpd os on top of redhat and we can see the site by ip:port , or another one remote paerson can see this site by ngrok . but we dont want to deploy job2 directly on production environment

if jenkins found any change in dev1 branch than jenkins trigger job1 , this work is first tested by quality assurance team to check the quality of code and fix error, if QAT will certified that there is no error in this code than we will merge this code to with master branch in job3 that is merge QAT approved, this job3 will merge dev1 branch with main master branch and launch a web server on production environment , that is tested by Quality assurance team.


Linkedin Artical Url : https://www.linkedin.com/pulse/devops-achieving-full-automation-using-jenkins-docker-varun-bhutani/?published=t
