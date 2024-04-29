# Jifeng Chen's 6.2C: Cloud Native Application Development Interacting with Kubernetes

This is the Jifeng Chen's implementation of SIT323 6.2C

To utilize this demonstration, please follow the steps below:

1. **Firstly**, verify the services are fully functioning
    ```bash
    kubectl get pods
    kubectl get services
    ```

2. **Next**, create a forwarding rule, change the "mydeployment-6d958b46cc-2blmm" to a specific pod name
    ```bash
    kubectl port-forward mydeployment-6d958b46cc-2blmm 9000:3040
    ```
3. **Finally**, test the following websites to check the execution of both two services
    http://localhost:9000/exponentiation?n1=10&n2=6 <br>
    http://localhost:9000/exponentiation?n1=10&n2=6

