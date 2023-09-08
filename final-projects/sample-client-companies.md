# Example Companies for ops-201 Projects 
## 1. A tiny new space startup looking to build and deploy micro-satalites.
   - The company has mostly been hardware and software engineers working out of a large converted garage space.
   - They have received some grants and some investments, and they want to expand to hire more engineers, but also a few non-technical employees such as an office manager, a media person, etc.
   - Most employees will continue to work out of a central location, but both technical and non-technical users will sometimes need to travel.
   - Information security is a priority: The company's only value is its intellectual property. The company is unwilling to allow these technical designs to be stored on the cloud, and does not want any it's intellectual property to leave the building (except in the form of offsite backups).

## 2. A small non-profit supporting a new popular cause.
   > This cause has recently become widely known, and the organization has received lots of donations, as well as funding support from the city for the next 5 years. They are not exactly rolling in dough, but it makes sense for them to create more volunteer, part time, and full time positions.
   - They have a deal to receive used business laptops donated by large companies, but they will still need an MSP to configure and manage them.
   - Employees will be allowed to keep their computers when they leave, since the cost of retrieving, inventorying, and redeploying already old systems is not worth it.
     - However, the computers will still need to be stripped of an sensitive information, licensed software, etc.
   - Keeping costs down is one of their highest priorities.
   - The non-profit has a small central office, but rather than trying to move to a larger location they are choosing to switch to a hybrid work model. The office will serve as more of a central meeting, coworking, and coordination space, with only a few people working from individual offices.
   - Your MSP will be donating most of the cost of this project, so it is important to your bottom line to minimize the labor costs of setting up and maintaining these systems, training users, and responding to help-tickets. Keep things simple.
   - Similarly, pursue free software solutions whenever possible, to reduce the non-profit's overhead.
   - Most employees fill roles as social media managers, community organizers, researchers, media strategists, etc., role with relatively low security requirements.
     - However, some employees handle a lot of financial information and PII from processing donations, so those users will have stricter security needs.
       - For political reasons (however sound or unsound), the leadership of the non-profit insists on storing this financial and PII data securely and on-site, rather than using the cloud.

## 3. A company specializing in remote surveying and GIS solutions has grown steadily and now wants to upgrade and formalize its IT systems.
   - The company has two main types of users:
     - GIS Software Engineers, who work in a central office and use powerful workstations running ArcGIS.
       - These systems need to automatically backup to central NAS in the office, available as a network drive.
       - GIS Engineers will occassionally need to remotely connect to these systems
     - Surveyors, who will work oversees for weeks at a time and use toughbooks running Linux Mint and specialized surveying software.
       - These systems need to automatically backup all data to a second internal hard drive.

## 4. A small CGI company was founded by two high-school friends needs to grow beyond the living room.
   > These friends started out making videos on their phones. Now they employ a few more artists and a business manager. The two founders live together and their home has served as a defacto office, but the other employees usually work from home.
   - With the money from recent advertising jobs, they want to hire more artists and move into a real office where they will have the space to expand.
   - They want to move away from the BYOD method and start providing computers owned and managed by the company.
   - The artists are proficient and responsible Windows and Mac users, but lack any IT skills.
     - Artists work mostly on powerful Mac or Windows workstations, though they also have laptops used for lighter work and when filming.
   - Managing the many large video and graphics files has been a pain-point. With artists working from home, the stop-gap solution has been a poorly organized shelf of external and internal hard-drives used to move data to and from the founders' home.
     - They would like some kind of central data storage solution on site at their office.
     - They may want to make this central data storage solution accessible remotely in the future, but that is not a current need.

## 5. A relatively successful Youtube channel making education videos would like to create spinoff channels with different themes and subjects.
   > The company is entirely remote, and would like to stay that way.
   - Responsibilities at the company include researchers, writers, video editors, market research, advertising, SEO, etc., though most people wear many hats.
   - Even though their existing BYOD policy has been working fine up until now, the company intends to start providing employees with laptops.
     - Because different employees will have different needs and preferences, the expectation is that users will select their preferred model of laptop, which the company would purchase and the MSP would provision and manage.
   - Employees include both Windows and Linux users, though most are not highly technical.
   - Written collaboration is a big part of this company's process, so some way to work together over the cloud is important. Detailed version control would be a plus, but is not required.
   - Video editors will need a large, local backup solution.
   - The company would like a cloud-based data storage solution for video files, though this is mostly for archival purposes rather than colalboration.

## 6. A local chain of grocery stores has survived for years on an ancient system of file-cabinets and paper receipts. 
   > Over the years only a minimal number of computers were added for point-of-sail systems and to comply with the digital ordering systems of their regional and national providers. ("If it's not broke, don't fix it! I've run my company like this just fine for 40 years!" was something she was fond of saying.) A few years ago the founder partially retired, and her two children took over day-to-day operations, and introduced a few more computers to the office, even wifi! Now the founder is fully retiring and handing the business over the now co-owners, who have big plans to bring their business into the 21st century.
   - The point-of-sale system is old, but still works fine. They may look into upgrading it in a few years, but for now it is not a priority.
   - Most of the company's employees work in roles which do not require computers or training.
   - Employees who do will need computers mostly work in a small central office, though branch managers and assistant managers will also need computers.
   - Many employees have been unofficially bringing and using their own computers at work for years, using them to email spreadsheets to one another, but there is no SOP and no training for how these computers are used, or any type of security training or requirements.
     - By and large, employees have very low computer skills.
   - Over the years the original paper inventory management system has been variously and incompletely supplemented or replicated in excel spreadsheets, emailed back and forth and passed down from employee to employee.
     - That situation is a mess, and the new owners intend to implement a modern, database-backed inventory management system using some kind of off-the shelf commercial software. That is more than they can tackle this year though, but for now they would still like you to set up a server which could be used to host this software in the future.

## 7. A tech startup writes specialized software for managing industrial control systems. 
   > Though they have a superior product, their market share is small, since most companies don't see the need in changing something that works. That was until a couple of months ago, when the current market leader suffered a catostrophic, humiliating security breach which dominated a slow news cycle for a week. Now potential clients are starting to shop around, but they'll want to know that any new software provider will be able to handle their large needs. Faced with this increadible opportunity for rapid growth, the startup needs to first scale itself quickly, and that means replacing the one employee who has filled all the IT needs for the company with a professional MSP.
   - As far as software companies go, this one is more old-school than hip start-up. Most of their developers are older, with many years in the industry.
   - The company used to work out of the same office in 2019, but quickly dropped the lease in 2020 when the state ordered all non-essential workers to stay home. After the restrictions eased the company continued to operate remotely, but many employees miss the comraderie of a shared work-space.
     - Both to satisfy these employees and to help integrate all the new hires into the existing company culture, the company intends to open a new office and establish a hybrid work model.
   - The company has acquired several pieces of equipment to serve as a real world testing platform for their control software. For the software engineers to effectively work from home they will to be able to remote into these systems (both CLI and GUI).
   - Software engineers use a mix of Windows and Linux systems. The hardware is owned by the company, but the engineers have traditionally been granted local admin access and allowed to install, modify, and configure their machines as they wish.
     - The company's CISO has determined that to achieve a desired level of security compliance, this policy will end, and all engineers will need to run laptops configured and managed by the MSP according to company SOPs.
   - The company's code-base has been maintained on Github, but the company would like to move to a private git server located in the office.
   - Both engineers and non-technical employees will need a way to easily share files.
