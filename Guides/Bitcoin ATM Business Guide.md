==== THIS ARTICLE IS A ROUGH DRAFT
This guide is written by Zachary Owens. Twitter: @zaowens for questions, comments, and contributions.

This guide was created to educate potential entrepreneurs how to properly setup and manage a legally operating bitcoin ATM business in the United States. By providing this information, the goal is to spread bitcoin ATMs out of major cities and into small rural areas and local communities to allow easier access acquiring bitcoin. ATMs are one of many critical “on-ramps” transforming traditional US dollars to into bitcoin. In addition to expanding ATMs to smaller cities and towns, this guide is also intended to create more competition which may eventually result in lower fees charged by operators.

Its very important to understand the regulations regarding this industry before deciding to go into business. This guide should to be followed in order unless otherwise instructed.

Guide Overview:

Understanding Legalities & Research
Prior Reading and Important Links (Index)
Business Laws & Licenses
Regulations
BSA / AML / KYC
Money Service Business (MSB) & Money Transmitter
Understanding Fiat/BTC Liquidity Flow (Money Cycle)
Banking Partners & Restrictions
Research ATM Manufacturers & Armored Truck Services
Business Setup
Forming an LLC
Setup LLC TIN
Opt-in to FINcen Regulations
Bitcoin Exchange Institutional Account Setup
Research Exchanges that Integrate with ATM Software
Register for Institutional Account
Gemini
Coinbase
itBit
Banking & Financial Partners
Understanding Out-of-state and LLC Foreign Entity Banking
Finding a MSB & Bitcoin Friendly Banking Partner
Traditional Bank / Credit Union
Third Party / Middleman Services
Umbrella ATM Company
Cash Vault and Armor Truck Services
Purchase and Setup of ATM
General Bytes ATM
Research and Purchase
Machine & Hardware Basics
Server Setup
Admin Panel Basics
Twilio Account Setup
BSA/AML/KYC Settings
Exchange Settings
Testing
ATM Placement & Servicing
Branding, Support, and Notices
Ideal Locations
Security
Internet Availability and Hotspots
Understanding Legalities & Research
Starting up a bitcoin ATM business is not as simple as you might think. Researching topics related to money service businesses and FinCEN regulations are a must. Your research should not stop there. Research every topic listed in this guide. If you are confused at any point then you are going to be in trouble and it will cost you money in one way or another.

Prior Reading and Important Links (Index)
As stated, prior research is very important. Here are some important links regarding topics you will become familiar with throughout this guide. This links are simply to help start off your research. Finding your own information is just as important and reviewing the ones listed here.

https://bitcoinsupport.center/blogs/operating-as-a-money-service-business-the-bitcoin-banking-burden-in-the-united-states/
https://en.wikipedia.org/wiki/Bank_Secrecy_Act
https://en.wikipedia.org/wiki/Financial_Crimes_Enforcement_Network
https://www.irs.gov/businesses/small-businesses-self-employed/money-services-business-msb-information-center
https://www.fincen.gov/sites/default/files/shared/FIN-2013-G001.pdf (FinCEN Virtual Currency Money Transmitter Statement)
https://en.wikipedia.org/wiki/Money_services_business
https://www.fincen.gov/sites/default/files/news_release/20141110.pdf
Business Laws & Licenses
A very important step before registering an LLC is to research state, county, and local business law and license requirements for you area. Some states require quarterly or yearly filings from LLCs. You might even decide you want to register your LLC in another state for tax or banking purposes. Most importantly, research any and all Money Transmitter laws and how they might apply to your ATM business. We will touch more on that in another section.

