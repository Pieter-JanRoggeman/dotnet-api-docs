all: Share.dll server.exe client.exe

Share.dll: ChannelServices_syncdispatchmessage_Share.cs
	csc /t:library ChannelServices_syncdispatchmessage_Share.cs

server.exe: ChannelServices_syncdispatchmessage_Server.cs ChannelServices_syncdispatchmessage_Share.dll
	csc ChannelServices_syncdispatchmessage_Server.cs /r:ChannelServices_syncdispatchmessage_Share.dll

client.exe: channelservices_syncdispatchmessage_client.cs ChannelServices_syncdispatchmessage_Share.dll
	csc ChannelServices_syncdispatchmessage_client.cs /r:ChannelServices_syncdispatchmessage_Share.dll