# openshift-clusters
# Managing Users with the HTPasswd Identity Provider
Creating the new file (htpasswd -c -B -b /tmp/htpasswd student redhat123)
Add or update credentials (htpasswd -b /tmp/htpasswd student redhat1234)
Delete credentials (htpasswd -D /tmp/htpasswd student)
Creating the HTPasswd (oc create secret generic htpasswd-secret \ --from-file htpasswd=/tmp/htpasswd -n openshift-config)
