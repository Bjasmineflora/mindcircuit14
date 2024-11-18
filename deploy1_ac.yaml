---
apiVersion: apps/v1
kind: Deployment
metadata:
  name: fbdeploy
  labels:
    app: facebook
    env: sbox
spec:
  selector:
    matchLabels:
      app: facebook
  replicas: 3
  template: 
    metadata:
      name: fbpod
      labels:
        app: facebook
        env: sbox
        version: AC_V1
    spec:
      containers:
        - name: fbcont
          image: bjasmine/jasdevopshub_batch14:mcappimg
          ports:
            - containerPort: 8080
