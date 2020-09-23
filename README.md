# AWS-case-study


### Samsung Migrates 1.1 Billion Users across Three Continents from Oracle to Amazon Aurora with AWS Database Migration Service
2020

The cloud, as it turns out, is big enough for everyone. It’s even big enough for Samsung Electronics, the world’s second-largest IT company by revenue. As users of Samsung Account—the company’s certification and authorization service—ballooned to over 1.1 billion, the electronics giant decided it was time to move its massive database away from its monolithic legacy Oracle internet data center (IDC) solution, which was expensive and made it difficult to scale to accommodate growing traffic. Looking to the cloud, Samsung Electronics found Amazon Web Services (AWS) a perfect fit for this shift. In less than 18 months, Samsung Electronics migrated its global Samsung Account data to Amazon Aurora, a MySQL- and PostgreSQL-compatible relational database built for the cloud. This migration from Oracle resulted in a profound cost reduction as Samsung was able to free itself from the restrictive licensing costs of the on-premises legacy database. With the migration to cloud-native Aurora, Samsung is able to focus on innovating and positioning itself for the company’s expected growth.

### Moving from Monolith to Microservice
Samsung Account is the gateway through which users access Samsung devices and services such as Bixby, SmartThings, and Samsung Pay. Roughly 400 million of Samsung Account’s 1.1 billion users are active on the platform, which sees about 80,000 requests per second, making it critical that the system functions well. Though the IDC database solution hosted by Oracle was adequate when it was instituted 10 years ago, Samsung Electronics needed a more flexible, microservices-driven solution to better serve current and future users. According to Jung, Oracle was not ready for microservices architecture, nor did it have reasonable pricing for it.

“The Oracle-based architecture is harder to update because it’s a big chunk of application, thus called a monolith,” explains Salva Jung, Principal Architect and Engineering Manager at Samsung. Also, scaling up the dated system without downtime had become risky and costly, causing concern over whether it could handle the scale of new users and services and the volume of traffic they create. “We wanted to have new technology and a microservices architecture to cover upcoming traffic from our Samsung devices and services.” By moving to AWS, Samsung gained access to tools such as Amazon Elastic Compute Cloud (Amazon EC2), which provides secure, resizable compute capacity in the cloud.

Attempting to achieve the needed scale on the monolithic architecture presented risks—and costs—that Samsung did not want to accept. Still, transitioning Samsung Account’s massive amount of data would be no small task, especially considering Samsung’s requirement that the transition not disrupt service. Samsung needed to move away from a central database, breaking down its databases into sections suitable for microservice uses, and the fully managed Aurora with PostgreSQL compatibility emerged as the best destination for the data migration and the most cost-effective option. 

### Easing the Great Migration with AWS Database Migration Service
For Samsung, one of Aurora’s most attractive features was that 85–90 percent of the PostgreSQL queries in Aurora matched the existing Oracle queries, meaning that converting the queries to Amazon Aurora PostgreSQL would be practically automatic. The company had 2–4 TB of data to migrate for each of the three regions—the European Union, China, and the United States—and it needed help ensuring everything went smoothly and successfully.

Samsung Electronics began the migration process in the European Union in October 2018 by creating dedicated lines between the IDC and the application programming interface, which acted as the gateway to Aurora. Then AWS Database Migration Service (AWS DMS)—which supports data migrations, including heterogeneous migrations between different database platforms such as Oracle to Aurora—initiated the transition of the data. As the data left the IDC for its new home, AWS DMS ensured that the source database remained operational so that end users could still access Samsung Account as usual. At the same time, AWS DMS replicated the large-scale heterogeneous database, duplicated 2 or 3 TB of user data in 3–4 days, and routed user traffic one by one from the IDC to the cloud. In just about 22 weeks, Samsung transitioned to Aurora, migrating 4 TB of data and converting nearly 3,000 queries. “AWS provided us the best information at the appropriate time,” says Jung. “And AWS had lots of tools and services to help the migration—AWS DMS is one example.”

Samsung completed the EU migration by April 2019, the China migration by October 2019, and the US migration by March 2020, all with minimal downtime. “We had some downtime but not much,” says Jung. “The important thing is that we detected problems quickly and minimized the user impact.

### Streamlining the Experience for Samsung and Its Customers
After the migration, Samsung is fully prepared for future growth. For example, Aurora now allows Samsung to seamlessly scale up to 15 Aurora Replicas—independent endpoints in an Aurora database cluster used for scaling read operations and increasing availability—across the availability zones in each region. With the scalability of Aurora, Samsung can serve more users more quickly than before: now 90 percent of latency is less than 60 ms. The automation of the cloud solution also allows Samsung to deliver more features to users faster.

Jung acknowledges that Samsung could not serve its customers as well using the old system. “If we had stayed with the IDC, we would have risked having servers go down, which would have meant a lot of downtime for the Samsung Account system,” he says. “Once we achieved the migration, we were able to receive a lot of traffic and provide a lot of services. The scalability of Aurora is the best benefit—especially if we focus on the cost.”

According to Byungyul Ko, Samsung’s database administrator, the company saves 44 percent on monthly operational costs with Aurora PosgreSQL compared to Oracle, on top of the additional Oracle expenses of a pricey IDC license fee and another 22 percent in maintenance fees. With Aurora, Samsung pays as it goes and only pays for what it uses, with no upfront fee or restrictive licenses.






### Looking Ahead to More Opportunities in the Cloud
The scope of the benefits of the migration to Aurora are still revealing themselves. For example, the Samsung team plans to explore how the AWS database engine can provide better analytics and insights. “We want to build up the data lake this year,” says Kiheung Park, principal data architect. “In the cloud, we have lots of options. We can aggregate all data in one region so we can analyze the user data better.”

By migrating to Aurora, Samsung was able to transform its monolithic database architecture into a faster, nimbler, and more cost-effective solution that streamlined service for both staff and end users. This goes to show that no company, even one as large as Samsung, is truly tethered to its legacy data center. There’s plenty of space in the cloud—and even more opportunity.


### About Samsung Electronics Co.
Samsung Electronics, the world’s second-largest IT company by revenue, is the flagship company of the Samsung conglomerate. It is the world’s largest manufacturer of mobile phones and a major manufacturer of numerous other electronics and electronic components.


### Benefits of AWS Databases
Underwent a global migration of a mission-critical workload in 18 months
Enabled 60 ms latency or less 90% of the time
Reduced monthly database costs by 44%
