For AWS:
Instance metadata is data about your instance that you can use to configure or manage the running instance. Instance metadata is divided into categories, for example, host name, events, and security groups. You can also use instance metadata to access user data that you specified when launching your instance.

To view all categories of instance metadata from within a running instance, use the following URI.
http://169.254.169.254/latest/meta-data/
The IP address 169.254.169.254 is a link-local address and is valid only from the instance.
Note that we are not billed for HTTP requests used to retrieve instance metadata and user data.

For Azure:
The Azure Instance Metadata Service (IMDS) provides information about currently running virtual machine instances. You can use it to manage and configure your virtual machines. This information includes the SKU, storage, network configurations, and upcoming maintenance events.
IMDS is a REST API that's available at a well-known, non-routable IP address (169.254.169.254). You can only access it from within the VM. Communication between the VM and IMDS never leaves the host.

1st Command: To query the meta data of a VM within Azure and provide a json formatted output.
2nd Command: For VM Tags (Example for: data key to be retrieved individually)
3rd Command: To get a unique ID for a VM (Example for: data key to be retrieved individually)

