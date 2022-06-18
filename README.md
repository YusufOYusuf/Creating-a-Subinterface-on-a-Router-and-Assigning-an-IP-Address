<h1>Creating a Subinterface on a Router and Assigning an IP Address</h1>


<h2>Description</h2>
In this lab, I learned to create a subinterface on a router and assign an IP address to it. A subinterface is a virtual interface on a signle physical interface. This is a handy interface capability supported by most router and switch manufacturers that allows you to create many virtual interfaces out of a single physical interface.
<br />



<h2>Environments Used </h2>

- <b>Ubuntu 20.04.2 LTS</b> 

<h2>Languages and Utilities</h2>

- <b>PuTTY SSH Client</b>
- <b>Terminal Window</b>

<h2>Program walk-through:</h2>

<p align="center">
From the left sidebar, click the PuTTY SSH Client icon: <br/>
<img src="https://i.postimg.cc/sXs0MCG1/Screen-Shot-2022-06-17-at-5-14-13-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
<br />
In the PuTTY Configuration dialog box, perform:  <br/>
  <br> 1. Type Host Name as 172.16.43.128</br>
  <br> 2. Type port as 5005</br>
  <br> 3. Under connection type, select the Telnet radio button</br>
  <br> 4. Click Open to connect </br>
<img src="https://i.postimg.cc/VL8557Dp/Screen-Shot-2022-06-17-at-5-12-22-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In R1 terminal window , execute the following commands to create a subinterface and assign an IP address: <br/>
<br> 1. configure terminal </br>
<br> 2. interface e1/0 </br>
<br> 3. ip address 10.10.10.10 255.255.255.0</br>
<br> 4. no shutdown</br>
<img src="https://i.postimg.cc/dt57X2jf/Screen-Shot-2022-06-17-at-5-16-49-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
<br />
In the R1 terminal window, exceute the following command to show the IP address assigned to the e1/0 interface:  <br/>
<br> 1. do show ip interface brief</br>
<img src="https://i.postimg.cc/Sx5G0FfH/Screen-Shot-2022-06-17-at-5-18-57-PM.png" height="80%" width="80%" alt="Creating a Subinterface on a Router and Assigning an IP Address Steps"/>
<br />
  
  
  
</p>

<!--
 ```diff
- text in red
+ text in green
! text in orange
# text in gray
@@ text in purple (and bold)@@
```
--!>
