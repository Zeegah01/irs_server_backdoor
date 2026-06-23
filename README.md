# irs_server_backdoor
A perl backdoor script on IRS server 13281
#Key take away

As a cybersecurity analyst, while analysing exploit codes, you should focus on this questions:


1.How does it communicate?
    TCP socket
    UDP socket
    HTTP request
2.What vulnerability is being abused?
    In this case, a backdoored IRC daemon that executed shell commands.
    What data is sent?
    The payload strings.
3.What indicators of compromise (IOCs) would appear?
    Unexpected outbound downloads (wget)
    Execution from /tmp
    New processes
    IRC service crashes
    File deletion attempts
4.What detection opportunities exist?
    IDS/IPS signatures for the malicious command pattern.
    Monitoring execution from temporary directories.
    Logging unusual child processes spawned by the IRC daemon.