Regulations
In 1970 congress passed the Banking Secrecy Act (BSA), a law requiring financial institutions in the United States to assist government agencies to help detect and prevent money laundering. The agency in charge of the reporting is the Financial Crimes Enforcement Network (FinCEN), a branch of the United States Department of Treasury. Unfortunately, since your business is dealing with exchanging bitcoin for US dollar, the federal government has branded your business as a “money transmitter”. A money transmitter by FinCEN’s own definition is a person (or business) that provides a service that engages in a ‘transfer of funds’, or substitutes funds in another form to be transmitted or delivered from one person to another. Since FinCEN now declares businesses that buy/sell bitcoin as a money transmitter, it effectively groups businesses into what is referred to as a Money Services Business (MSB). MSB’s include money transmitters, check cashing, dealers in foreign currency exchange, or other money related instruments. All Money Services Businesses (MSB) are required by law to register with the Financial Crimes Enforcement Network (FinCEN).

BSA / AML / KYC
Banking Secrecy Act (BSA), Anti-Money Laundering (AML), and Know Your Customer (KYC) are the three most important things that will keep you out of federal prison while operating a bitcoin ATM. FinCEN requires financial institutions (you) to report any transaction totaling over $10,000 by filing a currency transaction report (CTR). CTRs can be filed electronically through FinCEN and is identified as FinCEN Form 112. Identifiable information regarding your customer will need to submitted on your CTR. This is where KYC comes into play. You need to know is purchasing large dollar amounts from your ATM in case a reportable incident occurs. Limiting your customer to $9999 per day is not a smart idea. FinCEN requires common sense reporting. In fact, if a customer purchases $5000 one day and $4000 the next day, you should likely file a CTR. If customers continue such actions in an attempt to avoid CTR reporting, its likely the customer is “structuring” their payments. Structuring is just like it sounds, arranging purchases to have an appearance of being smaller than they actually are. If you suspect a customer of structuring, laundering money, or just illegal activity in general, you are then required to file a suspicious activity report (SAR). These reports are filed with FinCEN and are identified as Treasury Department Form 90-22.47 and OCC Form 8010-9, 8010-1. It is illegal (federal law) for you to tell a customer you are filing these forms. All the reports mandated by the BSA are exempt from disclosure under the Freedom of Information Act.

Also, regulations require the business to draft a written anti-money laundering (AML) policy. The drafted policy typically states how the business will review itself to make sure that its own policy is followed. For smaller businesses this usually involves hiring an accounting firm to perform an annual audit.

All customer records, especially larger transactions, are required to be kept on file for 5-7 years. Not keeping proper logs or backups could result in financial fraud charges by the federal government. These regulations and reporting requirements are why bitcoin exchanges place limits on customer transactions for a daily/weekly amount.

Understanding Fiat/BTC Liquidity Flow (Money Cycle)

There a few different methods for paying out BTC to your customer. You need to figure out how you want to distribute your BTC, and how your cash will eventually be transferred from machine, to the bank, from the bank, then to the exchange. Your money/btc will need to come full circle to create a money cycle. One method is to hold US dollar on an exchange in surplus to the amount of expected cash sales. For this example we will hold $20,000 (USD) in our exchange. In our bitcoin hot wallet, which the ATM sends BTC to your customer, we will hold $20,000 in BTC. Now lets say a customer makes a $500 purchase from your ATM. Your hot wallet sends $500 worth of BTC to the customer minus your fees. That total is instantly purchased using your USD balance on the exchange, bringing your exchange balance to ~$19,500. Your ATM can now be emptied to retrieve $500 which is deposited into your bank. You now can initiate a transfer from your bank to the exchange for $500 bringing your exchange balance back to $20,000.

As you can see, there will likely be a delay from transferring your cash from the machine to the bank, and then the bank to the exchange. This means you will need enough BTC to cover customer purchases, as well as USD in the exchange to cover the BTC repurchase, to minimize your exposure to bitcoin price volatility.

Some operators have been able to cut out certain steps, such as purchasing on the exchange and sending from the exchange to the customer. This avoids the need to hold, for our example above, $20,000 in BTC. However, this method includes its own setbacks, and it may be against your exchange’s policy to send to customers from the exchange. Likely because it would expose the exchange to certain BSA/AML liabilities.

