# Pulumi-cosgrid
You will use Pulumi to depoy infrastructure changes using code. Install Pulumi here , verify that it is working install pulumi ,Please go through folowing steps:-

Step1:- check your system that's its  have a pre-install pulumi or not

$ pulumi version
v2.7.1

If not then go to https://www.pulumi.com/ and install it according to your system configuration and operating system .So,if your system have a linux then just write a command or copy paste it in your terminal to install pulumi 
curl -fsSL https://get.pulumi.com | sh , 
After this check again that it install or not by type a command  pulumi version in your terminal.

For more detail or reference to download and install it in your system ,you can go through the pulumi docs https://www.pulumi.com/docs/get-started/install

Step 2:- Now , after installing you can sigin to pulumi at pulumi console or by just typing a command pulumi login to get your token https://app.pulumi.com/ 

Step 3:- Now, some prerequisites you have to install in your system ,to satisfied a need of your resources :
NodeJS
Docker
AWS Subscription ,If you want azure or want use any other cloud or want any programming languages installation ,you can go through :-
https://github.com/pulumi/infrastructure-as-code-workshop/blob/master/00-installing-prerequisites.md

for your aws subscription go to aws.amazon.com and sign in .Now, you have to install aws cli verion 2 to install it open yoou terminal and type 
curl "https://awscli.amazonaws.com/awscli-exe-linux-x86_64.zip" -o "awscliv2.zip"
unzip awscliv2.zip
sudo ./aws/install
For more detail visit https://docs.aws.amazon.com/cli/latest/userguide/install-cliv2-linux.html
after ,thhis you can configure your aws for your security by getting a security credentials from IAM user in a programatic access.
Type :- aws configure
 and type your access and secret key that you get from your credentials
 Example:-
 $ aws configure
AWS Access Key ID [None]: AKIAIOSFODNN7EXAMPLE
AWS Secret Access Key [None]: wJalrXUtnFEMI/K7MDENG/bPxRfiCYEXAMPLEKEY
Default region name [None]: us-west-2
Default output format [None]: json


Now, you readdfy to go:-


#######Create a new project####### :
Step 1:- open your terminal
Step 2:- type mkdir pulumicosgrid
Step 3:- cd cosgrid
Step 4:- pulumi new aws python -y
Step 5:- you can name your projrect otherwise enter ,then it save your project name by default as directory name.
Step 6:- Your stack is created now , its by default name is dev but if you want to change you can otherwise hit enter
Step 7:- code . , its open yourv editor to help to access your main file and other configuration file too.
Step 8:- You have a main.py file which by default have a s3 bucket code ,that creates a s3 bucket .
Step 9:- To check whether it have a error or not , type a command in a terminal of visula studio or in your root terminal pulumi preview
Step 10:- If have a error then debug it,otherwise run pulumi up in a termianl.
In  a next  have upload with a images too .
