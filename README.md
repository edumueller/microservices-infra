# Commands

## Updating a deployment

1. Deployment must be using "latest" tag in the pod spec section
2. Make an update to the code
3. Build the image
4. Push the image to docker hub
5. Run the command `kubectl rollout restart deployment [depl_name]`
