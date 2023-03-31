# torrc
A wonderfully reduced exit policy for the Tor software.



Here's what each option does:

`ORPort` and `DirPort`: Specifies the ports for incoming Tor connections.
`ExitPolicy`: Specifies the outgoing ports and protocols allowed by the exit node.
`ContactInfo` and `Nickname`: Identifies the exit node and provides contact information for the operator.
`BandwidthRate`, `BandwidthBurst`, and `AccountingMax`: Limits the amount of bandwidth used by the exit node.
`RelayBandwidthRate` and `RelayBandwidthBurst`: Limits the amount of bandwidth used by the relay node.
`Log`: Configures logging options for the Tor daemon.
`IPv6Exit`: Enables IPv6 support for the exit node.
`V3IdentOnion`: Enables v3 onion services for the exit node.
`HiddenServiceStatistics`: Disables onion service statistics collection.
`AllowSingleHopExits`: Disallows single-hop circuits for outgoing connections.
`ExitPolicyRejectPrivate`: Blocks outgoing traffic to private IP addresses.
`ExitRelay`: Identifies the node as an exit node.
`LongLivedPorts`: Specifies the ports that are likely to be used for long-lived connections.
`ClientRejectInternalAddresses`: Disallows connections to internal IP addresses.
`NumCPUs`: Limits the number of CPUs used by the Tor daemon.

# NOTE:

In this configuration file, the exit policy only allows outgoing traffic on port 53, which is used for DNS requests. This is a reduced exit policy that limits the risk of abuse of the exit node while still allowing it to be useful for common Internet activities.

Again, please note that this is just an example configuration and may need to be adjusted depending on your specific use case and network configuration.
