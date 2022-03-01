# minikube
# REF: https://minikube.sigs.k8s.io/docs/start/

export tx=ubuntu@119.28.116.234
k8s_test


# nginx image
FROM nginx

docker build -t nginx .

# minikube deploy service 

export new_pod='test-nginx'
export app_image='nginx'
export app_port='80'
export app_out_port='8001'

kubectl create deployment $new_pod --image=$app_image
kubectl expose deployment $new_pod --type=NodePort --port=$app_port

kubectl get services $new_pod
minikube service $new_pod

kubectl port-forward --address 0.0.0.0 service/$new_pod $app_out_port:$app_port




