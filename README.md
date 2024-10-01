Amazon EKS is a managed Kubernetes service to run Kubernetes in the AWS cloud. Amazon EKS automatically manages the availability and scalability of the Kubernetes control plane nodes responsible for scheduling containers, managing application availability and storing cluster data.

2048 game: 2048 is a single-player sliding tile puzzle video game written by Italian web developer Gabriele Cirulli and published on GitHub. The objective of the game is to slide numbered tiles on a grid to combine them to create a tile with the number 2048

In this video, I am demonstrating how the 2048 game (container based) can be deployed on to a simple Kubernetes cluster. It shows mainly 4 steps
1. Create the EKS cluster
2. Create a node group within the cluster
3. Create a POD which will run containers with 2048 game container image. Config file is written using YAML.
4. Create a Load Balancer service (ingress controller service) so that the game app can be accessed from outside using the Load balancer’s DNS name


Note:
Please note that the EKS cluster is not free. So, there will be a nominal charge if you keep it open for a couple of hours. Besides, you will be using t3.medium EC2 in the node group. So, there will be some nominal charge for that resource as well.
