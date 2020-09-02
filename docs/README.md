
# Eng. Managment
by Vic Cekvenich

## Background

There are organization where top managment jokes about: I don't even know why we are spending $40K per month on AWS. And they do that with pride.

One way to manage is to plan what you should be spending. That allows you to the compare and monitor to what you are spending on tech.
And it does not have boring, you can just come up with some ideal spending, and do that every 3 years or so. Here is some ideas as to what is cost effective to invest in:

## #1: Development / IDE

- Development is now moving into the cloud, so instead of running VS Code localy, you would run it in your cloud linux box - a bit similar to CodeAnywhere.com. :
<br/>
<img src="0ideVSCode.png" height="500">

- For front-end and designers you may use something modern, like Corvid or WebFlow. :
<img src="00wixFE.png" height="300">
<p/> 

<p/><br/><p/>
- For back end, you may want to leverage modern cloud services such as Google FireBase, it does an OK job w/ User Auth. Similar to FireBase is Strapi.io and it is free. :<br/>
<img src="00fbBEUser.png" height="200">
<p/>

<p/>
- And it maybe nice to have some automated code review like Codacy:
<img src="0codeQ.png" height="300">


### Dev. tools budget 
About $75 / month / developer.
So a team of 5 is ~$4K annual.

## #2: Architecture / DB

- When using a cloud, a popular service is S3:<br/>
<img src="01was.png" height="300">

- If using microservices, you'll need to use Dockerfiles and an enterpirse event bus, like NATS:
<img src="01nats.png" height="300">

- And you'll need a CDN, it makes things cheaper, faster and safer: 
<img src="01cdn.png" height="300">



### Architecture budget / Enviroments
About $150 / month / enviroment. Likely you'll have following enviroments:
2 Production:Blue/Green/Canary/EU
1 Staging Branch: Beta/QA
1 Dev(CI/CD Master):
So 4 enviroments is ~$6K annual.


## #3: SRE Infrasturcutre 

- You do need centralized logs:
<img src="2logs.png" height="300">

- And monitoring:
<img src="2mon.png" height="300">

- As you start getting customer traffic you'll need to build a centralized NOC/SOC dashboard, eg. Grafana:
<img src="2graf.png" height="300">

- With growth, you maybe doing infrastructure as code, Pulumi ( or Teraforma ):
<img src="2puluGitHub.png" height="300">

- Pulumi has help with complaince (eg SOC, HIPAA, PCI, etc. ):
<img src="2za_gove.png" height="300">

### Infrasturcutre tools budget 
About $250 / month.
So about ~$3K annual.


## #4: Testing, QA and CD

- In order to do capacity planning, you'll have to use one of the many load generators. If you use network, it will be expensive, so just use large RAM VM so you can have all the services and load generators VMs on the same box. If you don't do load testing, you can't do capacity planning. Large RAM cloud: 
<img src="4doStress.png" height="300">

- CD:
<img src="4CI.png" height="300">

- Mobile apps CD:
<img src="4mobileCI.png" height="300">

- Testing, E2E, there are 2 example vendors, Cypress and Puppetry:<br/>
<img src="4pup.png" height="200">
<img src="4teste2e100.png" height="200">


### Testing tools budget 
About $500 / month.
So about ~$8K annual.


## #5: Business Intelegence & business value

- Basic analytics : 
<img src="5anal.png" height="300">

- Optional analytics support :
<img src="5clickH.png" height="300">

- Business dashboard :
<img src="5dash.png" height="300">

- BI integration :
<img src="5panBi.png" height="300">


### BI tools budget 
About $1.2k / month.
So about ~$15K annual.




Managment tip, 10th sincer feedback
manage for celling or the floor
