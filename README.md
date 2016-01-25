# udacity-p1-portfolio
Udacity P1

# Install

1. Clone this repository
2. Run the following commands on the project directory as a user. Refer to documentation to install npm.
  
  ````bash
  npm install
  bower install
  grunt build
  ````

3. Point a VirtualHost to the ````dist```` directory. For example, in apache 2.4:

  ````
  <VirtualHost *:80>
	ServerAdmin webmaster@localhost
	ServerName udacity-p1.local

	DocumentRoot /home/username/projects/udacity/udacity-p1-portfolio/dist/
	<Directory /home/username/projects/udacity/udacity-p1-portfolio/dist>
		AllowOverride All
		Require all granted
	</Directory>


	# Possible values include: debug, info, notice, warn, error, crit,
	# alert, emerg.
	LogLevel warn

	ErrorLog ${APACHE_LOG_DIR}/udacity-p1.local-error.log
	CustomLog ${APACHE_LOG_DIR}/udacity-p1.local-access.log combined
  </VirtualHost>
  ````
