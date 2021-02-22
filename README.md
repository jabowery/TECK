To try out The Electoral Corruption Killer, click this link for a live sandbox demo:

https://delegate.network/teck/audit

# Workflow For The Electoral Corruption Killer

## Introduction
*The Electoral Corruption Killer* is an *auditable* vote-by-proxy system designed to stop betrayals of the public by Congress such as occurred with the 1998 expansion of H-1b visas when Congress overwhelmingly disregarded the will of 82% of the public. See:

https://web.archive.org/web/20010217052101/http://www.ieeeusa.org/releases/1998/pr091698.html

It's based on a computer program consisting of less than 120 lines of Perl code (not counting preformatted text like this). TECK makes it easy for a small campaign to win against a major incumbent in an election for Representative or perhaps even Senator, at the State or perhaps even the National level. Unlike ordinary electronic voting systems with hundreds of thousands of lines of code and sophisticated database technology, TECK works by making all votes public via a website so anyone with sufficient interest can at any time verify the *audit*. The program script itself is designed to be simple and small so anyone with a modicum of computer system administration expertise can analyze and install it, but as already stated the key to security of this system is in the public availability of the *audit*, so don't be mislead by ease of analyzing a small script and the care with which the installation is done. That's not what is important.  Again: the key is the public availability of the *audit*. TECK works by keeping track of citizen delegates so that ordinary citizens *can* but don't *need* to be intimately involved with politics to exercise their legitimate rights as the ultimate keepers of security. If there is someone they trust, say an elder in a family or church, they simply declare their delegate to be that trustee. These trustees may in turn throw their delegates to other trustees. All delegates are revocable at any time. The sole plank in the campaign platform of TECK candidates is that they will make a good-faith attempt to abide by the votes of their constituents *as **represented** by their delegates* during the legislative session. Given the current corrupt state of electoral politics and the alienation of the voters from it, anyone who knows someone who can run a small computer system can make a credible bid against an incumbent as a TECK.

## To Kick-off Your Campaign
Kick off your campaign as The Electoral Corruption Killer with a bang! Or at least a bash. Here is a suggested procedure to create synergy between candidates for TECK and their constituents:

1. Set up a website for your office. This website must be able to run Perl CGI scripts that require as much as a CPU second on a modern processor and 100M of RAM.
2. Install the attached Perl CGI script on your website. To make the database writable you must, in the CGI directory where it is installed, execute the shell command: "touch audit_writable"
3. Obtain a dedicated computer system with an amount of RAM at least equal to 32M plus 1K for each voter in your district. This system will be used only for auditing delegates and votes.
4. Place the computer in a physically secure area, disconnected from all networks except the electrical grid.
5. Invite a variety of computer experts from the local community over for a campaign kick-off party. Admittance to the party is predicated on them agreeing not to touch the computer system and to report anyone attempting to touch the computer system. During this party you will all be in the same room as the computer system but the computer system will be roped off from the rest of the attendees and you will:
 1. Do a clean install of the latest version of Linux or FreeBSD with:
Perl, GUI interface, a web browser (probably Mozilla) and a web server (probably Apache) capable of running Perl CGI scripts.

 2. Copy the attached Perl CGI script (the file named `audit`) to the web browser's CGI directory (probably /usr/local/apache/cgi-bin).
 3. As root, cd to the CGI directory and to each directory above the CGI directory to execute the shell command:

"chmod a+w ." including the period but not the quotes.

 4. From the web browser hit the URL: http://localhost/cgi-bin/audit
 5. Satisfy yourselves that the script is working as expected. If not, obtain help from your guests. Just about any reasonably sophisticated computer system administrator will be able to solve the problem easily unless there is a problem with the system you were given.
 6. Obtain the names of computer professionals that are looking for work and give them the following campaign statement to pass to their circle of acquaintances:
"82% of the public opposed expansion of the H-1b visa program yet Congress voted nearly unanimously to expand the H-1b program. Representative democracy is neither representative nor democratic. People are staying away from the voting booths in droves. <Your name> is running for representative to change that. He will vote only the way you, his voters, tell him to vote either directly on each bill or, if you prefer, you can revocably delegate your votes to others (but not to <your name>). You will be able to see how you are telling him to vote by visiting his web site at <URL>. Your vote will be public so everyone can verify the honesty of the system."

 7. Say goodnight to your guests and secure the facility.

## Running Your Campaign and Office
During the campaign simply run your office as you would during the legislative session:

1. Solicit and accept input from voters on how they want to vote on various bills and to whom they wish to delegate their votes. Input it to the secured audit system.
2. Optimize your office as necessary to secure it and speed it. (An obvious suggestion is to give preference to processing easily-verified authorizations. For example, put up a caller-ID telephone answering computer for people to call. If they leave their name, and their caller ID is a listed phone number matching their name, then process their authorizations first. Process the others as you can afford the time and resources to authenticate them. Let people know how they can help ease your timely processing of their authorizations.)
3. Periodically (as often as you can afford given your resources) copy the audit_data.pl file to removable media and that copy to your website's CGI directory, treating your secured system's web access log as your transaction log for disaster recovery purposes.
4. Set audit_data.pl on your website to be read only for owner, group and world. The shell command for this is:
"chmod 444 audit_data.pl"

Copyright 2003 The Electoral Corruption Killer

The author grants the right to copy under the terms of the Reciprocal Public License. You may obtain a copy of RPL from:

http://www.opensource.org/licenses/rpl.php
