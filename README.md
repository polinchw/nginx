# Nginx Helm Chart

# Description

This helm chart will run nginx in a Kubernetes statefulset.

## Installation instructions

```git clone https://github.com/polinchw/nginx```


```helm install nginx nginx```

## Delete helm chart

```helm delete nginx```

## Add html files

Shell into the nginx pod (web-0) and place you htmls under this directory:

/usr/share/nginx/html

For example create a directory /test under the /usr/share/nginx/html directory.

Create an index.html file in the /test directory

## Test the page

Update your /etc/host file with something like:

```
192.168.1.158    test.com
```

Point your browser to:

```
http://test.com/test
```

The index.html should load.