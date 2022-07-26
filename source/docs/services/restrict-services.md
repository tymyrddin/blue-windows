# Start, stop, restart, enable, and disable services

You must be signed in as an administrator to be able to do these.

* If you stop, start, or restart a service, any dependent services are also affected. Starting a service does not automatically restart its dependent services.
* Changing the default service settings may prevent key services from running correctly. It is especially important to use caution when changing the Startup type setting of services that are configured to start automatically.
* Some services, such as Remote Procedure Call (RPC), Event Log, and Plug and Play, cannot be stopped by using the Services snap-in window or the net stop command. These services are required for the operating system to function properly.
* Create a restore point before making changes to the services. 
* If you disabled the wrong service and lost access to the computer, then try booting into Safe Mode to change the service back.

## "Startup Type" for Service

* Automatic - With a service in this state, it will start at boot time. Some services, when no longer required, will also automatically stop when not needed. If you find you do not need a service, place it into Manual or Disabled.
* Automatic (Delayed Start) - With a service in this state, it will start just after boot time. Some services, when no longer required, will also automatically stop when not needed. If you find you do not need a service, place it into Manual or Disabled.
* Automatic (Delayed Start, Trigger Start) - With a service in this state, it will start just after boot when specifically called.
* Manual (Trigger Start) - This is a version of Manual mode that allows Windows to start a service when specifically called and Microsoft’s answer to “too many services running all the time”.
* Manual - Manual mode allows Windows to start a service when needed. However, very few services will start up when required in Manual mode. If you find you need a service, place it into Automatic.
* Disabled - This setting will stop a service from starting, even if needed. Errors in the Event Viewer will show up complaining of that fact. Some services, while Disabled, will constantly complain. However, this situation is taken care of if placed in Manual. The service descriptions identifies those that should be in Manual vice Disabled.

## Examples

### Services window

* Open the Services snap-in window (open the Run dialog, type services.msc OR Administrative Tools -> Services)
* Choose a service and double click it. You can
  * Change its "Startup Type" (OR)
  * Click the Stop button (OR)
  * Enable/start a service: If the Startup type of the service is set to Disabled, then you will need to change it to either Manual, Automatic, or Automatic (Delayed Start) before you click the Start button (OR)
  * Disable a service: If the service shows a status of running, then click/tap on the Stop button, and wait until the service status shows as stopped before you diable it.

### Using net Command

Requires the elevated command prompt, knowing the service name, and the double quotes. The Display name of a service is 
the name displayed in the Services snap-in window, and in the service's properties.

    net stop "service name"
    net stop "display name of service"
    net start "service name"
    net start "display name of service"
