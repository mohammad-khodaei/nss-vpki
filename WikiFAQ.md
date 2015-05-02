# Introduction #

Here, some of the questions asked by other students are provided to facilitate your progress if you encounter the same problem.





&lt;BR&gt;


# Which libraries to install? #
For the **Java developers**, there might be a mismatch on using different jar files. Based on the feedback from other users, these libraries work perfectly fine:

  * apache-xmlrpc-3.1.3 (included xmlrpc-client and xmlrpc-common)
  * apache common codec 1.9  [only use the Base64 library

You can download them from <a href='http://grepcode.com/snapshot/repo1.maven.org/maven2/org.apache.xmlrpc/xmlrpc-client/3.1.3'>here</a>.





&lt;BR&gt;



&lt;BR&gt;



# Hints on different steps #
Here, you can find some hints on different steps.



&lt;BR&gt;



&lt;BR&gt;


### Obtaining Voucher ###
  * Normally, the vouchers are sent immediately to your KTH emails. If it takes more than the usual time, contact us to figure out the problem.





&lt;BR&gt;



&lt;BR&gt;


### Obtaining X.509 Certificate ###
  * Include your email address into the CSR as: _"emailAddress"_
  * Make sure the CSR is properly generated. It starts with _"-----BEGIN CERTIFICATE REQUEST-----"_ and ends with _"-----END CERTIFICATE REQUEST-----"_.
  * 
  * 




&lt;BR&gt;



&lt;BR&gt;


### Obtaining Ticket ###





&lt;BR&gt;



&lt;BR&gt;


### Obtaining Pseudonym ###




&lt;BR&gt;



&lt;BR&gt;


### Revocation ###
The PKI does not provide CRL or OCSP for X.509 certificates. It only provides them for anonymous credentials (the pseudonyms).




&lt;BR&gt;


# ERRORS #
kth-vespa returns appropriate errors for incorrect requests. Here, you can figure out some hints in case of receiving different errors.


## How to check if the servers are working ##
The following message shows that the LTCA server is properly running if you click on https://172.31.212.119/cgi-bin/ltca:


**405 Method must be POST**

**The Xmlrpc-c CGI server was unable to process your request. It could not process it even enough to generate an XML-RPC fault response.**

## What does ERR\_CODE\_DESERIALIZATION\_FAILED\_USING\_PROTO\_BUFF error mean? ##
This error indicates that at least one of the required fields is not fulfilled. Check the request to see if all the required fields are properly fulfilled.