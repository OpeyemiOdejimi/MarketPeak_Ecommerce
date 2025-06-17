# E-commerce Platform Deployment with Git, Linux and AWS

The scope of the project is develop an e-commerce website for a new online marketplace named "MarketPeace" . This platform will feature product listings, a shopping cart, and user authentication. Objective is to use Git for version control, develop the platform in Linux environment, and deploy it on an AWS EC2 instance.

## Tasks
### 1. Implement Version control with Git

* In linux cli, create a project directory named _**MarketPeak_Ecommerce**_.
* Initialize a git repository inside the directory for version control

```
mkdir MarketPeak_Ecommerce
cd MarketPeak_Ecommerce
git init
```

### 1.1 Obtain and Prepare the E-commerce Website Template

Instead of developing a website from scratch, a template can be downloaded from ![specific template](https://www.tooplate.com/view/2130-waso-strategy). Extract the downloaded template into your project directory.

```
unzip <website-template>.zip
```

The command will unzip the downloaded zip file which contains the website template.

### 1.2 Stage and Commit the Template to Git

* Add your website files to the Git repository.
* Set your Git global configuration with your username and email
* Commit your changes with a clear and descriptive message.

```
git add .
git config --global user.name "YourUsername"
git config --global user.email "Youremail@example.com"
git commit -m "Initial commit with basic e-commerce site structure"
```

### 1.3 Push the Code to a GitHub Repository

* Create an empty repo on github named _**MarketPeak_Ecommerce**_. Link the local repo to GitHub in your terminal. Run the commands below

```
git remote add origin https://github.com/your-git-username/MarketPeak_Ecommerce.git
```

> Note: Replace 'your-git-username' with your username

* Push your code to the remote repository.

```
git push -u origin <branch-name>
```
* Run `git branch` to find out the branch you're currently working on.

### 2.AWS Deployment

### 2.1. Set Up an AWS EC2 Instance

* Log in to the AWS Management Console
* Launch an EC2 instance using an Amazon Linux AMI
* Connect to the using SSH

```
ssh -i path\key-pair\ ec2-user@ip-address
```

