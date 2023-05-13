Postmortem Report: Products API Outage (May 13, 2023)

Summary
On May 13, 2023, at approximately 10:30pm East African Time, the products section of our online application experienced an outage. The issue was caused by a problem with the API querying the products, which prevented customers from buying certain products. The problem was reported by the sales team and was fixed by the engineering team at approximately 11:45pm East African Time.

Timeline
10:30pm: The sales team noticed that customers were unable to buy certain products and reported the issue to the engineering team.
10:35pm: The engineering team started investigating the issue and identified the problem as being with the products API.
11:00pm: The engineering team continued to investigate and troubleshoot the problem.
11:30pm: The engineering team identified the root cause of the problem and began working on a fix.
11:45pm: The engineering team deployed a fix to the products API, and the issue was resolved.

Root Cause
The root cause of the outage was determined to be a problem with the products API. Specifically, a code change that had been made earlier in the day caused a compatibility issue with a third-party API that the products API relied on. This led to a cascading failure that ultimately resulted in the outage.

Resolution and Recovery
To resolve the issue, the engineering team rolled back the problematic code change and made a few modifications to the products API to ensure that it would work with the third-party API. The engineering team then tested the fix and deployed it to production. Once the fix was deployed, the sales team confirmed that customers were once again able to buy products as expected.

Lessons Learned
Communication between teams was key to resolving the issue quickly. The sales team's prompt reporting of the issue allowed the engineering team to start investigating and fixing the problem right away.
It's important to thoroughly test any code changes, especially those that involve external dependencies. In this case, the code change that caused the problem had not been fully tested with the third-party API that it relied on, leading to the compatibility issue.
We will implement additional monitoring and alerting to quickly detect and respond to similar issues in the future.

Action Items
Develop a plan to improve testing and quality assurance processes to prevent similar issues from occurring in the future.
Implement additional monitoring and alerting to quickly detect and respond to similar issues in the future.
Review incident response procedures to identify areas for improvement and implement changes as necessary.

