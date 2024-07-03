# Google-Cloud-VM-and-Networks-Load-Balancing

![image](https://github.com/iahalkhatib/Google-Cloud-VM-and-Networks-Load-Balancing/assets/170050432/3fd0751d-2a21-4735-a537-0ef0d2d6d6db)

# Cloud Load Balancing in Google Cloud

Overview of Cloud Load Balancing

Cloud Load Balancing is a fully distributed, software-defined, managed service designed to handle all your traffic. 
It distributes user traffic across multiple instances of an application, ensuring performance consistency and reducing the risk of performance issues.

# Key Features

Fully Managed Service:

No need to manage or scale load balancers.
Works for HTTP, HTTPS, TCP, SSL, and UDP traffic.
Cross-Region Load Balancing:

Provides automatic multi-region failover.
Smoothly shifts traffic if backends become unhealthy.
Quick Reaction to Changes:

Adjusts to user traffic, network conditions, and backend health in real-time.
No pre-warming required for handling large spikes in demand.

# Types of Load Balancers

Global Load Balancers:

Global HTTP(S) Load Balancer: Ideal for web applications requiring cross-regional load balancing.
Global SSL Proxy Load Balancer: For secure sockets layer (SSL) traffic that is not HTTP.
Global TCP Proxy Load Balancer: For TCP traffic without SSL.

# Regional Load Balancers:

Regional External Passthrough Network Load Balancer: Balances UDP traffic or traffic on any port within a region.
Regional External Application Load Balancer: For application layer load balancing within a region.
Regional Proxy Network Load Balancer: For network layer load balancing within a region.

# Internal Load Balancers:

Regional Internal Load Balancer: Balances traffic within a project, between different layers of an application.
Cross-Region Internal Load Balancer: A Layer 7 load balancer for globally distributed backend services.

# Key Terminology

Load Balancer: A device that distributes network or application traffic across multiple servers to ensure no single server becomes overwhelmed.

Cross-Region Load Balancing: The ability to distribute traffic across different geographic regions.

Pre-Warming: A process required by some load balancers to prepare for a large increase in traffic; not required by Google Cloud Load Balancing.

Layer 7 Load Balancer: A load balancer that operates at the application layer (Layer 7) of the OSI model, capable of inspecting traffic content.

# Which type of load balancer should you use for balancing HTTP traffic across multiple regions?

A) Regional External Passthrough Network Load Balancer
B) Global HTTP(S) Load Balancer
C) Global TCP Proxy Load Balancer
D) Regional Internal Load Balancer

Correct Answer: B) Global HTTP(S) Load Balancer
Explanation: The Global HTTP(S) Load Balancer is specifically designed for handling HTTP traffic across multiple regions.

# What is a primary advantage of Cloud Load Balancing over traditional load balancers?

A) Requires pre-warming
B) Manual scaling required
C) Fully managed service with no need for user intervention
D) Limited to specific traffic types

Correct Answer: C) Fully managed service with no need for user intervention
Explanation: Cloud Load Balancing is a fully managed service, eliminating the need for users to manage or scale the load balancers themselves.

# Which load balancer would you use for UDP traffic across a region?

A) Global SSL Proxy Load Balancer
B) Regional External Passthrough Network Load Balancer
C) Regional Internal Load Balancer
D) Global TCP Proxy Load Balancer

Correct Answer: B) Regional External Passthrough Network Load Balancer
Explanation: The Regional External Passthrough Network Load Balancer is suitable for balancing UDP traffic across a specific region.
