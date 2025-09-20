Create a front end server

Access AWS Cloud
1.Log into AS,
	 AMI user preferably, Root User if necessary.
2. Go to dashboard
3. Select your Region 
4. Click All services
5. Click EC2

Security Groups 
1.	Click Security Groups from sidebar
2.	Create security group
3.	Create a name for Security Group
4.	Provide a Description
5.	Go to Inbound Rules and Add rule
6.	Under 'Type' select "http"
7.	Under 'source' select "Anywhere-IPv4"
8.	DO NOT TOUCH OUTBOARD RULES(Avoid like the plague)
9.	At Tags, add tags as needed or wanted

Create EC2 Instance
1.	Go to Instances 
2.	Click Launch Instance.
3.	Create a Name for the instance.
4.	Go to Key Pair.
5.	Create a new Key Pair.
	Name it the same as your instance.
6.	Download the .pem file.
7.	Go to Network Settings.
8.	Select the existing security group you created.
9.	Confirm it by checking the last 4 characters of the ID.
10.	Next, skip to Advanced Details.
11.	Find User Data.
12.	Copy the EC2 script from Theo's GitHub link.
13.	Paste the scrip in Use Data.
14.	Click Launch Instance.

Test the Server
1.Once successfully launched, click the link in the green bar.
2.Copy the Public DNS.
3.Paste the link in your browser.
4.Always type http:// before the DNS.
	Example:http://ec2-18-191-216-220.us-east-2.compute.amazonaws.com
5.If it fails:
	a.Check that the correct security group is attached.
	b.Confirm the Inbound Rules include HTTP, source set to Anywhere-IPv4.

