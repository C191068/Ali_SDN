# Ali_SDN

![s2](https://github.com/C191068/Ali_SDN/assets/89090776/d78fc224-3f94-49ff-aef9-2476145e0d72)

traditional network interconnects multiple networks using routers <br>

![s3](https://github.com/C191068/Ali_SDN/assets/89090776/61992f08-f2a3-410e-8bd5-a75b3c31bd8c)

imagine computer A wants to sent data to computer B

the roter device or router primarily does two functions <br>
 on a very high level <br>

 ![s4](https://github.com/C191068/Ali_SDN/assets/89090776/f54a33bd-b6d5-40a6-9a6f-213b0661b446)

 the first one is to decide the best path to take data from computer A to computer B <br>

which will help to learn network topology and update the routing table <br>

![s5](https://github.com/C191068/Ali_SDN/assets/89090776/904ed5ea-75cd-4486-808c-22f76e5e048d)


this function is performed by control plane <br>


![s6](https://github.com/C191068/Ali_SDN/assets/89090776/baef3762-8724-4b80-9c38-e737dc6c568f)

the second function is to forward actual data packets to next device <br>

based on the address of the destination machine <br>


![s7](https://github.com/C191068/Ali_SDN/assets/89090776/936bd139-fb6f-4d33-9eb4-1eacda171045)

this function is performed by data plane <br>

traditional router have both data plane and control plane function running at the same hardware <br>

mostly they are proprietary hardware and software are provided by vendors <br>

Proprietary hardware refers to computer or electronic hardware that is designed, manufactured, and controlled by a specific company or organization. It means that the hardware is not made by multiple manufacturers or available for use by anyone; instead, it is exclusive to the company that created it.<br>

Imagine you have a special toy that only works with batteries made by the same toy company, and you can't use regular batteries from the store. That toy's batteries are like proprietary hardware – they are unique and can only be used with that specific toy.<br>

Similarly, proprietary hardware can only work with specific software or accessories provided by the same company. This exclusivity can limit your options and potentially make it more expensive to maintain or upgrade your hardware because you're tied to that one company's ecosystem.<br>


so a network administrators will have to learn technology developed by different vendors and configure  <br>
each devices in atraditional network <br>


In Software defined network(SDN) it separates control plane from data plane <br>


![s8](https://github.com/C191068/Ali_SDN/assets/89090776/7c3b543e-6b22-40f6-ab2a-ad5b0c650006)


the SDN switches just perfomed the data plane function of forwarding packets to next device  <br>

so it can run on less expensive hardware <br>

![s9](https://github.com/C191068/Ali_SDN/assets/89090776/a42721c8-6de0-4623-97fb-32c14d313d67)

the control plane function is managed by contoller <br>

the priamary function of this controller is to identify the route <br>

and update the the flow table in the SDN switches <br>

the controller talk to the switches using a protocol called OpenFlow <br>


![s10](https://github.com/C191068/Ali_SDN/assets/89090776/802ad479-60a1-4845-9f62-67d6f9c9e927)

the controller can talk to thse SDN switches through OpenFlow APIs <br>


![s11](https://github.com/C191068/Ali_SDN/assets/89090776/f33a6630-67f3-46dc-8861-58c12f65fca5)


and can update the flow table entries in each of thses SDN switches <br>


these APIs are called southbound APIs <br>


so the controller use these southbound APIs to update thse SDN switches <br>



![s12](https://github.com/C191068/Ali_SDN/assets/89090776/51dfd162-341d-4d24-a494-d19434e690c5)


the controller also provide APIs for application to communicate <br>




these APIs are called Northbound API <br>



so the application can provide dynamically instructions to controller <br>

and controller can update the SDN switches <br>


So now a developer can write applications that can configure <br>

network in real time based on business requirement <br>


![s13](https://github.com/C191068/Ali_SDN/assets/89090776/46a5fbb9-0638-4e8c-ba88-759eeb2b8751)

imagine an application that uses video streaming <br>

It is a very critical application and video traffic has to be priotirize <br>


In SDN an application can use Northbound APIs to send the instruction to controller<br>

and controller can update those switches accordingly <br>

so that the application can prioterize video streaming and other traffics like VoIP <br>

![s14](https://github.com/C191068/Ali_SDN/assets/89090776/fc711242-3764-42be-88e3-23ac216b8ee5)

the controller provides an abstraction layer for the application <br>

the application need not know the complexity of the actual network infrastructure <br>

it can just provide intstruction the controller <br>

and controller can take care of updating actual physical ntework infrastucture <br>

These open controllers can run on any virtual machine <br>

so there is no requirement of purchasing a proprietary hardware for running a controller <br>

Developers can run the application on any virtual machine and provide intructions <br>

to controllers <br>


What if the operating system on which the application runs get compromised  <br>
and a bad actor gets acces to the application <br>

by compromosing the application the bad guys may get acces to your entire network <br>


![s15](https://github.com/C191068/Ali_SDN/assets/89090776/f11a2091-a3b9-479d-903e-d7ff57854b76)



because application can instruct the controller can upadte the network infrastructure <br>

so adequate security should be implemented on applications and physical network infrastructure <br>














































Most of these routers run protocols like OSPF <br>















 

 


















https://github.com/GNS3/gns3-registry/tree/master/docker

![s1](https://github.com/C191068/Ali_SDN/assets/89090776/5778b935-6fdd-4d82-adcd-63b0d2a86f05)


SDN implemenataion contoller <br>


