apiVersion: v1
kind: Service
metadata:
    name: mygame-svc
spec:
    selector:
       app: webapp-ws
     ports:
       -protocol: TCP
        port: 80
        targetPort: 80
      type: LoadBalancer
