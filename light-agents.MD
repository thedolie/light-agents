# Light Agents

## Overview

This document describes a protocol for the creation of "light agents". What they are, how to authenticate them, and what the implications of such a mechanism might include.

## Light Agents

### What is a light agent?

Indy agents have DID's, key management, adhere to certain protocols, etc. Simply put light agents aren't restricted to these protocols, and instead they operate as **extenstions** of a full indy-agent. Think of them as a remote device issuing commands to a module. For example a remote to a TV set, or in agent land a remote web page that issues commands to a full indy-agent living on a server or device. This "agent" does not have full functionality but can issue commands to an entitiy that does have full functionality.

### Why do we need light agents?

Agents are an amazing idea, but like many pieces of software they have limitatations. One of the biggest limiations of an agent is execution environment. 

For example: Lets take the scenario when Alice may need to form a pairwise relationship with Bob. In typical agent land this may not be too difficult with the protocols we have laid out as a community, but Alice has special circumstances: She lives in a 3rd world nation and has very limited access to smart devices and computers powerful enough to do anything more than simply open a web browser session and execute very simple javascript code. Alice does not have a smart phone, and does not have a mobile wallet. She simply does not have the resources to set up a mobile agent. 

Lets say we continue to extend this scenario and assume Alice is very fortunate and happens to have well connected family members that are able to get Alice a cloud agent to store her credentials. She is fortunate, but still is unable to access it as she does not have a mobile agent, and only has very limited access to the internet where she lives. Now Alice meets Bob and really wants to form a pairwise relationship between her cloud agent and bob's cloud agent. Alice simply needs to issue a remote command to her edge agent (in the cloud), and do it in a highly secure, authenticated, and highly trusted way. In this scenario Alice could, if she had the a mechanism to do so, execute a command from a **web page**, which is the only real device she does have access to, and form a pairwise relationship with Bob. This mechanism should recieve an update when the command has been executed and both parties can be highly satisfied and confident it was done according to agent governed protocols. This is where light agents come to the rescue.

## Authentication

The single most critical piece of any remote device whether a tv, mouse, etc is a protocol that ensures that when being commanded to issue something it is allowed to do so. 