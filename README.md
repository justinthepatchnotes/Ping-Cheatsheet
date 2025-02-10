# Ping Cheatsheet

The ` ping` command is a network diagnostic tool used to test connectivity between your computer and a specified host (such as a website or another device ) 

- It helps diagnose network issues such as latency, packet loss, and unreachable hosts.

![ping](https://i.imgur.com/w2I9SgH.png)

## Basic Ping Commands 

## Ping with a Specific Number Of Packets

example : ``` ping -w [Number of Packets][destination]``` 

 ``` ping -n 5 justinthepatchnotes.com ``` 
 
 Sends 5 packets instead of running indefinitely.

 ![ping](https://i.imgur.com/BKqPUbR.png)


## Ping with a Specific Packet Size

example : ``` ping -l [packet size][destination]``` 


``` ping -l 1000 justinthepatchnotes.com ``` 

Sends packets of 1000 bytes instead of the default 32 bytes.

![ping](https://i.imgur.com/hmsGZ4T.png)

## Ping Until a Timeout (in Milliseconds)
  
example : ``` ping -w [timeout][destination]``` 

``` ping -w 5000 justinthepatchnotes.com ```

This waits up to 5000 ms (5 seconds) for each response before timing out.

![ping](https://i.imgur.com/mhj4E0u.png)

## Ping a Local Network Device 
``` ping [Your Local Device IP Address] ``` 

Useful for testing connections to routers, printers, or other networked devices. 

## Ping an IPv6 Address

example : ``` ping -6 [ipv6].[destination]``` 

``` ping -6 ipv6.google.com ``` 

Tests connectivity using IPv6.

![ping](https://i.imgur.com/TerJbDs.png)


## Ping with No Reverse DNS Lookup
example : ``` ping -4[destination]``` 

``` ping -4 google.com``` 

Forces IPv4 and skips resolving the hostname, speeding up the test.

 
![ping](https://i.imgur.com/eZev4fL.png)


## Continuous Ping (Useful for Monitoring)

example : ``` ping -t[destination]``` 

``` ping -t google.com``` 

Pings indefinitely until manually stopped with ```Ctrl + C``` .

 
![ping](https://i.imgur.com/jWoLhon.png)
