Components and Their Purpose
    Control Plane:
         The brain of the Kubernetes cluster. It maintains the desired state of the cluster by managing the scheduling and scaling of applications.
    kubectl: 
        CLI tool to interact with the Kubernetes API server for cluster management.
    Secrets:
         Stores sensitive data such as passwords, tokens, and keys.
    Config (ConfigMap):
         Stores non-sensitive configuration data for applications.
    Deployments:
        MongoDB Deployment: Manages MongoDB container instances.
    Web App Deployment: 
        Manages web application container instances.
    Services:
        MongoDB Service:
             Exposes MongoDB deployment internally within the cluster.
        NodePort Service:
             Exposes web application deployment externally, accessible from outside the cluster on a specified port.





-Yaml ma Kind vaneko kun component of kubernetes such as deployment ho ki secret ho ki configmap ho ki and so on 

--- = break garna yaml , naya banxa tyo tala as chuttai yaml file jastai 

1.Secrets = Different webapp , mongoapp, prosgreapp all should have different secrete yaml file for different cod 

2.ConfigMaps = Non-confidential data rakhna lai , URl rakhxa jastai database url , ConfigMaps is usually or mostly for Database as database outside of kubernetes rakhxan such mongodbatlas , AWS 


3.Deployments =  replication and also called abstract of pods , blueprint hunxa actual replica haina ( Container ko data sabai asma spec garnu parxa , contrainer ko abstraction pod ho , pod ko abstraction deployment)


4.Serivce= Internet ma expose garna lai use hunxa using NodePort, Pod keep on dying , so service provide permanent ip add, also experntal sanga expose garna we user service , also service work as a load balancer 


5. --- paxi ko chuttai file ma rakhna sakinxa but sano project ma we can use ahutai file ma , Here selector le kun sanga comminute garney vanera chosee garna lai use huxna 


important = Minikube le setup matra gardiney ho sabai download gaera , cluster banayera , and so on cpu ram milauney , run ko lagi all 
BUT we do not worki with minikune once we run minikube start WE will use kubectl that is used after we run minikube start



APPLY in KUBECTL is must important 