Actor Model is using most of the time for concurrent processing. Rails or any 
ruby server application can be deployed on top of that PaaS which can be 
configured to have multiple node actors & a supervisor on top of the nodes. 
Mailbox of the each actor will be responsible for communication in between actors.

The framework should have a mechanism to create, destroy new nodes based on the 
requirements. And nodes should be able to communicate between each other. 
Supervisor node should be notified when other nodes go down. A simple Ruby server
should be able to deploy on top of the framework.