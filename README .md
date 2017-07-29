# Catalog Item Project :
  Web Site that list set of categories and its Items , allow registered users via Oauth2 by third part which is google plus , allowing CRUD operation for both Category and its items .

#Installation:
  you have to follow the following steps to make the project run : 

    1- you have to download and install Python backage from [here](https://www.python.org/ftp/python/2.7.13/python-2.7.13.msi) 
    2- use terminal like Git Bash that comes with Git software
	2- install virtual box  to run virtual machine 
	3- install vagrant which enable you to configure virtual machine and let you share files between your host computer and the vm's file system , install it from vagrantup.com 
	4- download VM configuration from here : https://github.com/udacity/fullstack-nanodegree-vm.
	5- start virtual machine , from your terminal and inside vagrant directory at vm configuration directory , run thisa command Vagrant up  which will download linux operating system and install it 
	6- log into linux operating system by type vagrant ssh after previous step
	7- change directory to vagrant which is shared directory by  typing cd /vagrant
	8- place the project directory inside the vagrant shared directory 
	9- change directory to /project 
	10- run this command python allication.py which will run application project that  listen locally on port 8000
	11- go to your browser and hit this url http://localhost:8000
	13- navigate our site by visiting public home page and loge in to enjoy using my project  


#Project Directories and Files : 
	A- Project Directory : the main directory that contain all files and directories of the project as follow: 
    	1-Application.py:
			is the main Flask module which has the definition of the all methods and settings of all routes which is responsiple for accessing various pages and get action to various http requests , also connecting to database 


	    2-database_setup.py:
			it is python file that have the ORm that deals with the database by creating its metadata 

		3- lotsofitems.py :
			python file to populate the database with set of categories and items 
		4- itemscatalog.db :
			the generated database from running lotsofitems.py
		5- client_secrets : it is google based file that generated from google api and have all credentials of my application to get access to google api seuucessfully

		5- templates Directory : 

			1- categories.html:
				to list all categories and items for the loged in user 
			2- deletecategory.html :
				to delete category and accessed only by the loged user 
			3- deleteitem.html:
				to delete an item and accessed only by the loged user 
			4- editcategory.html:
				to edit category and accessed only by the loged user 
			5- edititem.html:
				to edit an item and accessed only by the loged user 
			6- itemdetails.html :
				to show item detals accessed only by the loged user 
			7- login.html:
				to enable users from logging into the application using google plus 
			8- loginheader.html:
				contain the required items that have to  be placed in the header of the site for loged users
			9- main.html :
				contain main sengelton of any page and have tags to import jquery library and style sheet file styles.css 
			10- newcategory.html:
				to create new  category and accessed only by the loged user 
			11- newcategoryitem.html:
				to create new category item and accessed only by the loged user 
			12- publiccategories.html:
				to list all  categories and items and  accessed by public
			13- publicheader.html:
				contain the required items that have to  be placed in the header of the site for public navigators
			14- publicitem.html:  
				to list  items for selected category and  accessed by public
		6- static directory : 
			1- styles.css :  contain all css code to style all templates elemenets 

  
#License: 
	The contents of this repository are covered under the [MIT License](https://github.com/udacity/ud777-writing-readmes/blob/master/LICENSE).