#Build your execution environnment image
ansible-builder build -v3 --tag=vmware-ee

#Fetch the image ID of your newly built image
podman images

#Push your container image to a registry
podman push <container-id> quay.io/your_username/image_name:tag


