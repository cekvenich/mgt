
# Eng. Tooling and Management Budget
by Vic Cekvenich

# Eng. Tooling 

There are organization where top management jokes about: I don't even know why we are spending $60K per month on AWS. And they do that with pride.

One way to manage is to plan what you should be spending. That allows you to the compare and monitor to what you are spending on tech.
And it does not have boring, you can just come up with some ideal spending. Here is some ideas to help you with your budget line items:

## #1: Development / IDE

- Development is now moving into the cloud, so instead of running VS Code locally, you would run it in your cloud Linux box - a bit similar to CodeAnywhere.com. And more secure than local development :
<br/>
<img src="0ideVSCode.png" height="500">

- For front-end and designers you may use something modern, like Corvid or WebFlow. :
<img src="00wixFE.png" height="300">
<p/> 

<p/><br/><p/>
- For back end, you may want to leverage modern cloud services such as Google FireBase, it does an OK job w/ User Auth. Similar to FireBase is Strapi.io and it is free. Maybe user auth should be it's own line item :<br/>
<img src="00fbBEUser.png" height="200">
<p/>

<p/>
- And it maybe nice to have some automated code review like Codacy:
<img src="0codeQ.png" height="300">


### Dev. tools budget 
About $75 / month / developer.
So a team of 8 is ~$7K annual.

## #2: Architecture / DB

- When using a cloud, one of the popular services is S3 store:<br/>
<img src="01was.png" height="300">

- If using micro-services, you'll need an enterprise event bus, like NATS:
<img src="01nats.png" height="300">

- And you'll need a CDN, it makes things cheaper, faster and safer: 
<img src="01cdn.png" height="300">

Plus some Docker cloud host, eg. DO.

### Architecture budget / Environments
About $150 / month / environment. Likely you'll have following environments:
2 Production:Blue/Green/Canary/EU
1 Staging Branch: Beta/QA
1 Dev(CI/CD Master):
So 4 environments is ~$6K annual.


## #3: SRE Infrastructure 

- You do need centralized logs:
<img src="2logs.png" height="300">

- And monitoring:
<img src="2mon.png" height="300">

- As you start getting customer traffic you'll need to build a centralized NOC/SOC dashboard, eg. Grafana:
<img src="2graf.png" height="300">

- With growth, you maybe doing infrastructure as code, Pulumi ( or Teraforma ):
<img src="2puluGitHub.png" height="300">

- Pulumi has help with compliance (eg SOC, HIPAA, PCI, etc. ):
<img src="2za_gove.png" height="300">

### Infrastructure tools budget 
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


## #5: Optional: Business Intelligence & business value

- Basic analytics : 
<img src="5anal.jpeg" height="300">

- Optional analytics support :
<img src="5clickH.png" height="300">

- Business dashboard :
<img src="5dash.png" height="300">

- BI integration :
<img src="5panBi.png" height="300">


### BI tools budget 
About $1.2k / month. 
So about ~$15K annual. But sometimes people don't have a budget for BI.
As an alternative to BI budget, Excel can connect to SQL and run queries for basically free.

# Management tools

## #1: Day to day

- Task tracking Notion, or AirTable ( most people don't like Jira ):
<img src="13notJiraTruth.png" height="300">
<img src="13air.png" height="200">

- Daily status reports, I like video: 
<img src="13loom.png" height="300">

- Screen shot tool: 
<img src="13screenShot.png" height="250">

- Live meetings tool: 
<img src="13skypeSlack.png" height="300">

### Day to day tools budget 
Day to day $75 / month / resource.
So a team of 8 is ~$7K annual.

## #2: Management tools

- Managing up, one of the most important tasks for VPE is doing info-graphics: 
<img src="99reportsUpPicto.png" height="300">

- 360 Management, OKR and 1:1 tool:
<img src="98small.png" height="300">

- Job posting:
<img src="99up.png" height="300">


### Management tools budget 
Day to day $80 / month / resource.
So a team of 8 is ~$8K annual.

# Resources / Salaries budget

2 FE /designer remote $25 / hr (100K)<br/>
1 BE / dba  $100K <br/>
1 BE / BI remote $15 / hr (40K)<br/>
1 SRE remote USA weekends $150K / yr <br/>
1 QA offshore weekends up/work $12 / hr (30K) <br/>
1 SA remote Upwork $50 / hr (100K) <br/>
==<br/>
$550K for staff

And tools:
7 + 6 + 3 + 8 + 0 + 7 + 8  
==
~$40K

and a remote VPE ~ $150K to run it, so a total of ~ $700K / year.


### A good use of this is for you to do your own budget

I hope above gives you ideas. If I missed a category or if something I have listed can be more efficient, please get in touch and let me know.

If you have a line item missing from the budget, it still can fly, in the way a plane can fly with one wing.<br/>
<img src="f15.jpeg" height="200">
