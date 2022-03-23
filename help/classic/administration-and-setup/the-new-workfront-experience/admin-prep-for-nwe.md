

# Prepare to move your organization to the new Adobe Workfront experience

As of March 31, 2022, Workfront will no longer support Adobe Workfront Classic. Because of this, you need to ensure that your organization is ready to move to the new Adobe Workfront experience. Your organization is unique, and it is difficult to predict how your network configuration and usage of Workfront will affect tthe new Adobe Workfront experience. To ensure a smooth transition, we highly recommend the following schedule:

| Goal |Deadline |Details  |
|---|---|---|
| Test the new Adobe Workfront experiencein your own account |As soon as possible |See [Test the new Workfront experience in your own account](#test2). |
| 30% of your organization's users are using the the new Adobe Workfront experience |Mid-January 2022 |See [Aim for 30% adoption by mid-January 2022](#aim). |
| 100% of your organization's users are using the new Adobe Workfront experience |March 31, 2022 |Workfront Classic will not be supported after this date. |

## Test your organization's readiness for the new Adobe Workfront experience

These tests allow you to identify possible network or configuration issues in your organization that may affect performance in the new Workfront experience.

* [Test the new Workfront experience in your own account](#test2) 
* [Aim for 30% adoption by mid-January 2022](#aim)

### Test the new Workfront experience in your own account

As the Workfront administrator, you can test the new Workfront experience in your own account.

>[!IMPORTANT]
>
>We recommend performing this test as soon as possible so that your IT department has time to make any configuration changes before your organization transitions to the new Adobe Workfront experience.

To identify possible configuration changes needed for your transition:

1. Switch your account to the new Adobe Workfront experience.

   For instructions, see [Switch your admin account to the new Adobe Workfront experience](../../administration-and-setup/add-users/create-and-manage-users/enroll-users-new-workfront-experience.md#switch2) in [Enroll users in the new Adobe Workfront experience](../../administration-and-setup/add-users/create-and-manage-users/enroll-users-new-workfront-experience.md).

1. Explore your organization's Workfront instance.

   Think about what areas of Workfront your company uses most frequently. Explore each area thoroughly, including performing actions that your users are likely to perform.

   For example, if your organization frequently uses projects with large numbers of tasks, you should explore some of those projects. You might try opening multiple projects at once, update user assignments, or create a project from a template. Anything your users do, do with your own account.

   Consider the following areas when exploring Workfront :

   * Home
   * The Workload Balancer
   * The Resource Planner
   * The Portfolio Optimizer
   * Documents
   * Projects with large numbers of tasks or issues
   * Large update streams
   * Reports with large amounts of data
   * Reports that use complex calculations 
   * Any other areas that your organization uses

1. Compare the performance of the new Adobe Workfront experience with Workfront Classic.

   >[!TIP]
   >
   >Log in to Workfront Classic as a different user in another window for easy comparison.

If you notice that some areas load significantly more slowly than in Workfront Classic, continue to [Troubleshoot common connection and performance issues](#troubles).

If the performance is largely the same between Workfront Classic and the new Adobe Workfront experience, then you can begin enrolling users in the new Adobe Workfront experience on a larger scale.

### Aim for 30% adoption by mid-January 2022

Because your own account might not reflect how others in your organization use Workfront, we highly recommend that you enroll at least 30% of your organization's users into the new Workfront experience by the middle of January 2022. These users will be able to identify any issues with your organization's transition early enough that your IT department can address those issues well before March 31, when Workfront Classic is longer supported.

If your users notice that some areas load significantly more slowly than in Workfront Classic, continue to [Troubleshoot common connection and performance issues](#troubles).

If the performance is largely the same between Workfront Classic and the new Adobe Workfront experience, then you can move the rest of your users to the new experience. All users must be enrolled in the new Workfront experience by March 31, 2022.

## Troubleshoot common connection and performance issues

Frequently, slower performance in Workfront is caused by issues in your organization's setup that Workfront cannot address. If you are noticing lag or slow loading in Workfront, check for the following issues.

>[!IMPORTANT]
>
>If you have trouble identifying and addressing performance issues in the new Workfront experience, contact the Adobe Workfront customer support team. We understand that configuration is unique and complicated for every organization, and we are happy to help you troubleshoot your organization's transition to the new Adobe Workfront experience.
>
>For information on contacting customer support, see [Contact Customer Support](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)

* [Common connection issues](#common) 
* [Other performance issues](#other)

### Common connection issues

* [Your local connection](#your) 
* [VPN](#vpn) 
* [Web Proxy](#web) 
* [Firewall](#firewall)

#### Your local connection

If you are working from your home or another public location, your internet connection might be unreliable. Running a speed test can help you identify if your internet connection is having difficulties. If your internet speeds are low, consider checking your WIFI setup.

Similarly, if you are working in an office and are experiencing slow performance, try working from home or another location. If performance is better at home, work with your IT&nbsp;department to identify and address the cause of the slow performance in the office.

#### VPN

Your organization might use a VPN (Virtual Private Network). VPNs allow users to connect to a private network over a public network, that is, from the outside of the private network. For example, if a user is working remotely, they might need to log in to a VPN to access data stored on the organization's private network. A VPN can affect data flow between your organization and Workfront.

Try disabling or logging out of your VPN. If performance improves while the VPN is disabled, work with your IT department to address the issue.

#### Web Proxy

Your organization might use a web proxy, also known as a proxy server. This proxy is a server that stands between your organization and the public web. Your organization communicates with the proxy, and the proxy communicates with the web. Your web proxy can affect data flow between your organization and Workfront.

Your network administrator or IT&nbsp;department can address issues with your web proxy.

#### Firewall

Your firewall is a security barrier between your organization's network and the public web. Firewalls maintain network security by only allowing data from trusted sources to pass into or out of the network.

Work with your network administrator or IT department to make sure your firewall is up to date.

For more information on how firewalls work with Workfront, including instructions for updating your firewall, see [Firewall overview](../../administration-and-setup/get-started-wf-administration/firewall-overview.md).

### Other performance issues

#### Your organization's Workfront settings

You might be able to improve your performance by altering settings or using other Workfront best practices.

For example:

* If large projects are taking a long time to load, set the list to display a smaller number of items.
* If a report is loading slowly due to complex calculations, consider simplifying the report.
* If long update streams cause performance issues, consider disabling system updates.

Optimizing for your organization's specific use cases can significantly benefit the performance of Workfront in your environment.
