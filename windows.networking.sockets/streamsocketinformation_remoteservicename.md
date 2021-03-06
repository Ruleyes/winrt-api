---
-api-id: P:Windows.Networking.Sockets.StreamSocketInformation.RemoteServiceName
-api-type: winrt property
---

<!-- Property syntax
public string RemoteServiceName { get; }
-->

# Windows.Networking.Sockets.StreamSocketInformation.RemoteServiceName

## -description
Get the service name or TCP port number of the remote network destination associated with a [StreamSocket](streamsocket.md) object.

## -property-value
The service name or TCP port number of the remote network destination.

## -remarks
The [RemoteServiceName](streamsocketinformation_remoteservicename.md) property represents the remote service name or TCP port number for the remote network destination associated with a [StreamSocket](streamsocket.md) object. The remote service name or TCP port that a [StreamSocket](streamsocket.md) object connects to is passed in the *remoteServiceName* parameter to the [ConnectAsync](streamsocket_connectasync.md) method on the [StreamSocket](streamsocket.md).

The [RemoteServiceName](streamsocketinformation_remoteservicename.md) property can be one of the following:


+ A numeric literal for a TCP port number (80 for the TCP port typically used for the HTTP protocol, for example).
+ A string alias for a port number ("http", for example) that matches a string in the following file on the local computer: %WINDIR%\system32\drivers\etc\services
+ A service name that can be resolved by a namespace provider using a SRV record.
The [RemoteHostName](streamsocketinformation_remotehostname.md) property represents the remote service name or TCP port number for the remote network destination associated with a [StreamSocket](streamsocket.md) object.

After a connection is established, the [RemoteAddress](streamsocketinformation_remoteaddress.md) property contains the IP address and the [RemotePort](streamsocketinformation_remoteport.md) property contains the TCP port number of the remote endpoint for the socket connection.

## -examples

## -see-also
[How to use advanced socket controls ](http://msdn.microsoft.com/library/2e1071d8-a1c7-44c0-b93a-31a701d431c4), [How to use advanced socket controls ](http://msdn.microsoft.com/library/f2c5be73-3461-452e-a38f-d2ddef9b5682), [ConnectAsync](streamsocket_connectasync.md), [RemoteAddress](streamsocketinformation_remoteaddress.md), [RemoteHostName](streamsocketinformation_remotehostname.md), [RemotePort](streamsocketinformation_remoteport.md), [StreamSocket](streamsocket.md)

## -capabilities
ID_CAP_NETWORKING [Windows Phone]
