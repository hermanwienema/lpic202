# lpic202
Course material

Use ubuntu and install docker before running the ldap.sh script:

<code>sudo apt install docker.io</code>

1.) Searching for LDAP object:

<code>ldapsearch -b 'dc=example, dc=com' '(objectclass=*)'</code>
  
2.) Add 
<code>ldapadd -x -D "cn=admin,dc=example,dc=com" -w password -H ldap:// -f newgroups.ldif</code>