Banking Partners & Restrictions
As stated above, your business is considered a Money Service Business (MSB). This label by the federal government brings along a certain stigma. Banking is the most common point of failure when it comes to operating any kind of bitcoin related business, especially when your branded as a money services business. Most traditional banks will not bank MSBs, as MSBs are considered ‘high risk’ to banks. This, coincidentally enough, its due to the bank’s very own BSA/AML related policies. You need to be upfront with banks about your business. You likely need to talk directly to bank compliance managers in order to even stand a chance of opening an account. Lying to the bank about your business activities is a terrible idea. Same goes for using an already existing business name and bank account to deposit your ATM cash. You will learn very quickly that banks frown upon large cash deposits. In some cases, banks will open accounts, pass your account through compliance, then still shut down your account months later after seeing large cash deposits. This is why is important to be upfront with the bank, and work directly with compliance manager. Nothing is worse than setting up an  ATM and closing it down 3 months later due to banking issues. This exact scenario is VERY COMMON for small ATM operators.

Pay very close attention to any and all banking information is this guide. This cannot be stressed enough.

Research ATM Manufacturers & Armored Truck Services

You will need to decide which ATM manufacture fits your needs. The software provided by manufacturers will typical help run and monitor multiple machines. Read all sales contracts VERY carefully. Some manufacturers even charge a percentage of cash processed through the machine. Most have contracts regarding modifying the machine or require approval to resell your machine to another operator.

Common bitcoin ATM manufacturers:

General Bytes
Genesis Coin
Lamassu
bitaccess
Bitteller
Common Armored Truck Services

GardaWorld
Brinks
Loomis (wont service bitcoin ATMs directly)
Business Setup
For best results in setting up and forming your new business, you should have thoroughly researched all of the information above. By this stage, you should be forming some sort of business plan on how your business will operate, and what kind of starting capital you will likely need get your business up and running.

Forming a Limited Liability Company (LLC)
The difficulty of forming an LLC can vary by state. This guide will not discuss why you should form an LLC or even what it is. Please do some independent research in this area, or use the Legalzoom link we will provide in this section. Its usually recommended you talk to a business lawyer to form an LLC. Prices are usually well over $1000-$2000.

A cheaper and easier way to form your LLC is using an online service like Legalzoom. Here’s a quick example of what you should purchase from Legalzoom:






Once your registered with the state, your lawyer/Legalzoom will provide you with your company’s operating agreement. Scan every page of the agreement and save it on your PC and print out multiple copies. You will be asked for copies of your agreement when you register with financial companies and exchanges.

Setup LLC Employee Identification Number (EIN)
Your EIN is basically your business’s social security number with government. You will file your taxes using this number. Applying for an EIN is very straight forward and can be done instantly on the IRS website: https://www.irs.gov/businesses/small-businesses-self-employed/apply-for-an-employer-identification-number-ein-online

The website should give you an option to save / print a PDF of your generated number. Make sure to save this as financial institutions and exchanges will ask for it.

Opt-in to FinCEN Regulations
Now comes the hard part. FinCEN registration uses outdated adobe PDF submission software and internet explorer (not microsoft edge) compatible websites. Save yourself some trouble and just use internet explorer from the beginning.

These are legal documents. Its highly recommended you speak with a lawyer if you are not confident about fully understanding / administering the forms / legalities that you are reading.

Follow the information listen on the BSA E-Filing registration page here: https://bsaefiling.fincen.treas.gov/Enroll_Now_Step_02.html

If you are having trouble finding the actual registration link from that information its located here (example) :

https://bsaefiling.fincen.treas.gov/Enroll_Now_Step_02.html


After creating an account you will login here: https://bsaefiling1.fincen.treas.gov/PublicAccess (Using Internet Explorer) (NOT EDGE)

Once logged in, one the left menu under the “File FinCEN Reports” section, click “Report 107 – RMSB”. You will see a popup that looks like this:


Click “Open New Form” which should open your PDF registration file that looks like this:


Enter your LLC name like shown below:


Click the “Filing Information / Registrant Information” tab at the top of the page. For Part I, check “Initial Registration” box.  Under Part II check the entity box and enter your business LLC name on box 3 as shown:


