all: activatedclienttypeentry_client.exe activatedclienttypeentry_server.exe 

activatedclienttypeentry_server.exe: activatedclienttypeentry_server.vb activatedclienttypeentry_share.dll
	vbc activatedclienttypeentry_server.vb /r:activatedclienttypeentry_share.dll

activatedclienttypeentry_client.exe: activatedclienttypeentry_client.vb activatedclienttypeentry_share.dll
	vbc activatedclienttypeentry_client.vb /r:activatedclienttypeentry_share.dll

activatedclienttypeentry_share.dll: activatedclienttypeentry_share.vb
	vbc /t:library activatedclienttypeentry_share.vb

