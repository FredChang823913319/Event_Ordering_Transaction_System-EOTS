# event_ordering_transaction_system

Introduction
=============
<p>we built up a transaction system with up to 9 ATMs working in the same time. In the logger, events, time delay and bandwidth are recorded in order so as to plot the graphs representing the relationship among these clients. In each terminal, the balance of all users would be printed out.</p>

Code Implementation
=============
ATMs:
<p>Each ATM file(mp1_node.go) consists of 3 parts:
1. When events happen in its own ATM, it multicast to all other processes (Acting like a server, main function)
2. Handle connection among all other ATMs (Acting like a client) 3. Error Detection Subroutine
</p>


<p>Running instruction:</p>

<pre><code>go build mp1_node.go && python3 –u gentx.py 0.5| ./mp1_node [number of nodes running] [port number]
</code></pre>
