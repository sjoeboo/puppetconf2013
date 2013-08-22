scaling puppet infrastructute

why? Hyperscale computing, multi dc, cloud,dynamic environments

master vs masterless
	masterless w/ mcollective?

CA:
	only statful part of puppet.
	not needed w/ masterless
	CSR generated and signed by the CA
	Shared CRL across all CA machines

	clustering
		CA has lots of state
		masters are stateless
		reduce number of file shares..

	DNS based clustering
		many masters, single CA (We do this)
	Load balacing
		same as above, but LB instead of DNS RR (haproxy, mod_proxy, etc)
		
	Per region CA?
	Multicluster (we kind of do this)
	
	
Node classification @ scale:
	 
