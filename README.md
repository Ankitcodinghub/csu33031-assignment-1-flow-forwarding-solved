# csu33031-assignment-1-flow-forwarding-solved
**TO GET THIS SOLUTION VISIT:** [CSU33031 Assignment 1-Flow Forwarding Solved](https://www.ankitcodinghub.com/product/csu33031-assignment-1-flow-forwarding-solved/)


---

📩 **If you need this solution or have special requests:** **Email:** ankitcoding@gmail.com  
📱 **WhatsApp:** +1 419 877 7882  
📄 **Get a quote instantly using this form:** [Ask Homework Questions](https://www.ankitcodinghub.com/services/ask-homework-questions/)

*We deliver fast, professional, and affordable academic help.*

---

<h2>Description</h2>



<div class="kk-star-ratings kksr-auto kksr-align-center kksr-valign-top" data-payload="{&quot;align&quot;:&quot;center&quot;,&quot;id&quot;:&quot;90911&quot;,&quot;slug&quot;:&quot;default&quot;,&quot;valign&quot;:&quot;top&quot;,&quot;ignore&quot;:&quot;&quot;,&quot;reference&quot;:&quot;auto&quot;,&quot;class&quot;:&quot;&quot;,&quot;count&quot;:&quot;1&quot;,&quot;legendonly&quot;:&quot;&quot;,&quot;readonly&quot;:&quot;&quot;,&quot;score&quot;:&quot;5&quot;,&quot;starsonly&quot;:&quot;&quot;,&quot;best&quot;:&quot;5&quot;,&quot;gap&quot;:&quot;4&quot;,&quot;greet&quot;:&quot;Rate this product&quot;,&quot;legend&quot;:&quot;5\/5 - (1 vote)&quot;,&quot;size&quot;:&quot;24&quot;,&quot;title&quot;:&quot;CSU33031 Assignment 1-Flow Forwarding Solved&quot;,&quot;width&quot;:&quot;138&quot;,&quot;_legend&quot;:&quot;{score}\/{best} - ({count} {votes})&quot;,&quot;font_factor&quot;:&quot;1.25&quot;}">

<div class="kksr-stars">

<div class="kksr-stars-inactive">
            <div class="kksr-star" data-star="1" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="2" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="3" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="4" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" data-star="5" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>

<div class="kksr-stars-active" style="width: 138px;">
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
            <div class="kksr-star" style="padding-right: 4px">


<div class="kksr-icon" style="width: 24px; height: 24px;"></div>
        </div>
    </div>
</div>


<div class="kksr-legend" style="font-size: 19.2px;">
            5/5 - (1 vote)    </div>
    </div>
<div class="page" title="Page 1">
<div class="layoutArea">
<div class="column">
&nbsp;

1 Introduction

The focus of this assignment is to learn about decisions to forward flows of packets and the information that is kept at network devices that make forwarding decisions. The design of forwarding mechanisms aims to reduce the processing required by network elements that forward traffic while providing scalability and flexibility.

2 Protocol Details

Your are given the task to develop a replacement for IPv4 or IPv6 by designing a protocol that forwards payloads based on a collection of strings that identify the source and destination of traffic. The forwarding information will be kept in forwarding tables located at the individual network elements and the content of these tables will be controlled by a central controller.

Figure 1: An application will send UDP datagrams to a forwarding service on the local host. The forwarding service will consult a table to determine from the header informa- tion of your protocol where to forward the datagram to. The table will provide it with the IP address of the network element that is the next hop and your implementation should forward it to another instance of the forwarding service on this IP address.

The initial implementation of the forwarding mechanism will use a UDP service bound to port 51510 at every network element. Someone in future may use the same information that is currently transferred using

</div>
</div>
<div class="layoutArea">
<div class="column">
1

</div>
</div>
</div>
<div class="page" title="Page 2">
<div class="layoutArea">
<div class="column">
CSU33031 Flow Forwarding

</div>
</div>
<div class="layoutArea">
<div class="column">
UDP and send it, using Ethernet frames as a complete replacement to current IP protocols, as shown in figure 2 b) (see also the use of faces in NDN [1]).

An application using your protocol will create a header you design, attach the payload to be transmitted, and send it as payload to a service you develop, bound to port 51510 on the local host, such as shown in figure 2 a). The service will examine the header and decide where to forward the information to based on the header information and a forwarding table. The forwarding table will indicate instances of the service on other network elements.

