# agentSm1tH.pl
Who is it

#!/usr/bin/perl
# @nu11secur1ty
use warnings;
use strict;
use diagnostics;
use Term::ANSIColor;

print "Please show me the domain which you want to see, who is\n";
print "For example (example.com)\n";

our $domain = <STDIN>;
        our $get_IP = `ping -c 1 $domain`;
                print "$get_IP\n";
                print "Please paste the ip for the next step\n";
                        our $the_target = <STDIN>;

                                print color('bold red');
                                print "DNS is...\n";
                                print color('reset');
                                        my $NS_ = `dig -t ns $domain`;
                                        print "$NS_\n";

                our $prusni_mu_fantastikata = `whois $the_target`;
                        print "$prusni_mu_fantastikata\n";

                our $check_for_openports = `nmap -A $the_target`;
                        print "$check_for_openports\n";
        exit 0;
