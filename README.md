# Install Apache Maven on Linux
# Step 1:

      Download apache-maven-3.6.2-bin.tar.gz binary archive from the official link

      https://maven.apache.org/download.cgi
      
# Step 2:

      Open the Terminal and change the directory to /opt folder.
     
# Step 3:
      Extract the apache-maven archive into the opt directory.

      sudo tar -xvzf ~/Downloads/apache-maven-3.6.2-bin.tar.gz
      
# Step 4:
      Edit the /etc/environment file and add the following environment variable:

      M2_HOME="/opt/apache-maven-3.6.2"

# also, append the bin directory to the PATH variable:
      /opt/apache-maven-3.6.2/bin

# Notice the end of PATH variable and the M2_HOME variable.

      PATH="/usr/local/sbin:/usr/local/bin:/usr/sbin:/usr/bin:/sbin:/bin:/usr/games:/usr/local/games:/usr/lib/jvm/jdk-10.0.2/bin:/opt/apache-maven-3.6.2/bin"
      JAVA_HOME="/usr/lib/jvm/jdk-10.0.2"
      M2_HOME="/opt/apache-maven-3.6.2"

# Step 5:
        Logout and login to the computer and check the Maven version using the following command.
        mvn --version
