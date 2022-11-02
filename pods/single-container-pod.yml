apiVersion: v1
kind: Pod
metadata:
  name: my-pod1
spec:
  containers:
    - name: cont-1
      image: ubuntu
      command: ["/bin/bash", "-c", "while true; do echo Hi everyone; sleep 5 ; done"]
  restartPolicy: Never         # Defaults to Always
