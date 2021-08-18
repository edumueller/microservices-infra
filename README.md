# Commands

## Updating a deployment

1. Deployment must be using "latest" tag in the pod spec section
2. Make an update to the code
3. Build the image
4. Push the image to docker hub
5. Run the command `kubectl rollout restart deployment [depl_name]`

## Configuring nginx-ingress

https://kubernetes.github.io/ingress-nginx/deploy/#provider-specific-steps

In Windows and Mac, run the following command (see the above link for more info):

- `kubectl apply -f https://raw.githubusercontent.com/kubernetes/ingress-nginx/controller-v0.48.1/deploy/static/provider/cloud/deploy.yaml`

## hosts file

Change your dev environment's hosts file to redirect requests made to posts.com to 127.0.0.1.

Add the following line to your /etc/hosts file:

`127.0.0.1 posts.com`
