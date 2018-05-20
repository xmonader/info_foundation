## Frequent Asked Questions

Proposed FAQ Questions for ThreeFold from Richard Walker, Bruce Lites, Jennifer Long

### Internet versus Cloud?

**Question:** The precise role Threefold will play in the entire internet system needs more clarification. ThreeFold is often labeled as “the new internet”, but from what we understand it is more specifically a new cloud technology. The “internet” is the system of connections and routers (and more powerful core routers) that direct packets of information to their intended destination.  In addition to the system of routers and local connections, there is a system of high-speed, long-haul data pipelines (“highways”) called the internet “backbone”.  We understand that ISPs host and pay for maintaining the routing and data transfer infrastructure, hence charge their clients for this service.  Does ThreeFold not only provide an alternative to cloud computing, but also provide some routing service?  If not, is that an area where the ThreeFold grid could improve on its efficiency and speed?

**Answer:** You are right - the original term internet is short for inter(connected) net(works).  This is how it all started - independent networks decided to interconnect (for free).  The purpose of interconnecting networks is to make information available to a wide group (both in numbers and in geo locations) of people.  

So information is stored somewhere and people want to that information. So the original term internet was all about interconnecting networks but the actual purpose for doing that was to allow people to access content.  What would the current internet be without any content?  A network is only able to transport transient messages from source to destination - a means of communications.

What we mean with “internet” today is the total construct of a _lot_ of information stored in network accessible locations.  Therefore the ThreeFold Grid will present new _internet_ capacity to the world.

On top of this cloud technology has a specific connauchtation to it as technology capable of running applications centrally.  As we are building a complete decentralised grid of capacity we would like to stay away from calling it cloud not not have that centralised connaughtation.  However (and this might complicate this answer) our decentralised grid _is_ able to run the same applications and all the existing and established cloud providers.

### What is the required connection speed for Farming?

**Question** Will high-speed connections be essential to the ThreeFold nodes, even small individually-owned ones?  That is, is there only a very a limited utility for home-based ThreeFold nodes unless they have a very high connection speed? If so, it is important to quantify their minimum useful connection speed?