An application that intends to receive traffic will send a datagram to the forwarding service on its local host, indicating that it intends to receive traffic for a given string. The forwarding service will need to record the port number of that the application used and the string. Whenever datagrams arrive for the given string, it should deliver these datagrams to the port number that is associated with the string.

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 2: An application will transmit a header and payload to a forwarding service bound to port 51510 on the local host. The forwarding service will inspect the header and forward the header and payload to a forwarding service on another network ele- ment.

The header information should be encoded as type-length-value (TLV) format. Figure /refTLVExample shows an example where the first number of the encoding gives the type of the information that follows, the second number gives the length of the information and the third item of the field provides the value of the information itself. The first example shows a field that could represent a network ID, the network has the length of 7 characters and the value ’trinity’. The second example combines two network IDs by introducing a type combination that can hold any combination of further TLVs, in this case two network IDs. This example allows for construction of hierarchical networkIDs such as ’trinity.scss’.

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 3: The 1st number of the encoding gives the type of the information that follows, the 2nd number gives the length of the information and the 3rd item of the field provides the value of the information itself. The 1st example shows a field that could represent a network ID, the network has the length of 7 characters and the value ’trinity’. The 2nd example combines two network IDs by introducing a type combination that can hold any combination of further TLVs, in this case two network IDs.

So, the basic functionality that a forwarding service has to provide is to accept incoming packets, inspect the header information, consult the forwarding table and forward the header and payload information to the

</div>
</div>
<div class="layoutArea">
<div class="column">
Page 2 of 5

</div>
</div>
</div>
<div class="page" title="Page 3">
<div class="layoutArea">
<div class="column">
CSU33031 Flow Forwarding

</div>
</div>
<div class="layoutArea">
<div class="column">
destination. In the first place, if a destination is not known, a forwarding service would drop an incoming packet; once a controller has been implemented, the forwarding service needs to contact the controller to enquire about a forwarding information to the unknown destination and if it receives forwarding information, integrate this into its forwarding table.

Figure 4: This example shows the forwarding of traffic with a label ’trinity’ from an endpoint E1 to an endpoint E4. The names E1, E4, and R1 to R4 should be replaced by IPv4 addresses. The forwarding information should be supplied to the network elements by a central controller

In general, the network elements should be controlled by a central controller that initializes the flow tables of the network elements and would inform them about routes to destinations as the network changes. In a first step though, in order to reduce complexity, the flow tables of the individual network elements should be hardcoded. The implementation of the controller element should only be pursued once the implementation of the forwarding functionality of the network elements is stable and allows for basic communication between two endpoints.

The Named Data Networking (NDN) protocol [1] and the OpenFlow protocol [6] are examples of similar protocols that you could look at for functionalities that may be interesting for you to include in your protocol. In the end, it is up to you what functionalities you implement in your protocol. In the deliverables, you need to describe these functionalities and justify why you included them in your protocol.

The following flow diagrams, figures 5 is an examples of visualizations of network traffic between network elements. It shows a sequence of messages exchanged between the elements.

Please use Flow Diagrams like these to document the communication between components of your imple- mentation in your videos and in your final report.

The protocol can be implemented in a programming language of your choosing. One of the conditions is that the communication between the processes is realized using UDP sockets and Datagrams. Please avoid Python 2.7 because the implementation of Datagram sockets in the obsolete versions is based the transfer of strings instead of binary arrays.

