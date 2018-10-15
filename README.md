### RSVP Application

This deployes a sample RSVP application provided [here](https://raw.githubusercontent.com/cloudyuga/rsvpapp/master/rsvp.py). Users are allowed to  register for an event once a username and email id are provided. These get saved in a MongoDB database. The application consists of a backend database and a frontend. For the backend, uses a MongoDB database, and for the frontend, we have a Python Flask-based application.


![Application](rsvp.png)


### Run Application

- Install [minikube](https://github.com/kubernetes/minikube/releases)
- Clone this repository
- From the kubernetes directory run the following:
  - kubectl create -f mongo-db.yaml
  - kubectl create -f mongo-service.yaml
  - kubectl create -f web-service.yaml
  - kubectl create of web-frontend.yaml
  
- run **minikube ip**
- get the ip address and open it in a web-browser with the nodePort for the web-service
