---
author: Chen Wei Zhu
---
[![DOI](https://zenodo.org/badge/299578130.svg)](https://zenodo.org/badge/latestdoi/299578130)  

# Building a Static Personal Site on Github--A Guide with a Simple Template for Law Students

- This  template is made by [Yet Another Legal Academic (YALA)](https://icaruszhu.github.io/)  for my personal tutees at Birmingham Law School. Please feel free to download, fork, alter, remix, or do whatever you want with the repo template to suit your own need. It is licensed under the permissive MIT License.

- You can delete this README.md page later if you wish. 

- Personally, I like the [Architect theme](https://github.com/pages-themes/architect)  for its elegant simplicity. The theme is licensed under the CC-0. You can choose other themes that fit your aesthetic preference better. Remember almost everything in this repo is customisable. 


# Download this repo 

- Use your favourite command line terminal with ```git```
```git clone https://github.com/icaruszhu/student-gh-page-template.git```

- Alternatively, you can use the old-fashioned method by hitting the ```download``` button

# Modification for a quick start
There are two files in the repo you need to personalise in order to create your own site. I use some placeholder words such as the fictitious student name "Tem Plate" and the fabled "University of Rashomon ".  Please do change them as they only exist in [Meinong's jungle](https://en.wikipedia.org/wiki/Meinong%27s_jungle):-)

##  1) ```index.md``` 
```index.md``` is the file where your CV lives. You can add information such as your background, education, experience, award, hobby, aspiration etc. 

## 2) ```_config.yml``` 
You definite need to modify ``_config.yml```, especially these two places:
~~~yml
title: Tem Plate   # put your name to replace "Tem Plate
description:  Law Student @ Birmingham Law School # you can change this line as well
~~~
I have put some comments after the ```#``` symbol and they are self-explanatory.

## More modification

There are a lot more you can customise. For example, you can change layout files and those ```css``` files, but they can left alone for the time being. You may want to change them at some point when you feel a bit adventurous. 

# Create your ```gh-pages``` 
- Finally, you will need to create your site to be hosted by github pages. You can have a domain name  with your github ```UserName```, i.e., [UserName].github.io. The guide https://guides.github.com/features/pages/ provides a detailed guide.

- Alternatively, you can also store your personal site as a normal git project and then create a ```gh-pages```  branch to host html contents.  This branch needs to be created both remotely and locally. 

	- Remotely, create a gh-pages on from github. See the screenshot below
	
	  <img src="https://raw.githubusercontent.com/icaruszhu/student-gh-page-template/gh-pages/image/shot-create-gh-pages-branch.png" alt="create gh-pages branch on github" style="zoom:80%;" />
	
	  You can check if this ```gh-pages``` branch is created. Here is another screenshot that ```gh-pages``` has indeed be created and ticked!
	
	  <img src="https://raw.githubusercontent.com/icaruszhu/student-gh-page-template/gh-pages/image/shot-new-gh-pages-created.png" alt="gh-pages branch is created" style="zoom: 67%;" />
	
	-  Locally, create a ```gh-pages``` in your git repo on your laptop from the terminal. Copy and paste the below two lines of code:

```bash
  git checkout -b gh-pages  # create a local gh-pages brach
 
  git push --set-upstream origin gh-pages # link the local gh-pages with the remote gh-pages
```
Now, it's done! It may take a small while for your site to go live. So be a bit patient.

p.s. Since you are going to work onlny with the newly created ```gh-pages``` in future for your personal site, you may choose to delete the remote  ```master``` branch by  typing this command in the terminal:
~~~bash
      git push origin :master
~~~


# Next step: when you become a more advanced user ...

There are a lot more you can do with your static personal site. For example, you may wish to learn to use Jekyll to build your personal website locally on your laptop. Jekyll also allows to install plug-ins to have some more features. 

It is worth noting that many third-party jekyll plug-ins are not supported by Github pages. For example,  one of my favorite plugins [Jekyll-Scholar](https://github.com/inukshuk/jekyll-scholar) is not supported by gh-pages by default. I need to build my site locally and  need to use jekyll to locally and need to use ```git subtree``` to push html contents to the remote branch. However, you do not have to worry about this for the time being. The out-of-the-box features of gh-pages are more than sufficient for building a static personal site remotely. 

Of course, you may also wish to learn ```git``` [version control](https://git-scm.com/) in order to get to the bottom of what is ultimately going on. You can find local software carpentry workshops that teach ```git``` and plenty of online tutorials.  

Here is a screenshot that shows how  ```git``` is used to "push" the local ```gh-pages``` changes to their remote counterpart on Github. Please do not feel alarmed that the displayed text in my terminal is Chinese, but this does not really matter.)  

<img src="https://raw.githubusercontent.com/icaruszhu/student-gh-page-template/gh-pages/image/git-update-push.png" style="zoom: 50%;" />

# More informaiton

https://docs.github.com/en/free-pro-team@latest/github/working-with-github-pages/about-github-pages

Happy hacking!

# citation
```bibtex
@software{chen_wei_zhu_2020_4058914,
  author       = {Chen Wei Zhu},
  title        = {{Building  a static personal site on Github -- A 
                   guide with a simple template for law students}},
  month        = sep,
  year         = 2020,
  publisher    = {Zenodo},
  version      = {0.8.0},
  doi          = {10.5281/zenodo.4058914},
  url          = {https://doi.org/10.5281/zenodo.4058914}
}
```