Next we will enter our business address and EIN like shown:


Moving on to Part III “Owner or Controlling Person / MSB Services Location” tab, we will enter the controlling member of the LLC’s information (the owner). The TIN in this section will likely be your personal social security number. SSN-ITIN.


Section IV in the same tab will be titled “Money Services and Product Information”. Check the state or states you will be placing your machine in. You can always amend this information later. Example:


Moving on to Part IV continued, we will leave question 35 blank, and question 36 we will check mark ‘f’ for ‘Money Transmitter’. Referring back to our research, FinCEN considers your business as a money transmitter by federal definitions. Leave question 37 blank.


Skipping down to question 44 we will check mark ‘a’ for ‘Yes’. Question 45 is likely ‘b’ or ‘No’ depending on your business plans. All answers for question 46 are likely ‘0’ (zero) depending on your business. If you have registered agents, you probably don’t need to use this guide.


Part V “Primary Transaction Account for MSB Activities”. Unless you somehow already acquired a MSB bank account from a bank, this section will be left blank and amended when you open an account. The funny part about even asking for the banking information is that the bank will want proof of MSB registration (this form) before they open the account. So for the time being leave this section blank or fill in with N/A in required spots.


Part VI, enter you business or office address location. This information will likely be published publicly.


You will need to sign the document with your “PIN” which can be managed from the dashboard after you login as shown here:


 

 

Bitcoin Exchange Institutional Account Setup
After successfully setting up your business and acquiring the appropriate documents, we are now ready to apply for institutional accounts with leading US based bitcoin exchanges.  The reason you should use US based exchanges is because they offer ACH transfers between your bank and the exchange’s bank. Out of country exchanges will require international bank wires, which can become shady. You would also likely have to file additional tax paperwork showing money you have in foreign holding accounts. Banking partners may close your account when dealing with foreign exchanges. Best to stick with US if possible.

Gemini
Registering with Gemini for an institutional account is pretty straight forward. Fill out the form located at this URL: https://exchange.gemini.com/register/institution

A Gemini employee will send you a PDF application via e-mail. The application is around 16 pages long. They will require you fill out the application plus include proof of LLC registration with your state, your companies operators agreement, a W-9, copy of your BSA/AML program, and a driver’s license.

Coinbase / Coinbase Pro
itBit
 

== Banking and Financial Partners
The most difficult part of setting up a bitcoin ATM business is acquiring a banking partner. Since the federal government labels your business as a “money service business” (MSB), you are now considered a high risk to banks.

 

== Finding a MSB and Bitcoin Friendly Banking Partner
Your first goal should be to try to locate banks that will in fact bank MSBs. Not all banks advertise they bank MSB accounts. It may be easiest to call around and ask banks if they open accounts for regular cash ATMs. Once you find banks willing to bank regular cash ATM operators, you should try to setup a meeting with or email the banks compliance officer. The compliance officer at a bank is responsible for managing the bank’s risk. Speaking directly with a compliance officer means you are dealing directly with one of the main people that can authorize the opening of your account.

 

== Minimizing Appearance of Risk
A good approach to make a bank feel comfortable with banking you is to minimize the amount of legal gray areas you are operating in. You should be able to confidently demonstrate to a compliance officer that your business is in compliance and registered with FinCEN and that your business does not require a money transmitter license from your state. Some states you might be required to carry a money transmitter license. Check if your state’s department of banking has issued and regulatory guidance on cryptocurrency. You may wish to seek professional counsel and have them issue a written legal opinion on the information you have gathered. Presenting this information to a bank will remove a small area of risk.

Be able to demonstrate your mechanisms for complying with FinCEN BSA/AML/KYC regulations. Demonstrate you have a working knowledge of how to prevent money laundering on your ATM and restrictions you put in place. Explain how your machine collects and stores identifiable information on your customers.

 

If you have found a bank that accepts regular ATM operators, they may allow you to open account categorized as one since you were able to reduce your risk. In the end, some banks may just not open account for bitcoin related accounts.