## Google Cloud VPC Network Peering to Connect Two VMs and Check Nginx Server Access.

### Description

Explore hands-on VPC network peering within Google Cloud Platform (GCP). We'll create separate VPCs in different regions, set up VMs in each VPC, and deploy an Nginx server. Witness the practical dynamics of VPC network peering as these elements interact, gaining real-world insights into this powerful GCP feature.

### Overview Diagram

<figure > 
<p align="center">
  <img src="./assets/vpc-peering-overview.png" alt="vpc-peering-overview" style="background-color:white" />
</p>
</figure>

### Prerequisites

- Google Cloud Platform(GCP) account or playground.
- Knowledge about VPC, VM instance, Subnet, Network interface.

### Step-1: Create Two VPCs:

<details>
<summary>Creating <code>vpc-1</code></summary><br/>
<img src="./assets/vpc/vpc1-1.png" alt="vpc1-1"/>
<img src="./assets/vpc/vpc1-2.png" alt="vpc1-2"/>
<img src="./assets/vpc/vpc1-3.png" alt="vpc1-3"/>
<img src="./assets/vpc/vpc1-4.png" alt="vpc1-4"/>
</details>

<details>
<summary>Creating <code>vpc-2</code></summary><br/>
<img src="./assets/vpc/vpc2-1.png" alt="vpc1-1"/>
<img src="./assets/vpc/vpc2-2.png" alt="vpc1-2"/>
<img src="./assets/vpc/vpc2-3.png" alt="vpc1-3"/>
<img src="./assets/vpc/vpc2-4.png" alt="vpc1-4"/>
</details>

### Step-2: Create Two VMs:

<details>
<summary>Creating <code>vm-1</code></summary><br/>
<img src="./assets/vm/vm1-1.png" alt="vm1-1"/>
<img src="./assets/vm/vm1-2.png" alt="vm1-2"/>
<img src="./assets/vm/vm1-3.png" alt="vm1-3"/>
<img src="./assets/vm/vm1-4.png" alt="vm1-4"/>
<img src="./assets/vm/vm1-5.png" alt="vm1-5"/>
</details>

<details>
<summary>Creating <code>vm-2</code></summary><br/>
<img src="./assets/vm/vm2-1.png" alt="vm2-1"/>
<img src="./assets/vm/vm2-2.png" alt="vm2-2"/>
<img src="./assets/vm/vm2-3.png" alt="vm2-3"/>
<img src="./assets/vm/vm2-4.png" alt="vm2-4"/>
<img src="./assets/vm/vm2-5.png" alt="vm2-5"/>
</details>

### Step-3: Peering Two VPC:

<details>
<summary>Peering <code>vpc-1</code> to <code>vpc-2</code></summary><br/>
<img src="./assets/peer/peer1.png" alt="peer-1"/>
</details>

<details>
<summary>Peering <code>vpc-2</code> to <code>vpc-1</code></summary><br/>
<img src="./assets/peer/peer2.png" alt="peer-2"/>
</details>

### Step-4: Check Connection:

Now if we try to connect from vm-1 to the vm-2, it will be connected now.

<details>
<summary>Ping from <code>vpc-1</code> to <code>vpc-2</code></summary><br/>
<img src="./assets/peer/check-connection.png" alt="peer-1"/>
</details>
