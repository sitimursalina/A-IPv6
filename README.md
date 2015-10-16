# A-IPv6
Company A-how to get IPv6


package ipv6;

import java.net.InetAddress;
import java.net.NetworkInterface;
import java.net.SocketException;
import java.net.UnknownHostException;

public class AIPv6 {

	public static void main(String args[]) throws UnknownHostException {
	
	InetAddress address;
        try {

		    address = InetAddress.getByName(args[0]);
		    
		    if (address.isAnyLocalAddress()){
					System.out.println(address + " wildcard address. ");
				}
				if (address.isMCLinkLocal()) {
					System.out.println(address + " multicast address. ");
					
					} else  {
					System.out.println(address + " is a unicast address.");
                                        }

        }
	    }
	    
	}
