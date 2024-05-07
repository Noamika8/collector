Hey !!! 

have you installed the weather app ??
if not , please go ahead and install it first before we proceed to the next part 

pre requisites :
1. install the weather app or any other app you want to trace
2. deploy Logz.io using helm chart on your cluster

The process:
1. clone locally all the files in this repo
2. run the following command from the files location as you are connected to the target kubernetes cluster : "create configmap otel-collector-config --from-file=/your/path/config.yaml" - change the path to your local path.
3. then you can deploy the tracing collector using the commands :
4. "kubectl apply -f deployment.yaml                                                                                                                                                                                                                   ─╯
kubectl apply -f service.yaml
kubectl apply -f secret.yaml"

Usfull links I used during this project : 
1. https://logz.io/blog/nodejs-javascript-opentelemetry-auto-instrumentation/#jaeger
2. https://opentelemetry.io/docs/collector/installation/
3. chatgpt


