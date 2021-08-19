To try out The Electoral Corruption Killer, click this link for a live sandbox demo:

https://delegate.network/teck/sandbox/audit


# Introduction
*The Electoral Corruption Killer* is an *auditable* vote-by-proxy system designed to stop betrayals of the public by Congress.

Imagine every member of Congress were pressured into making one and only one campaign promise:

"I will cede my voting power to my constituents."

Under TECK:

* Political campaigns are simple demonstrations of how constituents would vote on the bills currently before Congress.
* Any voter can, at any time, audit whether this campaign promise is being kept or not.
* Constituents may auditably delegate their voting power and, at-will, recall their delegation.
* All Congressional negotiations devolve to negotiations between constituent delegations.

TECK works by making all votes, delgated or direct, public via a website so anyone with sufficient interest can at any time verify the *audit*. The key is the public availability of the *audit*. TECK works by keeping track of citizen delegates so that ordinary citizens *can* but don't *need* to be actively involved with politics to exercise their legitimate rights as the ultimate auditers. If there is someone they trust, say an elder in a family or church, they simply declare their delegate to be that trustee. These trustees may in turn throw their delegates to other trustees. **All delegates are revocable at any time**. The sole plank in the campaign platform of TECK candidates is that they will make a good-faith attempt to abide by the votes of their constituents *as **represented** by their delegates* during the legislative session. Given the current corruption of electoral politics and the alienation of the voters from it, anyone who knows someone who can run a small computer system can make a credible bid against an incumbent as a TECK.

# Workflow For The Electoral Corruption Killer

## Installation

1. Copy the files named **audit** **audit_data.pl** and **audit_writable** to a directory capable of running cgi web scripts at http://localhost.
2. In your web browser, enter the localhost URL for the **audit** script.  This should present you with the user interface with changes enabled.
3. After verifying the script is working, delete the **audit_data.pl** file.
4. In your web browser, enter the localhost URL for the **audit** script again.  This will initialize an empty **audit_data.pl** file.
5. Create a symbolic link to the localhost accessible cgi directory copies of **audit** and **audit_data.pl** from a directory capable of running cgi web scripts at a public domain name.
6. In your web browser, enter the public domain name URL for the **audit** script.  This will make public the current audit.

## Running Your Campaign and Office
During the campaign simply run your office as you would during the legislative session:

1. Solicit and accept input from voters on how they want to vote on various bills and to whom they wish to delegate their votes. 
2. Input their preferences via the localhost URL.
3. Optimize your office as necessary to secure it and speed it. Some suggestions:
3.1. Give preference to processing easily-verified citizens.
3.2. Obtain property assessment records from your county and mail a registration ID to each residential address.  Ask them for that ID when they call in.

Copyright 2003 The Electoral Corruption Killer

The author grants the right to copy under the terms of the Reciprocal Public License. You may obtain a copy of RPL from:

http://www.opensource.org/licenses/rpl.php
