## DomainKeys Identified Mail:
An email authentication method designed to detect forged header fields and content in emails. DKIM enables the receiver to check if email headers and content have been altered in transit.

Think of a DKIM signature in the email header sort of as an envelope seal: the sending server "seals" an email message on its way out by affixing a signature to the message; anyone who attempts to tamper with the email further in transit, must break the seal to do so, hence inevitably detectable by the email receiver.

## How it works:
Sample here: https://dmarcly.com/blog/how-to-implement-dmarc-dkim-spf-to-stop-email-spoofing-phishing-the-definitive-guide#what-is-dkim