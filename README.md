ASSIGNMENT NO.2
First repository index.html file
[root@ip-172-31-39-143 ec2-user]# cd REPO-1
[root@ip-172-31-39-143 REPO-1]# git config --global user.name piyali
[root@ip-172-31-39-143 REPO-1]# git config --global user.email piyalisaha@gmail.com
[root@ip-172-31-39-143 REPO-1]# vi index.html
[root@ip-172-31-39-143 REPO-1]# git add *
[root@ip-172-31-39-143 REPO-1]# git commit -m "repo1 commit"
[root@ip-172-31-39-143 REPO-1]# git log
commit 2884b758f374a4d4c3e9494c6404db15426357bc (HEAD -> master)
Author: piyali <piyalisaha@gmail.com>
Date:   Mon May 20 12:38:20 2024 +0000
    repo1 commit
[root@ip-172-31-39-143 REPO-1]# git remote add origin https://github.com/piyali1994/Repo1.git
[root@ip-172-31-39-143 REPO-1]# git push origin master
Likewise I followed this same steps for Repository2 index.html file and Repository3 index.html file.
Then I created job1 in Jenkins
1.	Adding URL of repository 1.
2.	Enabling built trigger as GitHub hook trigger for GITScm polling
3.	Build steps as follows
yum install httpd -y
service httpd start
service httpd status
cp * /var/www/html/
chmod -R 777 /var/www/html/
4.	Then I made changes in git hub webhook  
Simultaneously I followed this steps for my other 2 jobs in Jenkins.
the screenshot of my all 3 jobs in word file attached
1.	If I commit changes in my repository 1 then my job 1 builds automatically
2.	If I commit changes in my repository 2 then my job 2 builds automatically
3. If I commit changes in my repository 3 then my job 3 builds automatically
all the screenshots are their in my word file.
  

