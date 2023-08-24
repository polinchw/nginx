# Nginx Helm Chart

# Description

This helm chart will run nginx in a Kubernetes statefulset.

## Installation instructions

```helm install nginx .```

## Delete helm chart

```helm delete nginx```

## Add html files

Shell into nginx pod an place you htmls under this directory:

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