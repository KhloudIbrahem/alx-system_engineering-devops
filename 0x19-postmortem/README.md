We are talking tonight about an issue happened in an e-commerce site. As the internet is used everyday and becomes an important part of our lifes now. And any issue happened in a web application like this, it will affect large portion of people.


Issue Summary:

May 10, 2023, 2:30PM to 5:00PM (WAT), In our e-commerce site experienced a total failure. The website stopped responding and the users can’t access it during this time.

Impact:

The issue affected all the functionalities of the website. When the users trying to use it, it responds with error messages and unresponsive messages. We estimate that about 80% of the users are affected by this issue.

Root Cause:

The mandatory cause of this issue is a leak on the memory that causes in shutdown the server.

Timeline:

· 2:30 : The issue was detected by the monitoring team and told by it to the operations team.

· 2:35 : The operations team restarts the server to fix the issue, but, it doesn’t solve this issue.

· 2:40 : The team begin to investigation about the issue and they check the server configurations.

· 3:00 : During the investigation, they found that the memory was abnormally performed. They think that it was a leak.

· 3:15 : The team begin to check the code for the cause of this issue.

· 3:45 : The team found the issue and began to solve it.

· 4:30 : The team fix the issue and restart the server again.

· 4:40 : The website begins to work again full potential.

Misleading investigation/ Debugging paths:

In the beginning, the operations team think that it is a problem of server configurations, but, with time and more investigation, they found the true reason of the issue as it is a leak on the memory in the code.

Incident escalation:

The incident was initially handled by the operations team and was escalated to the development team when they realized that the issue was in the application code.

Resolution:

The memory leak was fixed and identified. The fix included code optimization and memory management then the server returns to work again with its full potential.

Corrective and Preventative Measures:

To prevent this issue in the future, we will follow these corrective and preventative measures:

· Make regular code reviews to catch memory leaks.

· Make more tests in the application to get all the memory leaks in the application before become with the production.

· Implement robust monitoring of server performance and resources usage.

· Improve documentation and training for the operations team to handle this issue in the future.

Specific tasks to address the issue include:

· Making comprehensive review of the application code.

· Applying tests in the application code to get all memory leaks.

· Updating monitoring tools to include more granular resource usage data.

Provide more training for the operations team members on troubleshooting web application issues.