The easiest way to start with the development of your solution is possibly to connect your components through the localhost interface of a machine; however, at the end, you will need to be able to demonstrate that your protocol can connect components located at a number of hosts. There are a number of platforms that support the simulation of topologies or provide virtual infrastructures e.g. Docker [3], Mininet [7], Kubernetes [2], etc. For someone starting with socket programming and networking, I would suggest to use a platform such as Docker or Mininet; for someone already familiar with these concepts, I would suggest to implement their solution using Kubernetes. However, these are only suggestion and you need to make the decision how to implement your solution.

</div>
</div>
<div class="layoutArea">
<div class="column">
Page 3 of 5

</div>
</div>
</div>
<div class="page" title="Page 4">
<div class="layoutArea">
<div class="column">
CSU33031 Flow Forwarding

</div>
</div>
<div class="layoutArea">
<div class="column">
Figure 5: The diagram shows a router contacting the controller with an initial ’Hello’ message and receives a modification message to its flow table. It replies to this with an acknowledgement. When a router receives a packet with an unknown destination, it will contact the controller and receive an additional modification to its flow table

3 Deliverables &amp; Submission Details

The deliverables for this assignment are split into 3 parts: 2 videos, a report describing your solution and the files making up the implementation of your solution. The deadline for the submission of these deliverables are given in Blackboard.

One component of the deliverables at every step is the submission of captures of network traffic. These cap- tures should be in the form of PCAP files [4]. Programs such as Wireshark [5], tshark, etc offer functionality to capture network traffic from interfaces

3.1 Part 1: Video &amp; PCAP file

The video of part 1 should demonstrate the initial design of your solution and a capture of network traffic between the components of your solution and the files of your traffic capture in pcap format. In the video, you should explain the setup of the topology that you are using and the information that makes up the header information in your traffic captures.

The submission process for this part consists of two steps: 1) Submitting the PCAP file or files that you captured from your network traffic, and 2) submitting the video for this step.

The video is to be no longer than 4 minutes; content past the 4 minute-mark will be ignored during marking. Videos with voice-over using text-to-speech (TTS) will not be accepted and marked with 0.

3.2 Part 2: Video &amp; PCAP file

The video of part 2 should demonstrate the current state of your solution, the functionality that you have implemented so far, and a capture of network traffic between the components of your solution and the files of your traffic capture in pcap format. In the video, you should explain the basic implementation fo your protocol and the information that is being exchanged between the components of your solution.

The submission process for this part consists of two steps: 1) Submitting the PCAP file or files that you captured from your network traffic, and 2) submitting the video for this step.

Videos with voice-over using text-to-speech (TTS) will not be accepted and marked with 0. The video is to be no longer than 4 minutes; content past the 4 minute-mark will be ignored during marking.

</div>
</div>
<div class="layoutArea">
<div class="column">
Page 4 of 5

</div>
</div>
</div>
<div class="page" title="Page 5">
<div class="layoutArea">
<div class="column">
CSU33031 Flow Forwarding

</div>
</div>
<div class="layoutArea">
<div class="column">
3.3 Final Deliverable

The final deliverable should include a report that describes the components of your solution and their functionality, the protocol that you implemented and the communication between the components of your solution, the topology that you used to run you solution and how your solution was executed.

The submission process for this part consists of three steps: 1) Submitting the PCAP file or files that you captured from your network traffic, 2) submitting the source code and any files that may be necessary to execute your solution, and 3) submitting the report about your solution.

The files that contain the implementation and the report should be submitted through Blackboard. Every file should contain the name of the author and the student number. The source files of the implementation should be submitted as an archived file e.g. “.zip” or “.tar.gz”. The report should be submitted as either word- or pdf-document. The deadline for the submission is given in Blackboard.

The report may be submitted to services such as TurnItIn for plagiarism checks.

</div>
</div>
<div class="layoutArea">
<div class="column">
&nbsp;

</div>
</div>
</div>
