install vs Code :
command:

sudo snap install code --classic


********************************************************************************************************
install postman:
command:

sudo snap install postman

***********************************************************************************************************
install xampp:

Step 1: Download the installation package

https://www.apachefriends.org/index.html


Step 2: Make the installation package executable
Move to the Downloads folder by using the following command:
$ cd /home/[username]/Downloads


The installation package you downloaded needs to be made executable before it can be used further. Run the following command for this purpose:
$ chmod 755 [package name]


Example:
$ chmod 755 xampp-linux-x64-7.2.10-0-installer.run


Step 3: Confirm execute permission
It is important to verify if the package can be executed by the current user. The execute permission can be checked through the following command:
$ ls -l [package name]

Example:$ ls -l xampp-linux-x64-7.2.10-0-installer.run


Step 4: Launch the Setup Wizard
As a privileged root user, run the following command in order to launch the graphical setup wizard.


Example:sudo ./xampp-linux-7.2.10-0-installer.run

Step 6: Launch XAMPP through the Terminal
$ sudo /opt/lampp/lampp start

********************************************************************************************************
laravel Project installation and composer installation:


   1. Update nad upgrade packages:
    sudo apt update && sudo apt upgrade

   2. Install php:
    sudo apt install php7.2-common php7.2-cli php7.2-gd php7.2-mysql php7.2-curl php7.2-intl php7.2-mbstring php7.2-bcmath php7.2-imap php7.2-xml php7.2-zip

    3.Install composer(dependency manager for php):
    sudo apt-get install composer

   4. Give full access to composer:
    sudo chmod 777 -R /home/$USER/.composer

   5. Command for generating laravel app:
    composer create-project --prefer-dist laravel/laravel blog

   6. Serving the application:
    cd blog && php artisan serve
    
    *******************************************************************************************************

