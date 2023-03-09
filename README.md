# How to host and format a resume online. 
The purpose of this README is to ensure that you know how to host a personal resume online and properly format it using more specialized software other than word.  

**Prerequistes**: Ensure you have the following... To better generate a resume a light-weight markup language is needed. One of the most popular ones is Markdown. A crash course for Markdown is linked [here](https://youtu.be/HUBNt18RFbo) by Traversy Media on Youtube. 

The tech-stack used for this instruction is Visual Studio Code, Jekyll, and GitHub. Instructions for using them are below. 

# **Instructions:**
**Let’s start!**  

### **Using a light-weight markup language.** 
As a computer science student you might have heard of one of the most popular IDE is Visual Studio Code. Did you know that Visual Studio Code can also write in markdown, requiring no other installation. 
1.	If you already have it installed you are set! Otherwise, it can be installed [here](https://code.visualstudio.com/). 
2.	click new file on the top bar of visual studio code, once installed.
3.	Type the name of the document in the box that popped up near the top, resumename.md, ensuring the .md is at the end.
4.	Click the preview button in the top right bar with a book and magnifying glass to see a preview of the markdown file as you type. 
5.	Click save, once finished. You now have a markdown file that you can customize!
Andrew Etter states on page 21 of  Modern Technical Writing (link below to access), that markdown makes the text easily readable in the file. Without the file looking like a complete mess and unreadable such as using the XML language would bring. Which is the reason why using Markdown is such a preferred choice. It also works well will version control systems which GitHub is specifically designed for. 
One you are happy with the styling of your resume in markdown you now have a file that can be used to host! 

### **The common static site generator Jekyll**
Jekyll can be used to easily modify your resume styling before hosting it to the GitHub pages platform. Andrew Etter states on page 31 using a static website is practical in that they have compatibility with many popular hosting sites, such as GitHub pages, but also there is less technical dependencies required to know for building the website. In fact the bulk of the work is simply uploading the file directory. One of the most requested features that Jekyll offers is the ability to host the website locally before uploading it. 


1.	Download the Ruby installer [here](https://rubyinstaller.org/). 
    * Note: you will want the most stable build for your operating system. Here Windows is used. 
2.	Run the Ruby installer. 
3.	Download RubyGems Zip file [here](https://rubygems.org/pages/download).
4.	Unzip the folder and run the setup.exe
5.	Open windows terminal. To ensure everything has installed correctly run the following commands independently. Both should state a version if installed correctly. 
Ruby -v
Gem -v
6.	Install Jekyll by running the command in Windows Terminal. ‘gem install Jekyll bundler’
7.	Verify Jekyll is installed by running, ‘jekyll -v’ in the windows terminal. 
8.	The next three commands will be in the terminal, we will create the source files. Run, ‘jekyll new projectName’
9.	Navigate to the directory ‘cd projectName’
10.	Run ‘bundle exec Jekyll serve’ . This will host your website locally at localhost:4000. 
11.	Open any browser and navigate to localhost:4000 in the address bar. 
12.	Edit the website to your liking. The site will start with a default layout, customize as you see fit. Removing any pieces that would not satisfy.
13.	Replace index.md file with your resume.md file, but rename your resume.md file to index.md. 
14.	Optionally choose a theme. Many Jekyll themes can be retrieved or bought. A website is linked in extra resources for a popular website for getting free themes. Alternatively, you can stick with the default theme.
15.	You now have a website you can use to host your resume! 

### **Using GitHub, a popular distributed version control system.**
Andrew Etter explains on page 28 that version control systems such as GitHub are used to allow for better performance, offline work, and concurrent work of the same set of files. There are many more version control systems that are used, but GitHub is the more popularly used. There are some downsides to using a version control system for documentation writing for example there are numerous other ways to use GitHub besides developing a single document, but the main benefit comes with writing he documentation on the same system that the application is developed on. 

1.	Go to [GitHub](https://github.com/).
2.	Make an account (If you don’t have one already).
3.	Create a new repository. Ensuring the public box is ticked. 
4.	Click ‘create repository’. A repository is used to hold our files, and to hold the history of those files as we update them. 
5.	Upload website files to repository creates. Under ‘code’, click uploading an existing file.
6.	Choose existing website files created by Jekyll in the previous topic, once uploaded commit the changes. 
7.	Now the files are in the repository! We just need to instruct GitHub to host it. 
8.	Click ‘settings’ under repository.
9.	Click ‘pages’ under the automation section on the left bar. 
10.	Click main, under branch. 
11.	Click save. This will start building your page! Note: this can take quite a long time, if the build fails you will be notified by email. 
12.	Your resume is now hosted globally at the website indicated of the top of the pages document! Congratulations!

![Guide](https://media.giphy.com/media/v1.Y2lkPTc5MGI3NjExOGY2MGFjMmQzZjY4YjgxZTQ1OGQwOGNiZDY2Zjc5YzAzZmFiN2MyNyZjdD1n/sSBB3OiKaMPpxi5Dqi/giphy.gif)



### **More resources**
* [Jekyll Website](http://jekyllthemes.org/)
* [Mike Dane Youtube Channel](https://www.youtube.com/playlist?list=PLLAZ4kZ9dFpOPV5C5Ay0pHaa0RJFhcmcB)
* [Free Jekyll Themes! ](https://jekyllthemes.io/free)
* [Markdown tutorial](https://youtu.be/HUBNt18RFbo)
* [Andrew Etter's Book](https://www.amazon.ca/Modern-Technical-Writing-Introduction-Documentation-ebook/dp/B01A2QL9SS)


### **Authors and acknowledgements:**
* Group 13 members including Jiazhem, Edmund, and Kushaan for peer review. 
* Jekyll 'minima' theme
* Traversy Media on Youtube.
* Mike Dane on youtube. 

## **FAQs:**
1.	Why is Markdown better than a word processor? 
    * The most popular word processor such as Microsoft Word actively opposes version control as Andrew Etter describes. Version control is essential to documentation. 
2.	Why is my Resume not showing up. 
    * Follow each step ensuring done correctly. 
    * in _config.yml, ensure the 'base URL' tab has your repository name, otherwise this will not work.
    * It is possible when uploading to GitHub not all the files uploaded correctly. Double check the required files are present.