**Anser** Yes and No.  (-; The connection speeds can in theory be anything and the further we reach out and go to the edge the lower the available connection speed will be.  We have not yet colelcted any real life data and once more Farmers are up and running we will start to collect and present this data.

A good rule of thumb is that for home based (small) nodes 10Mbps and up is a good starting point and for larger installations 100Mbps and up is good.  Obviously these numbers are available and affordable (!) in Europe, USA, and some areas in Asia but not everywhere.  For other parts of the world we might end up with mouch lower connection speeds or even alternative networking technologies for exmaple [LoRa](https://en.wikipedia.org/wiki/Long-range_Wi-Fi) or others.

### What specifically does the ThreeFold blockchain manage?

**Question:** Does the ThreeFold blockchain record all operations and data transfers?  If so, can this get out-of-hand rapidly in terms of storage capacity, and eventually slow the process of validating each blockchain?  If not, is it used only to manage the exchange of tokens for capacity (plus in the future to manage Digital Me), or does it manage metadata of all transactions?

**Anser:** The ThreeFold Chain has muiltiple dedicated blockchains running in parallel.  ThreeFold believes that the most secure and scalable way to run blockchains is not to operate general purpose blockchain technologies but create specific [hard coded](https://en.wikipedia.org/wiki/Hard_coding) in the blockchain software.  The TF Chain has a number of blockchains today and more likely than not will have more in the future.  The blockchains part of the TF Chain today are:

 - Financial transaction blockchain.  This blockchain is dedicated to allow financial transations
 - DataBase blockchain(s).  This blockchain is dedicated to store data.  These blockchains can store many different type of data and there are more of these depemnding on the use cases.

### How is redundancy achieved?

**Question:** How does the distributed data storage achieve redundancy?  

**Answer:** The Grid presents raw capacity in the form of primitives.  The actual Zero OS does not know how to store objects in a redundant manner, it provides storage primitives to read and write data. Primitives are best described as building block by which one can create a service.  For example the S3 service uses the storage primitives to build a software defined storage service.

Redundancy is achieved by the storage service by doing the following things:
 - cut the original object (document, photo, movie) into small pieces
 - by using a certain algorithm create additional (redundant) pieces of data.  Depending on the algorithm a small or larger number of redundant pieces of data can be created.  Think of this process as completing a [sudoku](https://en.wikipedia.org/wiki/Sudoku] puzzle).  The unsolved puzzle resembles the original object to store (photo etc.) the algorithms to create additional redundant data is the solving algorithm for the puzzle (numbers 1 - 9 can only appear once in a row, column and 3x3 number square).  The further solved the puzzle is the more data redundancy is created.  
   - unsolved puzzle + 4 additional numbers
   - unsolved puzzle + 8 additional numbers
   - etc.
  the individual numbers are then stored on a disk in a single zero-os node, on a number of disks on a zero-os node, on multiple zero-os nodes in the same location or on a number of zero-os nodes in multiple locations.

By adjusting the amount of redundant data created and where the data pieces are stored you can create very redundant storage solutions.

**Question:** Is this done somewhat like a RAID system?

**Answer:** No - This is very different, but is has elements that are similar.  Cutting objects into small pieces of data and storing those on different disk to be disk failure redundant is similar. The generic term for the technology is [erasure coding](https://en.wikipedia.org/wiki/Erasure_code)

### What is the redundancy factor for data on the ThreeFold network?

**Question** If stored data is present in multiple nodes for resistance of the grid to local failures, by what factor is the required grid storage greater than the actual data volume stored?

**Answer** As mentioned in a previous answer the level of redundancy depends on the software defined storage algorithmn.  The storage algorithm can be configured to be resistent to failure of:

 - disks
 - chassis
 - datacenter (location)

 The amount of required [Storage Units](https://github.com/threefoldfoundation/info_foundation/blob/master/docs/definitions/threefold_cloud_units.md) goes up with the higher level of redundancy build in the software defined storage solution.  Resilience to a single disk failure comes in at a lower price than building resilience to datacenter failure.

### Do larger nodes perform different functions than individual nodes?

**Question:** Do the small “household” nodes perform a different function from the larger configurations?

**Answer:** Nope - household nodes run zero-os and present a (lot) smaller number of cloud units than the larger configurations.  They will have a smaller number of applications running on it due to limited resources, but thay might be part of a super resilient storage solution.

As an exmaple of how household nodes can be used to build a large virtual datacenter consider a telecommunications operator that has in a large number of cities fibre to the home.  What if they consider putting a household machine into each and every home that purchased their internet connectivity.  Many commercial models can be deployed for this, the farmed tokens can be given as a discount to the telcos customer, the telco customer could be given an amount of storage capacity free of charge etc etc.  The telco would then have a distributed pool of capacity on which services can be build and run.

### Is there a simpler way to explain the 30% capacity rule for farming income?

**Question** A farm needs to reach 30% capacity before receiving TFTs.  Once this capacity is reached in a single month, will the farmed TFTs from all consecutive prior months where the 30% limit was not reached be awarded? Also, does this rule apply continuously; i.e. that each time the usage falls below 30%, tokens are withheld until th3 30% usage level is achieved again?

### Is there a simple way to quantify the 30% capacity treshhold?

**Question:** The online definition of ThreeFold compute units and storage units is not easy to comprehend by the non-expert.

**Quation:** How difficult is it to achieve 30% capacity usage, particularly for compute units.  Isn’t it a bit difficult to achieve 30% CPU usage on average?
The 30% number wsa invesnted to make sure people would join the movement to believe, follow and present usable capacity.  Not just token hunters.

The believe is that the required internet capacity to fuel the (Internet of Things)[http:8.8.8.8], (data storage growth)[http:8.8.8.8] and generic capacity requirements will drive capacity usage.  With the pricing being interesting compared to the competition it should attract tons of interest.

### How does the ThreeFold Grid know to host specific applications near it's users?




**Question** Not all applications and data can be hosted locally because of the scale of the data involved.

### How specificallt is "proof-of-stake: implemented in the Threefold Gdid?"

The TF Chain has multiple blockchains that are specific to a task.  The different blockchains running is parallel have a proof of stake consensus mechanism implemented.

### Where can one find a set of detailed technical requirements for ThreeFold farming hardware?

**Question** There is a lot of interest in small-scale farming, but the hardware requirements do not seem to be written down, particularly for single nodes that are financially possible for many people.  It is very important that capacity become widely available in many locations, so we need understand the constraints for the hardware before promoting the ThreeFold system. This information is also needed if we are to approach manufacturers to produce hardware for future farmers.

**Answer:** This is work in progress. In general please consider that the following high level requirements are considered to be the minimal requirements.  Older and smaller might work but there might not be enough token return in using that hardware to cover for the electricity, network and "cooling" cost.

- intel based CPU with at least 2 physical cores.
- 8 GB of ram
- 128 GB of SSD storage
- 1 TB of HDD storage

This combination of components provides you with a setup that will run zero-os and after the grif has inspected the hardware will provide a token return of approximately <<insert token return number>>

### How are ThreeFold Tokens valued relative to farming Capacity

There are several aspects to this question:

**Question** If the token value relative to fiat currency “floats” on the open speculative market, then its value can change rapidly by large amounts. The value of capacity in terms of fiat currency will fluctuate correspondingly unless the cost of internet capacity in tokens is also allowed to float.  If not, then if the speculative market for tokens drives the price up, the ThreeFold internet capacity could rapidly become more expensive than that of the current cloud providers. Will internet capacity in tokens be allowed to float?


**Answer:** The mechanism here is as follows:
 - Token value is determined by demand and supply on token markets
 - ThreeFold grid capacity pricing is _set_ by Farmers in **fiat** currency.

 Therefore the farmer can set his capacity pricing against the global market / competitors.  This is done in the (local) fiat currency.  When reserving Grid capacity on the grid the total pricing for reserved capacity will be calculated (week, month, quarter of annual) and translated against the currect token value.  The amount of tokens required to reserve the same capacity might vary based on the token value.   A higher token value provides you more ThreeFold capacity purchase power.  A lower price result in lesser.

**Question** The information we have seems to indicate that individual farmers set the price of their own capacity.  Do they set a price in terms of tokens, or in terms of fiat currency?  Either way, how do fluctuations impact the business of the farmers?

Farmer set their own pricing in **fiat** currency.  Capacity reservations are paid for in token so a higher value of the token will provide them with less tokens than when there is a lower token value.  Farmers have the freedom to change tokens to fiat when they believe they need to get fiat for business reasons or might sit on tokens to let them appreciate.

**Question** If the token price relative to fiat currency fluctuates rapidly, how do the small-scale farmers in particular regulate the cost of their capacity?  It seems to me that it would be very useful if there were a baseline price for farming capacity that is somehow automatically adjusted by the ThreeFold OS to follow a constant price relative to fiat currency in order to allow farmers to have a “hands-off” management of their own capacity. Then it might be useful to allow farmers to set the price of their capacity in terms of a multiplicative factor times this baseline price.

There is baseline pricing for farmers.  For farmers that have no idea or do not want to get involved in setting pricing for their capacity there is a defults pricing options set in the TF Grid.  As discussed before - capacity pricing is set in fiat and therefore no adjustment is needed when token pricing fluctuates.

**Question** How would an application that is intended for a mobile device negotiate prices with the various ThreeFold farmers as it roams around? This situation especially would require some automatic system-wide pricing.  It will be nearly impossible for a provider to negotiate individually with thousands (or eventually millions) of individual farmers.

**Answer:** The TreeFold grid will have a directory (TF Directory) that allows current and future user to search capacity based on search criteria.  The search criteria are still have to be defined but will include things like:

 - cloud unit pricing
 - capapcity geo-location
 - the service level guaranteed and achieved
 - some form of feedback on the performance of the farmners capacity used by others

### How will we implement the ThreeFold Grid in developing countries?

**Question** The places where ThreeFold is most needed are under-served regions that typically have minimal access to internet, if they have any access at all.  In these locations it would be necessary to improve the internet infrastructure first (i.e., more and better routers and backbone).  Furthermore, electric power is not reliable in these locations, compounding the problem of establishing a reliable ThreeFold grid there.  Are there ideas on how to surmount these challenges?

**Answer:** A lot of ideas - not of them have been executed yet.  ThreeFold foundation has been speaking with other startups and companies that are actually rolling out local m,obile and fixed networks.  Companies are actually investing a lot in these areas to bring mobile connectivity and data and we should be speaking to the telecoms operators and see how we can work with them to deploy internet connectivity to these homes and users or to work with the operator to deploy capacity in the telecommunication operators  infrastructure.

### Where best to concentrate our initial efforts to promote the ThreeFolf Grid?

**Question:** With respect to emerging markets / developing countries, how does it makes sense for ThreeFold to be in the business of lobbying governments or private companies to install the infrastructure needed to make ThreeFold viable? This is an admirable aspiration but in terms of getting traction it seems best to focus initially on locations where the infrastructure works well.

**Answer:**  We need to do both.  Please consider approaching the larger organisations and governments with a story about doing good (bringing the actual capacity to the country or region) and creating a significant earling model for them by doing so.  So it's an option to do good and create an earning model at the same time.

To approach the individuals and provide them with a money making project requires certain things to be in place.  There is no way around having to have a form of reliable electricity and network.  Having said that there might be some very smart people out there that will come up with inventive way to guarantee power and network.  Car batteries being used as uninterrupted power supplies, HAM radio's and Lora to get to the next internet point of presence (POP)

### How do small-scale farmers complete with farmers with more extensive capacity?

**Question:** Since software performance is a function of the applications being run, the hardware requirements of a software application (internet speed, compute performance, storage capacity, security) place demands on the capacity of the ThreeFold grid. How do farmers configure their hardware in order to satisfy what a consumer or business might need. Will small-scale farmers be shut out from clients either because they cannot provide sufficient capacity for the most common applications, or because the larger nearby farmers can run a more profitable service because of their scale of operation?

**Answer:** Initially we will be presenting [unmanaged](https://github.com/threefoldfoundation/info_foundation/blob/master/docs/definitions/threefold_unmanaged_capacity.md) capacity only.  This unmanaged capacity will presented by farmers from homes, offices, no datacenter locations and datacenter locations.  Everyone will be presenting the same type of capacity at the start in smaller or larger quantities.  So this is not a problem initially.

### How are ambassadors to promote the development of applications to run on the Threefold Grid.

**Question:** The ThreeFold network/solution is described as “computing at the edge”; a low-cost, energy-efficient computing solution offered close to where consumers and businesses are. It is meant to be an alternative to the likes of Amazon Web Services (AWS) where today you can buy a slice of their stack, including certain applications such as their e-commerce engine, plus the inherent security they offer for $x/month. Users of AWS can add their own specific solutions and integrate them within Amazon’s architecture. So with that said, how do consumers or businesses add their applications/solutions on to the ThreeFold network? What applications, if any, is ThreeFold offering? Is there any thought of encouraging companies like Amazon to migrate some of their services to the ThreeFold grid?

### Will ThreeFold be able to restrict malicious content?

**Question:** In the same way FaceBook and other social media platforms are getting hammered for privacy-related issues, will DigitalMe as implemented on the ThreeFold grid ensure user

**Answer:** DigitalMe will guarantee user privacy by allowing the user to 100% control what information is shared with whome.

**Question:** What is ThreeFold doing to ensure that the platform cannot be used to promote dangerous, hateful, offensive content? Side note: YouTube has a whole group of people who spend their entire days reviewing content to try to ensure its platform is not used to promote hateful, despicable content. ThreeFold‘s motives may be pure, but the bad guys may think it is a great “under the radar” platform to help them evangelize their point-of-view. Is it better to have a completely hands-off neutral system and accept the fact that there may be some bad players out there using it as a cost of the neutrality?

**Question:** All of the capacity that exists and will grow is owned by Farmers, not ThreeFold.  Therefore ThreeFold is not involved in any of the operational processes of the ThreeFold grid.  It cannot and will not control the content on the grid, it will not control and intervene with the applications on the grid.

### Is there a conflict between the distributed Grid and pricing of service by individual farmers?

**Question:**  If individual farmers do set the price of tokens, will pricing of service by farmers be available for all to see? If I find that tokens are cheaper in eastern Europe compared to California where I live, I may choose to buy capacity from the eastern Europe cooperative.

**Answer:** As discussed earlier:

The mechanism here is as follows:
 - Token value is determined by demand and supply on token markets by token holders selling their tokens and token buyers.
 - ThreeFold grid capacity pricing is _set_ by Farmers in **fiat** currency and made public by the TreeFold directory.

 Pricing of tokens will differ between exchanges and people selling token in other ways.  Capacity pricing will differ in fiat as well.  Purchasing tokens in remote exchanges or markets is fine and does not upset the distributed character of the grid at all.  See it similar to buying dollars or Euros therefore following the same rules and processes as fiat currencies having different pricing in different markets.

**Question:** How can I be assured of performance?

**Answer:** Performance is being measured by the TF Chain and reported.  The TF Chain also allows for a "social ranking" by capacity users which provides actual user experiences.

**Question:** How does this model lead to an increase in the value of tokens over time…especially if consumers decide to buy from whomever is offering the cheapest capacity?

**Answer:** The value of the token will increase by the token being traded in token markets.  The normal demand and supply mechanism will determine the token pricing.  As the supply is only driven by Farmers that put capacity online and the demand is driven by a lot of different groups:
 - people that need tokens to reserve

**Question:** ARE [ATOMIC SWAP](https://cointelegraph.com/news/decentralized-exchanges-off-chain-atomic-swaps-and-a-brief-look-into-the-future) EXCHANGES A PROVEN TECHNOLOGY? Atomic
swap exchanges sound like a great idea, do they exist yet and are they proven? This article seems to suggest they are still under development with many challenges to be overcome.
**Answer:**

### What can be the impact of Government Regulation of cryptocurrencies?

Governments lag behind technology innovation, but is it fair to assume that they will step in to regulate crypto currencies or potentially even decide to do their own? What if the US Government introduces a digital dollar, what might be the likely impact will be on ThreeFold tokens? If that happened why would anyone need tokens if they can simply trade in a digital version of their own fiat currency? Would national digital dollar be a good candidate for a managed ThreeFold system? Could ThreeFold token exchanges be taxed, for example, to provide funds for public services?

The ThreeFold token is has the following characteristics:
 - it is backed by the the gold of the digital age:  internet processing and storage Capacity
 - it is green token - no dirty mining as the TF Chain runs proof of stake blockchain technology
