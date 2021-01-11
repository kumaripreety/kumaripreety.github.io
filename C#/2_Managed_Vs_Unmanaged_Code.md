## 2. Managed Vs Unmanged Code



**Managed code** is the code which is managed by the CLR(Common Language Runtime) in *.NET Framework*. Whereas the **Unmanaged** code is the code which is directly executed by the operating system. Below are some important differences between the Managed code and Unmanaged code:





| MANAGED CODE                                                 | UNMANAGED CODE                                               |
| :----------------------------------------------------------- | :----------------------------------------------------------- |
| It is executed by managed runtime environment or managed by the CLR. | It is executed directly by the operating system.             |
| It provides security to the application written in .NET Framework. | It does not provide any security to the application.         |
| Memory buffer overflow does not occur.                       | Memory buffer overflow may occur.                            |
| It provide runtime services like Garbage Collection, exception handling, etc. | It does not provide runtime services like Garbage Collection, exception handling, etc. |
| The source code is complied in the intermideate language know as *IL or MSIL or CIL*. | The source code direclty compile into native langugae.       |
| It does not provide low-level access to the prgrammer.       | It provide low-level access to the prgrammer.                |